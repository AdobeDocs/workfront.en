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

   - **Per-section duplication**: Append `in Production` to the existing section heading. Add a new section with `in Preview` appended, wrapped in `<div class="preview"> ... </div>`. Use when the new behavior changes the procedure itself meaningfully — extra or reordered steps, a new image, or different step wording. Typical for how-to procedures.
   - **Per-row duplication**: For a table-based field description where only one row changes and the rest of the table/procedure is unchanged, leave the existing row byte-for-byte unchanged and add a new `<tr class="preview">` directly after it. Do not weave new sentences into the original row. See "Per-row duplication" under Content rules for the exact conventions.
   - **Per-line wrapping**: Add the new sentence(s) inline inside the existing section, wrapped in `<span class="preview"> ... </span>`. Use when the addition is a sentence or two that fits naturally in an existing paragraph or FAQ answer (not a table row — use per-row duplication for those).
   - **Mixed**: Some sections in the same article use different patterns for different content. Surface this option when the article mixes procedural tables, FAQ-style sections, and plain paragraphs.

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

   **When drafting the actual sentences** for either bucket, apply `~/.cursor/skills/writing-quality/SKILL.md` voice and tone rules as you write — a plain field/behavior description, not a changelog entry ("has been removed," "has been added"), and don't restate an unchanged instruction just to attach a preview note to it. Draft it right the first time rather than fixing tone in a later pass.

5. **Do a final writing-quality pass** on the drafted text before showing it. This is a safety net, not the first time these rules apply — catch anything step 4 missed (redundancy, tone, voice mismatch with surrounding rows).

6. **Propose edits.** Show before/after excerpts (or a focused diff-style description) for the article, covering: snippet placement, heading renames, new in-Preview content and where it sits, screenshot reference, and any inline `class="preview"` wraps.

7. **Wait for explicit approval** ("okay", "apply", "yes") before writing the file.

8. **Validate.** After writing, run `ReadLints` on the file and report any issues. Re-read the changed section to confirm structure.

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

### Per-row duplication

For a table-based field description where only the field's *behavior* changes (not the surrounding procedure):

- Leave the existing `<tr>` completely unchanged — it now stands for the current/production behavior. Never splice new sentences or spans into it.
- Add a new row directly after it:

  ```html
  <tr class="preview">
  <td><span class="preview"><strong>{new label} in preview</strong></span></td>
  <td><span class="preview">{self-contained description}</span></td>
  </tr>
  ```

- **Label**: don't just take the original field label and append `(in Preview)`. Write a short, natural label for the new capability itself (e.g., original label "Add names or emails" → new label "Add people or teams"), then append lowercase `in preview` with no parentheses: "Add people or teams in preview".
- **Description**: write a fresh 1–3 sentence description of only the new behavior, in the article's existing voice. Don't reuse the original row's sentences as a base and insert additions into them — the new row must read as a complete, standalone description on its own.
- **Supplementary notes**: append with a `<br>` line break followed by `Note:` on the next line, inside the same `<span class="preview">` — don't nest a `<p>Note: ...</p>`. Because the new row stands alone, restate any still-relevant fact from the original row's note briefly here rather than assuming the reader also saw it (e.g., an Advanced-mode "one open stage at a time" restriction that applies equally to the new row).
- **Multiple variants**: if the same field is being updated in more than one procedure in the same article (Basic vs. Advanced, legacy vs. ESM, and so on) and the underlying behavior actually differs between them (e.g., legacy keeps an opt-in default while ESM always expands), write each row to match that variant's real behavior. Don't copy one variant's wording into another's row.

### Snippet placement

- Snippet line goes immediately after the H1, with a blank line above and below.
- Snippet sits **before** the intro paragraph, the `>[!IMPORTANT]` callout, and any access-requirements block.
- One snippet per article.

### Screenshots

- Save new screenshots to the article's `assets/` folder with a descriptive kebab-case filename.
- Reference the new screenshot from within the new in-Preview section. If an in-Production section's screenshot no longer reflects the feature accurately, leave it in place — it still represents production behavior until GA.
- Don't fabricate screenshot filenames; if no screenshot has been provided yet, ask the user.
- **Placeholder for a screenshot that doesn't exist yet**: if the user wants to proceed without waiting for the asset, add an HTML comment directly after the existing (production) screenshot reference, reusing that filename with a `-v2` suffix:

  ```html
  <!--
  preview screen![{same alt text}](assets/{existing-filename}-v2.png)
  -->
  ```

  Swap in the real reference (and uncomment) once the screenshot is provided.

### Notes and tips

- Maximum one `>[!NOTE]` (or `>[!TIP]`, `>[!IMPORTANT]`, `>[!WARNING]`) per section. If the existing section already has a note, combine related new content into the same note as a bulleted list rather than stacking.

### What not to do

- Do not edit articles under `product-announcements/`.
- Do not bulk-edit; one article at a time, with explicit approval each time.
- Do not include observable-UI facts without surfacing them to the user first.
- Do not modify content inside `<!-- ... -->` HTML comments unless the user explicitly says to.
- Do not change `author:` or unrelated frontmatter fields.

## Quality checks before presenting edits

Run this full checklist for **every** article in the session — including secondary articles where you're "just adding a bullet," not only the first/primary one.

- Snippet appears once, on its own line, after the H1, with blank lines above and below.
- Existing section headings end with `in Production`.
- New section headings end with `in Preview` and the section is inside `<div class="preview">`.
- Inline additions are inside `<span class="preview">`.
- Per-row duplications: the original `<tr>` is byte-for-byte unchanged; the new `<tr class="preview">` has both cells wrapped in `<span class="preview">`; the label is a fresh short label + lowercase "in preview" (not the original label + "(in Preview)"); any supplementary note uses `<br>` + `Note:` inline, not a nested `<p>`.
- If the same field appears in more than one procedure variant (Basic/Advanced, legacy/ESM), each new row's wording matches that variant's actual behavior rather than being copy-pasted from another variant.
- New preview-marked prose reads like a plain field/behavior description, not a changelog entry, and doesn't redundantly restate an unchanged instruction.
- `ReadLints` is clean on the edited file.
- The article reads correctly in both states (with the preview content shown and hidden).

## References

- Workfront documentation style: see the **writing-quality** skill at `~/.cursor/skills/writing-quality/SKILL.md`.
- Snippet catalog: `help/_includes/snippets.md` in the docs repo.
- GA cleanup (inverse workflow): see the **remove-preview-highlighting** skill at `.cursor/skills/remove-preview-highlighting/SKILL.md`.
- Adobe Wiki MCP for PRDs: server `user-Adobe Wiki Confluence`, tool `get_wiki_content`.
