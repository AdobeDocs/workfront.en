---
name: release-notes-formatter
description: Format and validate Workfront release notes for consistency, correct structure, and proper linking. Use only for release note files in product-releases directories, or when the user mentions release notes, product releases, or quarterly releases. Do not apply to how-to articles or general documentation.
---

# Release Notes Formatter

Formats and validates Adobe Workfront release notes in the `help/quicksilver/product-announcements/product-releases/` directory.

## Page Types

Identify the page type from file path and content:

| Page Type | File Pattern | Template |
|-----------|-------------|----------|
| **Overview** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **Product Area** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **Planning** | `planning-release-activity-{YY}-q{N}.md` | Similar to product area |
| **Look and Feel** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#look-and-feel](reference.md#look-and-feel-page-template) |

## Step 0: Determine the Quarter (do this before anything else)

>[!IMPORTANT]
>
>Never assign a feature to a doc-quarter using calendar-quarter math on its Preview or Production date. Doc-quarter is based on which **monthly release** the feature ships in, per Workfront's internal release-calendar grouping, which is offset from the calendar quarter — see the [2026 Release Calendar](#2026-release-calendar) table near the end of this file. For example, a feature with a Production date of August 13, 2026 belongs in doc-quarter `26-q4`, not `26-q3`, because the August monthly release maps to `26-q4`.
>
>The "Quarter Mapping" table further down (Written Form / Months) is for writing out quarter names in titles (e.g., "Third Quarter" for Q3) — it is **not** sufficient on its own for deciding which quarter's files a feature belongs in. Always cross-check against the Release Calendar table before creating or editing any file.
>
>If a feature's Production date doesn't appear in the Release Calendar table (e.g., it's beyond the table's date range), ask the user for an updated calendar rather than guessing.

## Formatting Workflow

### Step 1: Validate Frontmatter

Required fields for all release note pages:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Rules:
- `feature` must be exactly `Product Announcements`
- `recommendations` must be exactly `noDisplay, noCatalog`
- Never invent an `exl-id` — only include if one already exists
- Do not add `draft: Probably` to real pages (templates only)

### Step 2: Validate Structure by Page Type

#### Product Area Pages

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Example: `# Second Quarter 2026 Administrator enhancements`
   - Quarter must be written out: "First Quarter", "Second Quarter", "Third Quarter", "Fourth Quarter"

2. **Intro paragraph**: Describes the area and links to the overview
   - Must link to the **correct quarter's** overview file
   - Common bug: linking to previous quarter (e.g., `26-q1` instead of `26-q2`)

3. **H2 per feature**: Feature title as heading
   - **Newest features first** — the most recent release note must appear as the first H2 after the intro paragraph
   - Older features follow in reverse chronological order

4. **Date callout block** after each H2:
```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

5. **Body**: Feature description, then link to help documentation

#### Overview Pages

1. **H1**: `{Written Quarter} release overview`

2. **Intro paragraph** with scheduled release month

3. **`>[!IMPORTANT]` block** with release schedule table

4. **H2 `Adobe Workfront enhancements`** with bullet list of anchor links:
```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

