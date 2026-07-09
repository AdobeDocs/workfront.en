---
name: update-for-release
description: >-
  Document a new Workfront feature for an upcoming release: identify affected
  help articles, choose the right preview snippet, mark new content with
  preview highlighting (per-section or per-line as appropriate per article),
  and surface borderline UI-level details as explicit approve/reject prompts
  before applying edits. Use when the user is updating Workfront help articles
  for a feature that is shipping (typically Preview first), mentions a PRD or
  upcoming release, asks about preview highlighting, or wants help adding
  "in Preview" / "in Production" sections to how-to or overview articles.
---

# Update for release (Workfront)

This skill walks through updating Workfront help articles for an upcoming feature release. The workflow is the inverse of `remove-preview-highlighting`: new behavior is being added to articles, marked as Preview, and (later, at GA) cleaned up by that other skill.

## Scope

Apply when **all** are true:

1. The user is updating Workfront help articles for a feature that is shipping (typically Preview first).
2. The change introduces new behavior or UI, not a GA cleanup. For GA cleanup, use **remove-preview-highlighting** instead.
3. The file is **not** a release note. For release notes, use **release-notes-formatter** instead.
4. The user has given feature context: at minimum a short description and a screenshot; ideally a PRD URL (Adobe Wiki).

If scope is unclear, confirm before starting.

## Required workflow (human in the loop)

Do **not** bulk-edit the repo. Move one article at a time. After each article, ask whether to continue to the next.

### 1. Gather feature context

Confirm with the user:

- **What changed** (1-2 sentence summary of the new behavior or UI).
- **Screenshot(s)** of the new UI. If provided, save under the target article's `assets/` folder with a descriptive kebab-case filename (e.g. `add-custom-message.png`). If not provided, ask whether to wait for one or proceed with a placeholder reference.
- **PRD URL** (Adobe Wiki), if available. Fetch it with the `user-Adobe Wiki Confluence` MCP tool `get_wiki_content`. Read it to find behavior the user can't see in the UI: notification side effects, what happens when something is edited or added later, character limits not displayed, permissions, etc.
- **Availability**: Preview-only, Preview + fast release, or already GA. This drives the snippet choice in step 3.
- **Explicit exclusions**: any articles the user wants to skip (e.g. "this feature is not in templates").

### 2. Inventory affected articles

Search the repo with the feature area's keywords (e.g. `approval workflow`, `document approval`, the specific field label). Build a candidate list:

- How-to articles in the relevant `help/quicksilver/.../` tree.
- Overview articles and FAQs that mention the feature area.
- **Exclude** `product-announcements/` (release notes use a different skill).
- **Exclude** TOC/index pages where the only mention is link text to another article.
- **Exclude** articles the user said to skip in step 1.

Present the candidate list to the user. Ask which to update and which to skip. Cross-reference `help/quicksilver/TOC.md` if a sibling article seems missing.

### 3. Pick the preview snippet

Read `help/_includes/snippets.md` and choose by availability:

| Availability | Snippet |
| --- | --- |
| Preview only — highlighted content is new in an otherwise-GA article | `{{highlighted-preview}}` |
| Preview only — the whole article is new | `{{highlighted-preview-article-level}}` |
| Preview + fast release customers, general | `{{preview-fast-release-general}}` |

If a release-specific snippet already exists for the current quarter, prefer that over the generic one. Confirm the choice with the user before applying.

### 4. Per article — show first, edit after OK

For each article in the user-confirmed list:

1. **Read the file.**

2. **Determine the highlighting pattern.** Ask the user which fits this article (the answer can differ per article):

   - **Per-section duplication**: Append `in Production` to the existing section heading. Add a new section with `in Preview` appended, wrapped in `<div class="preview"> ... </div>`. Use when the new behavior changes the procedure meaningfully — extra steps, a new image, new table rows, or different wording. Typical for how-to procedures.
   - **Per-line wrapping**: Add the new sentence(s) inline inside the existing section, wrapped in `<span class="preview"> ... </span>`. Use when the addition is a sentence or two that fits naturally in an existing paragraph, table cell, or FAQ answer.
   - **Mixed**: Some sections in the same article use per-section duplication, others use per-line wrapping. Surface this option when the article has both procedural sections and FAQ-style sections.

3. **Place the snippet** on its own line immediately after the H1 heading, with a blank line above and below. The snippet sits **before** the intro paragraph.

4. **Bucket new details into "always include" vs. "up for review".** This is the most important step.

   - **Always include** (apply automatically, no prompt): invisible behaviors the user can't observe while interacting with the UI. Examples:
     - Side effects (e.g. "editing this resends the email to all participants")
     - Behavior across other objects or later events
     - Prerequisites and permissions
     - Limits not shown in the UI
     - Anything the user can only learn from the PRD, docs, or product team
   - **Up for review** (present to user with `AskQuestion` as a multi-select): facts the user can see on screen while using the feature. Examples:
     - A character counter the UI already shows (e.g. `0 / 500`)
     - A field's default expanded/collapsed state
     - Default selected state of a visible checkbox
     - Button labels next to the field
     - Validation messages that appear inline

   For each "up for review" item, provide a one-sentence rationale ("Helps novices plan a longer message," "Helps users who don't see it on later stages know to expand it"). Include only the items the user picks. The default principle is "if the user can see it on screen as they're doing the task, don't restate it" — but the user gets the final call.

