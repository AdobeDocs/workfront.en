---
description: Formatting and validation rules for Adobe Workfront release notes (overview, product area, planning, and look-and-feel pages).
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
---

# Release notes formatter

These files are **release notes**, not how-to articles. Do **not** apply the
general writing-quality standards here. Before editing, read the full source of
truth, which includes the templates and the release calendar:

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## Critical rule — determine the doc quarter first

> [!IMPORTANT]
> Never assign a feature to a doc-quarter using calendar-quarter math on its
> Preview or Production date. Doc-quarter is based on which **monthly release**
> the feature ships in, per Workfront's internal release-calendar grouping, which
> is offset from the calendar quarter. For example, a feature with a Production
> date of August 13, 2026 belongs in doc-quarter `26-q4`, not `26-q3`. Always
> cross-check the 2026 Release Calendar table in the reference file before
> creating or editing any file. If a Production date falls outside that table,
> ask for an updated calendar rather than guessing.

## Key structural rules

- **Frontmatter**: `feature` must be exactly `Product Announcements`;
  `recommendations` must be exactly `noDisplay, noCatalog`. Never invent an
  `exl-id` — include it only if one already exists.
- **Newest features first**: the most recent release note is the first H2 after
  the intro (product area pages) and the top row of each feature table (overview
  pages).
- **Overview link**: product-area pages must link to **their own quarter's**
  overview file — a common bug is linking to the previous quarter.
- **Date callout**: each feature H2 is followed by a `>[!NOTE]` block with
  Preview / Production fast release / Production for everyone dates, matching the
  overview table row. Format dates as `Month Day, Year`; use `TBD` if unknown.
- **Written quarter names** in H1s: "First Quarter", "Second Quarter", "Third
  Quarter", "Fourth Quarter".

## Required companion updates when adding pages

- **New page (any)**: add it to `help/quicksilver/TOC.md` in the same change
  (overview first, product-area pages alphabetically, other enhancements last).
- **New quarter's overview page**: also update `help/quicksilver/home.md` —
  refresh the "Latest release" tab link and the planning activity link, and add
  the new quarter to the current-year releases tab.

See the SKILL.md and reference.md files above for the complete templates,
file-naming conventions, link formats, and the full release calendar.
