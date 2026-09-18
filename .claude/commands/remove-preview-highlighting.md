---
name: remove-preview-highlighting
description: >-
  Removes Workfront preview-only documentation framing for GA (how-to/reference
  topics outside product-announcements committed by the current git user in a
  given date range): preview boilerplate snippets, class="preview" HTML, and
  parallel in-preview vs in-production steps or sections. Use when the user
  says "remove preview highlighting," preview GA cleanup, or production release
  doc updates for preview-tagged content.
---

# Remove preview highlighting (Workfront)

## Scope

Apply only when **all** are true:

1. The user invoked this workflow (e.g. says **"remove preview highlighting"** or clearly the same intent).
2. The Markdown file's path does **not** contain **`product-announcements`** (exclude the whole folder tree, e.g. release notes, betas, announcements under `help/quicksilver/product-announcements/`).
3. The Markdown file is **not** listed under **[Excluded paths](#excluded-paths)** below.
4. The Markdown file appears in `git log` as having preview content **added or modified** by the current git user within the user-specified date range (see Inventory step).
5. The article has **at least one** of:
   - Preview-environment **language in body prose or real snippet paragraphs** (typical patterns: "highlighted information," "Preview environment," "not yet generally available," fast-release notes)—**not** a match from **link text alone** on a TOC/index page (see below); or
   - Any HTML element with **`class="preview"`** (e.g. `<span class="preview">`, `<div class="preview">`); or
   - A preview snippet **variable** such as **`{{highlighted-preview}}`** or **`{{highlighted-preview-article-level}}`**.

If scope is unclear, confirm before editing.

**TOC / index pages — always skip this case:** **Never** put a file on the inventory when the **only** preview-related wording is **inside** a markdown link's display text pointing at **another** article (e.g. *Send a report in the Preview Sandbox environment*) **and** the file has **no** `class="preview"`, **no** snippet variables, and **no** preview boilerplate in **prose outside of links**. This is not preview highlighting on that page—it is only a TOC mention. Applies to any index/TOC, not only one file.

### Excluded paths

Never add these to the inventory or edit them in this workflow unless the user explicitly overrides:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md` — parallel Preview vs Production limits need a deliberate editorial decision outside automation.
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md` — reports TOC; sole "preview" signal is the link to the Preview Sandbox delivery article.

## Required workflow (human in the loop)

Do **not** bulk-edit the repo without approval.

1. **Inventory**  
   a. **Ask the user which quarterly release** they are removing preview highlighting for (e.g. "Q3 2026" or "2026.07").  
   b. **Fetch the release calendar** from `https://wiki.corp.adobe.com/spaces/AWF/pages/3631617814/2026+Monthly+Release+Calendar` using the adobe-wiki MCP tool. Find:
      - The **Production Release Date** of the **previous** quarterly release → `--since`.
      - The **Production Release Date** of the **target** quarterly release → `--until`.
      - Quarterly releases are identified by the "Quarterly Release Name" column (e.g. 2026.01, 2026.04, 2026.07, 2026.10).
      - **If the current date is in Q4 (October–December):** after fetching the current year's calendar, ask the user to provide the URL for next year's release calendar, then fetch that too so all quarterly production dates needed are available.
   c. Determine the current git user, then run the following using the production release dates from step b:

      ```bash
      GIT_USER=$(git config user.name)
      git log --since="YYYY-MM-DD" --until="YYYY-MM-DD" \
        --author="$GIT_USER" --name-only --pretty=format: \
        -- "help/quicksilver/**/*.md" | sort -u | grep -v '^$'
      ```

   d. From those results, **filter to files where the current user's commits in the date range actually added or modified preview content**. For each candidate file, check whether the user's commits introduced preview markers:

      ```bash
      git log --since="YYYY-MM-DD" --until="YYYY-MM-DD" \
        --author="$GIT_USER" -p -- "<file>" | \
      grep -q '^\+.*class="preview"\|^\+.*{{highlighted-preview\|^\+.*highlighted information\|^\+.*not yet generally available'
      ```

      Include the file only if this grep matches (exit code 0). This avoids false positives where a user made an unrelated edit to a file whose preview highlighting was added by someone else.

   e. **Omit** any path under **`product-announcements`**, any **[Excluded path](#excluded-paths)**, and any **TOC/index** page per the TOC rule above.  
   f. Present the resulting sorted list. If the user says a listed file has no preview highlighting, remove it from the run and tighten criteria rather than forcing edits.

2. **Start**  
   Ask whether to begin with the **first** article in the list (or a path the user names).

3. **Per article — show first, edit after OK**  
   - Read the file.  
   - Propose edits clearly: **before/after excerpts** or a focused diff-style description of what will change.  
   - **Wait** for explicit approval (e.g. "okay," "apply," "yes") before writing the file.

4. **After each file**  
   Ask whether to move to the **next** article (or stop / skip).

## Content rules (GA: preview content becomes the doc)

When removing preview highlighting for **general availability**, the goal is: **keep the behavior that was documented for Preview**, drop **obsolete "in production" / old-process** branches, then **remove preview-only labels and wrappers** so the topic reads as current for all customers.

### Parallel steps

- If the article has a step (or numbered item) **framed as "in production"** (or equivalent: current production / existing production behavior) **and** a **parallel** step framed as **"in preview"** (or Preview environment):
  - **Remove** the in-production step (the old path).
  - **Keep** the in-preview step's **substance**, but **reword** so it is **not** Preview-specific (remove "in preview," "Preview environment," etc.). Adjust numbering so the list stays consistent.

If structure is ambiguous (no clear parallel), **stop** and show both candidates; ask the user which block to keep.

### Parallel sections

- If a **section** (heading + body) is **about "in the production environment"** and there is a **parallel section** **about "in the preview environment"**:
  - **Remove** the production-environment section (the superseded content).
  - **Replace** with the preview section's content, then **remove** preview-environment wording and any **`class="preview"`** wrappers so the section is neutral (GA-ready).

### Snippets and top-of-article notices

- Remove **preview-only boilerplate** blocks (spans/divs or paragraphs that only explain that highlighted content is Preview-only, fast release, sandbox, etc.) once the feature is GA.
- Remove links or sentences whose **only** purpose is preview availability, unless the user says to keep a different notice.

### HTML `class="preview"`

- Remove the **opening and closing tags** for elements that use **`class="preview"`**, **keeping inner content** (markdown/HTML inside the tag).
- Handle both **`<span class="preview">`** and **`<div class="preview">`**, and the same pattern on other tags (e.g. **`<p class="preview">`**, **`<li class="preview">`**) when they appear in **visible** (non-commented) body content.
- Preserve list/table structure; fix broken lists or stray whitespace after unwrapping.

### Commented-out sections (HTML comments)

- **Do not** delete, unwrap, or otherwise **modify** any content inside **`<!-- … -->`** HTML comments **unless the user explicitly says** what to do (e.g. delete the whole comment, strip preview classes inside the comment only, uncomment for GA).
- If preview-related content or **`class="preview"`** appears **only** inside comments, **call that out** when reviewing the article: say what is in the comment and **ask** what to do. **Default: leave commented sections unchanged.**

### What not to do

- Do not run this workflow on paths under **`product-announcements`** (release notes and related); inventory must exclude them.
- Do not inventory or edit paths listed under **[Excluded paths](#excluded-paths)** unless the user explicitly asks to include one.
- **Do not** automatically remove or edit **commented-out** (`<!-- … -->`) blocks; follow **Commented-out sections** above.
- Do not remove "Preview" when it is **not** about this feature-availability pattern (e.g. [Preview Sandbox environment](·) as a **product name** in unrelated context)—use judgment and ask if unsure.
- Do not change `author:` or unrelated frontmatter unless the user asks.
- Do not skip the **show → approve** step.

## Quality checks before presenting edits

- No remaining **`class="preview"`** on the agreed scope of change.
- No orphaned duplicate headings or broken step numbers.
- Introduction reads correctly **without** contradicting GA (no "only in Preview" for shipped features).

## References

- Match **[Workfront documentation style](https://experienceleague.adobe.com/)** and repo conventions (commit/PR rules if the user is committing).