5. **Propose edits.** Show before/after excerpts (or a focused diff-style description) for the article, covering: snippet placement, heading renames, new in-Preview content and where it sits, screenshot reference, and any inline `class="preview"` wraps.

6. **Wait for explicit approval** ("okay", "apply", "yes") before writing the file.

7. **Validate.** After writing, run `ReadLints` on the file and report any issues. Re-read the changed section to confirm structure.

8. **Defer prose-level edits** to the **writing-quality** skill. Don't redo voice, capitalization, bold rules, or link patterns here — read `~/.cursor/skills/writing-quality/SKILL.md` if a prose pass is requested.

### 5. After each article

Ask whether to move to the next article, stop, skip, or revisit the current one.

### 6. End of session — copy/paste release note

When the user wraps up for the session (says "done," "that's it," "stop," or declines to continue to the next article), ask:

> "Want a copy/paste release note entry for the enhancement page?"

If yes, generate a draft entry using the feature context from step 1 and the primary help article updated in this session. **Do not write it to any file** — provide it as copy/paste text only.

Format the entry to match the product area page structure from the **release-notes-formatter** skill:

```markdown
## {Feature name}

>[!NOTE]
>
>Preview: {date or TBD}
>Production fast release: {date or TBD}
>Production for everyone: {date or TBD}

{1–3 sentences describing what changed and why it helps users. Lead with the benefit, not the UI action.}

For more information, see [{Primary article title}](/help/quicksilver/{path-to-article}.md).
```

Rules:

- Use `TBD` for any date not yet known; ask the user if they have the dates.
- Feature name is sentence case (capitalize only the first word and proper nouns).
- Description should focus on what users can now do, not the implementation detail.
- Link to the most specific how-to article updated, not an overview page.
- Do not include a `>[!NOTE]` date block if all dates are unknown and the user does not want placeholders — omit it and note it needs to be added later.

## Content rules

### Headings

- Append exactly **`in Production`** to existing section headings that stay as the production-side reference.
- Append exactly **`in Preview`** to new section headings.
- Keep the rest of the heading in sentence case (per `writing-quality`).

### Preview wrappers

- **Section-level**: wrap in `<div class="preview"> ... </div>`. Place opening and closing tags on their own lines, with a blank line above and below each tag, so markdown headings and lists inside still render.
- **Inline (sentence-level)**: wrap in `<span class="preview"> ... </span>` inside the existing paragraph, table cell, or FAQ answer.
- Never nest a `<span class="preview">` inside a `<div class="preview">`.

### Snippet placement

- Snippet line goes immediately after the H1, with a blank line above and below.
- Snippet sits **before** the intro paragraph, the `>[!IMPORTANT]` callout, and any access-requirements block.
- One snippet per article.

### Screenshots

- Save new screenshots to the article's `assets/` folder with a descriptive kebab-case filename.
- Reference the new screenshot from within the new in-Preview section. If an in-Production section's screenshot no longer reflects the feature accurately, leave it in place — it still represents production behavior until GA.
- Don't fabricate screenshot filenames; if no screenshot has been provided yet, ask the user.

### Notes and tips

- Maximum one `>[!NOTE]` (or `>[!TIP]`, `>[!IMPORTANT]`, `>[!WARNING]`) per section. If the existing section already has a note, combine related new content into the same note as a bulleted list rather than stacking.

### What not to do

- Do not edit articles under `product-announcements/`.
- Do not bulk-edit; one article at a time, with explicit approval each time.
- Do not include observable-UI facts without surfacing them to the user first.
- Do not modify content inside `<!-- ... -->` HTML comments unless the user explicitly says to.
- Do not change `author:` or unrelated frontmatter fields.

## Quality checks before presenting edits

- Snippet appears once, on its own line, after the H1, with blank lines above and below.
- Existing section headings end with `in Production`.
- New section headings end with `in Preview` and the section is inside `<div class="preview">`.
- Inline additions are inside `<span class="preview">`.
- `ReadLints` is clean on the edited file.
- The article reads correctly in both states (with the preview content shown and hidden).

## References

- Workfront documentation style: see the **writing-quality** skill at `~/.cursor/skills/writing-quality/SKILL.md`.
- Snippet catalog: `help/_includes/snippets.md` in the docs repo.
- GA cleanup (inverse workflow): see the **remove-preview-highlighting** skill at `.cursor/skills/remove-preview-highlighting/SKILL.md`.
- Adobe Wiki MCP for PRDs: server `user-Adobe Wiki Confluence`, tool `get_wiki_content`.
