---
mode: agent
description: Remove Workfront preview-only documentation framing for GA — preview boilerplate snippets, class="preview" HTML, and parallel in-preview vs in-production steps or sections.
---

# Remove preview highlighting

Run this workflow only when I ask to "remove preview highlighting" (or clearly the
same intent). It converts preview-tagged, Courtney-authored how-to/reference
topics into GA-ready content.

## Scope

Apply only when **all** are true:

1. I invoked this workflow.
2. The file path does **not** contain `product-announcements` (exclude the whole
   tree: release notes, betas, announcements).
3. The file is not listed under **Excluded paths** below.
4. The frontmatter `author:` line includes **`Courtney`** (sole or co-author).
5. The article has at least one of:
   - Preview-environment language in body prose or real snippet paragraphs
     ("highlighted information", "Preview environment", "not yet generally
     available", fast-release notes) — **not** a match from link text alone on a
     TOC/index page;
   - Any HTML element with `class="preview"` (`<span>`, `<div>`, `<p>`, `<li>`…);
   - A preview snippet variable such as `{{highlighted-preview}}` or
     `{{highlighted-preview-article-level}}`.

If scope is unclear, confirm before editing.

**TOC / index pages — always skip** when the only preview wording is inside a
markdown link's display text pointing at another article, and the file has no
`class="preview"`, no snippet variables, and no preview boilerplate in prose
outside of links.

### Excluded paths

Never inventory or edit these unless I explicitly override:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md`
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md`

## Required workflow (human in the loop)

Do not bulk-edit without approval.

1. **Inventory** — build a sorted list of in-scope paths (search `help/`). Omit
   `product-announcements`, excluded paths, and TOC/index-only mentions.
2. **Start** — ask whether to begin with the first article (or a path I name).
3. **Per article — show first, edit after OK** — read the file, propose edits as
   before/after excerpts or a focused diff, then wait for explicit approval.
4. **After each file** — ask whether to move to the next (or stop/skip).

## Content rules (preview content becomes the doc)

Goal: keep the behavior documented for Preview, drop obsolete "in production"
branches, then remove preview-only labels and wrappers.

- **Parallel steps**: remove the "in production" step; keep the "in preview"
  step's substance but reword it so it isn't Preview-specific. Fix numbering. If
  no clear parallel, stop and ask which block to keep.
- **Parallel sections**: remove the production-environment section; replace it
  with the preview section's content, then neutralize preview wording and remove
  `class="preview"` wrappers.
- **Snippets and top-of-article notices**: remove preview-only boilerplate and
  sentences whose only purpose is preview availability.
- **`class="preview"`**: remove the opening and closing tags, keep inner content.
  Preserve list/table structure; fix broken lists or stray whitespace.
- **Commented-out sections (`<!-- … -->`)**: do not modify unless I explicitly
  say so. If preview content appears only inside comments, call it out and ask.
  Default: leave comments unchanged.

## Do not

- Run on `product-announcements` paths or excluded paths.
- Auto-edit commented-out blocks.
- Remove "Preview" when it's a product name in unrelated context (e.g. Preview
  Sandbox environment) — ask if unsure.
- Change `author:` or unrelated frontmatter.
- Skip the show → approve step.

## Quality checks before presenting edits

- No remaining `class="preview"` in the agreed scope.
- No orphaned duplicate headings or broken step numbers.
- Introduction reads correctly for GA (no "only in Preview" for shipped features).
