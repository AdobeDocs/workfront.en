---
name: clean-el-traffic-csv
description: Cleans a raw Experience League / Adobe Analytics traffic CSV export down to Workfront-only pages, sorted by Page Views. Use when the user provides an Experience League page-traffic CSV (columns like "Page URL Generic", "Unique Visitors", "Visits", "Page Views") and asks to clean, filter, or process it, or mentions "documentation tracking" / "most viewed articles" spreadsheets.
---

# Clean Experience League traffic CSV

Turns a raw Adobe Analytics Freeform-table export of Experience League page traffic into a clean, Workfront-only, deduplicated CSV sorted by Page Views, overwriting the original file.

## Input shapes

The input may be one of two shapes:

1. **Raw export** — starts with metadata comment lines (`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"`, etc.), followed by a hierarchical breakdown table (e.g. `Solution (v2)` → `workfront` → `Page URL Generic (v33)` → individual URL rows). The literal cell `Page URL Generic (v33)` (or similar `Page URL Generic ...` label) appears partway down, in the second column.
2. **Already-clean CSV** — first row is already a plain header like `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, with no metadata rows or extra leading columns.

Detect which shape you have before starting: if row 1 is a plain header row matching shape 2, skip straight to Step 2 (no date range will be available, so also skip Step 7 unless the user supplies a date range separately).

## Workflow

### Step 0: Capture the date range (raw export only, before deleting anything)

Find the metadata line near the top matching `# Date: <range>` (e.g. `"# Date: Jul 1, 2026 - Jul 31, 2026"`). Record `<range>` (e.g. `Jul 1, 2026 - Jul 31, 2026`) — it's needed later in Step 7. Do this before any rows are deleted.

### Step 1: Strip the raw export down to a plain table (raw export only)

1. Find the row containing the cell `Page URL Generic (...)` (it's in the second column in the standard export).
2. Delete every row above that row, including the metadata comment lines and the `Solution (v2)` / `workfront` subtotal rows.
3. Delete every column to the left of the `Page URL Generic` cell (in the standard export, this is just column A).
4. On that same row (now the header row), replace the numeric subtotal values to the right of `Page URL Generic (...)` with the literal headers, in order: `Unique Visitors`, `Visits`, `Page Views`. Leave the `Page URL Generic (...)` cell itself unchanged.

Result: a plain CSV with header `Page URL Generic (v33),Unique Visitors,Visits,Page Views` followed by one row per URL.

### Step 2: Keep only Workfront rows

For every data row, check whether the URL contains the literal substring `/workfront/` (slash on both sides). Locale prefix doesn't matter (`/en/`, `/zh-hans/`, etc. — all stay as long as the product segment matches).

- Delete the row if the URL does **not** contain `/workfront/` as a path segment — this removes other products such as `workfront-fusion`, `workfront-learn`, `proofhqpapi`, etc. (a substring like `tutorials-workfront` does **not** count — the match must be the exact segment `/workfront/`).
- Keep the row otherwise.

### Step 3: Trim the URL

For each surviving row, find `/using` in the URL and keep only the portion from (and including) the `/` that follows it onward, discarding everything before and including `/using`.

Example: `https://experienceleague.adobe.com/en/docs/workfront/using/home` → `/home`

If `/using` isn't found in a Workfront row's URL, leave that URL unchanged and flag it for the user rather than guessing.

### Step 4: Strip fragment/query suffixes

If the trimmed URL contains a `#` or `?`, delete that character and everything after it.

Example: `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### Step 5: Merge duplicates

After trimming, multiple rows may now share the same URL (e.g. two different locale rows that collapse to the same path). Combine all rows with an identical URL into one row, summing `Unique Visitors`, `Visits`, and `Page Views` independently.

Example: `/home,2,2,3` and `/home,5,6,7` → `/home,7,8,10`

### Step 6: Sort by Page Views

Sort all data rows by `Page Views` descending (largest first). The header row stays fixed at the top, above the sorted data.

### Step 7: Add the date range row (raw export only, if captured in Step 0)

Before inserting it, strip any commas out of the captured date range (e.g. `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`) — the raw range has commas that would otherwise be misread as CSV column separators on that row.

Insert one new row at the very top, above the header row, containing just the comma-stripped date range.

Final row order: date range row → header row → sorted data rows.

### Step 8: Save

Overwrite the original input file in place with the cleaned result.

## Out of scope

Posting or sharing the cleaned CSV (e.g. to Slack) is a separate, not-yet-defined step — do not attempt to attach or upload the file anywhere as part of this skill.

## Implementation (raw export)

For a raw export, run Steps 0–8 with this tested PowerShell script rather than editing rows by hand — it's faster and less error-prone for files with hundreds of rows. Substitute the real file path for `$path`.

Before running, check whether the file is locked (e.g. open in Excel) — if `Set-Content` fails with "being used by another process," ask the user to close it, then re-run.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8
```

For an already-clean CSV (input shape 2), skip the header-relocation and date-range logic — just run Steps 2–6 and 8 on the existing header/rows as-is.
