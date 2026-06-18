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
| **Overview** | `{YY}-q{N}-release-overview.md` | See .claude/commands/_release-notes-formatter-reference.md#overview-page-template |
| **Product Area** | `{YY}-q{N}-{area}.md` | See .claude/commands/_release-notes-formatter-reference.md#product-area-page-template |
| **Planning** | `planning-release-activity-{YY}-q{N}.md` | Similar to product area |
| **Look and Feel** | `look-and-feel-updates-{YY}-q{N}.md` | See .claude/commands/_release-notes-formatter-reference.md#look-and-feel-page-template |

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

5. **H3 per product area** with HTML feature table (see .claude/commands/_release-notes-formatter-reference.md#overview-feature-table)
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

## File Naming Conventions

| Type | Pattern | Example |
|------|---------|---------|
| Overview | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Product area | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Directory | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Standard area slugs: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Quarter Mapping

| Quarter | Written Form | Months |
|---------|-------------|--------|
| Q1 | First Quarter | Jan–Mar |
| Q2 | Second Quarter | Apr–Jun |
| Q3 | Third Quarter | Jul–Sep |
| Q4 | Fourth Quarter | Oct–Dec |

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

## Additional Resources

- For complete HTML templates and examples, see .claude/commands/_release-notes-formatter-reference.md