5. **H3 per product area** with HTML feature table (see [reference.md](reference.md#overview-feature-table))
   - Within each table, **newest features first** — the most recent row appears at the top of the table (after the header row)

6. **Trailing sections** (H2): Release notes for other areas, Desktop proofing viewer updates, Announcements, API version, Maintenance Updates, Training updates

### Step 3: Validate Links

- **Overview link in product area pages**: Must point to the same quarter
  - Correct: `26-q2-release-activity/26-q2-release-overview.md`
  - Wrong: `26-q1-release-activity/26-q1-release-overview.md`
- **Anchor links in overview**: Must match the H3 IDs (lowercase, hyphens)
- **Feature links in overview tables**: Must use `class="MCXref xref" xrefformat="{para}"`
- **Help doc links**: Must start with `/help/quicksilver/`

### Step 4: Validate Dates

- Format: `{Month} {Day}, {Year}` (e.g., "March 12, 2026")
- Use `TBD` for unknown dates
- Dates in the product area page `>[!NOTE]` block must match the corresponding overview table row
- Preview dates should precede Production dates

### Step 5: Common Fixes

Apply these fixes when formatting:

| Issue | Fix |
|-------|-----|
| Wrong overview link quarter | Update to match file's own quarter |
| Missing `>[!NOTE]` date block | Add block after H2 feature heading |
| Inconsistent date format | Standardize to `Month Day, Year` |
| Missing blank line before `>[!NOTE]` | Add blank line |
| Extra spaces in callout lines | Trim trailing whitespace |
| HTML in product area pages | Keep as markdown (HTML is for overview tables only) |
| Missing `exl-id` | Leave it out — do not generate one |

### Step 6: Update the TOC

Whenever you create a **new** release-note page (overview or product area), add it to `help/quicksilver/TOC.md` in the same change. A page that is not in the TOC will not appear in the published navigation, even if links in the overview table point to it.

Where to add it:

- The TOC has a section per quarter under a heading like `* 2026 Q3 Release {#release-26-q3}`. If the quarter heading does not exist yet (first page of a new quarter), add it above the previous quarter so the newest quarter is on top.
- Under that quarter heading, list the pages in this order:
    1. **Overview** first (`Third Quarter 2026 release overview`).
    2. **Product-area pages** alphabetically by area name (Administrator, Documents, Enterprise Operations, Projects, Reporting, Requesting).
    3. **Other enhancements** last (always after the alphabetical product areas).

Each TOC entry is a markdown link using the page title and the absolute repo path:

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Match indentation (six spaces) to the surrounding entries. Use the page H1 verbatim as the link text — for example `Documents enhancements`, `Requesting enhancements` (not `Requests`) — so TOC labels match prior quarters.

Common mistakes to avoid:

- Creating a product-area page without adding it to the TOC.
- Linking to a different quarter's overview from the new product-area page (Step 3).
- Inserting a new quarter's pages under the previous quarter's heading.

### Step 7: Update the home page

Whenever you create a **new quarter's overview page** (i.e., this is the first page of a new quarter, not just a new product-area page added to an existing quarter), update `help/quicksilver/home.md` in the same change:

- In the `>[!TAB Latest release]` section, replace the release overview link with the new quarter's overview link.
- Also in that section, update the Adobe Workfront Planning release activity link to point to the new quarter's planning file (`planning-release-activity-{YY}-q{N}.md`), if one exists.
- In the `>[!TAB {YYYY} releases]` tab for the current year, add the new quarter's overview link at the top of the list, above the previous quarter's entry.

Do not touch `home.md` when only adding a product-area page to a quarter that already has an overview page listed there.

Common mistakes to avoid:

- Creating a new quarter's overview page without updating `home.md`'s "Latest release" tab (it will keep pointing to the old quarter).
- Forgetting to also add the new quarter to the current-year tab list.

## File Naming Conventions

| Type | Pattern | Example |
|------|---------|---------|
| Overview | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Product area | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Directory | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Standard area slugs: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Quarter Mapping

>[!NOTE]
>
>This table is for writing out quarter names (e.g., in an H1 or title). It does NOT determine which quarter's files a feature belongs in — use the [2026 Release Calendar](#2026-release-calendar) table below for that, since doc-quarter is offset from calendar-quarter.

| Quarter | Written Form | Months |
|---------|-------------|--------|
| Q1 | First Quarter | Jan–Mar |
| Q2 | Second Quarter | Apr–Jun |
| Q3 | Third Quarter | Jul–Sep |
| Q4 | Fourth Quarter | Oct–Dec |

**Important — the doc quarter used in file names (`26-q3`, `26-q4`, etc.) is offset by one month from this calendar mapping.** It follows Workfront's internal release-calendar grouping instead, where each doc quarter = the two preceding monthly releases + the quarterly release month. For example, doc quarter `26-q3` covers the May/June/July 2026 monthly releases (quarterly release `2026.07`), and doc quarter `26-q4` covers the August/September/October 2026 monthly releases (quarterly release `2026.10`). Always check the release calendar below (or ask for an updated one) before assuming a file's quarter based on the calendar-quarter table above.

## 2026 Release Calendar

Source: "2026 Monthly Release Calendar" (Adobe corp wiki, AWF space — `wiki.corp.adobe.com`, space key AWF, title "2026 Monthly Release Calendar"). WebFetch cannot reach this page (requires Adobe SSO); ask the user to paste an updated PDF/table when dates are needed beyond what's captured here.

| Release Month | Final Preview | Production | Monthly Release | Quarterly Release | Doc Quarter |
|---|---|---|---|---|---|
| Nov 2025 | 30-Oct-2025 | 13-Nov-2025 | 2025.11 | 2026.01 | 26-q1 |
| Dec 2025 | 27-Nov-2025 | 11-Dec-2025 | 2025.12 | 2026.01 | 26-q1 |
| Jan 2026 | 23-Dec-2025 | 15-Jan-2026 | 2026.01 | 2026.01 | 26-q1 |
| Feb 2026 | 29-Jan-2026 | 12-Feb-2026 | 2026.02 | 2026.04 | 26-q2 |
| Mar 2026 | 26-Feb-2026 | 12-Mar-2026 | 2026.03 | 2026.04 | 26-q2 |
| Apr 2026 | 02-Apr-2026 | 16-Apr-2026 | 2026.04 | 2026.04 | 26-q2 |
| May 2026 | 30-Apr-2026 | 14-May-2026 | 2026.05 | 2026.07 | 26-q3 |
| Jun 2026 | 28-May-2026 | 11-Jun-2026 | 2026.06 | 2026.07 | 26-q3 |
| Jul 2026 | 07-Jul-2026 | 16-Jul-2026 | 2026.07 | 2026.07 | 26-q3 |
| Aug 2026 | 30-Jul-2026 | 13-Aug-2026 | 2026.08 | 2026.10 | 26-q4 |
| Sep 2026 | 03-Sep-2026 | 17-Sep-2026 | 2026.09 | 2026.10 | 26-q4 |
| Oct 2026 | 01-Oct-2026 | 15-Oct-2026 | 2026.10 | 2026.10 | 26-q4 |
| Nov 2026 | 29-Oct-2026 | 12-Nov-2026 | 2026.11 | 2027.01 | 27-q1 |
| Dec 2026 | 26-Nov-2026 | 10-Dec-2026 | 2026.12 | 2027.01 | 27-q1 |
| Jan 2027 | 05-Jan-2027 | 14-Jan-2027 | 2027.01 | 2027.01 | 27-q1 |

Notes on using this table:

- **Final Preview** is the last date features may appear in Preview for that monthly release — use it for the overview page's "last date that features may appear in the Preview environment" bullet (quarter-ending month only).
- **Production** is the official Production-for-everyone date for that monthly release.
- For the quarter-ending month (the one matching the Quarterly Release column), the overview page's schedule table lists that month's release **twice**: once in the "Monthly release" column dated **one day before** the Production date (the fast-release date), and once in the "Quarterly release" column dated the actual Production date. Non-final months in a quarter use the same Production date in both the monthly listing and any "fast release" references — no adjustment needed.
- This table only goes through January 2027. When later dates are needed, ask the user for an updated calendar rather than guessing.

The quarterly production release typically lands on the Thursday of the second full week of the last month of the quarter.

## Validation Checklist

When reviewing a release note file, verify:

- [ ] Frontmatter has all required fields with correct values
- [ ] H1 matches the page type format
- [ ] Overview link points to the correct quarter
- [ ] Each feature has a `>[!NOTE]` date block (product area pages)
- [ ] Date format is consistent (`Month Day, Year`)
- [ ] Feature table rows in overview match product area page content
- [ ] No broken internal links
- [ ] Anchor links in overview match H3 section IDs
- [ ] Features are ordered newest-first (both product area pages and overview tables)
- [ ] New release-note pages are listed in `help/quicksilver/TOC.md` under the correct quarter, with the overview first and product areas in alphabetical order (Other last)
- [ ] If a new quarter's overview page was created, `help/quicksilver/home.md` "Latest release" tab and the current-year tab point to it

## Additional Resources

- For complete HTML templates and examples, see [reference.md](reference.md)
