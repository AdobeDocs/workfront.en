---
description: Workfront technical writing standards for help articles. Applies the Workfront Documentation Style Guide and Developing Quality Technical Information (DQTI) principles.
applyTo: "help/**/*.md"
---

# Writing quality

Apply these standards whenever editing, reviewing, or writing a help article.
Preserve the author's intent and technical accuracy. For the complete
punctuation, terminology, capitalization, and procedure reference, read
[.cursor/skills/writing-quality/reference.md](../../.cursor/skills/writing-quality/reference.md).

Do **not** apply these rules to release notes under
`help/quicksilver/product-announcements/product-releases/` — use the
release-notes-formatter instructions instead.

## Voice and point of view

- Use **second person** ("You can...") when addressing the reader.
- Use contractions for a conversational tone (don't, can't, it's, they're).
- Use "We recommend" for best practices — not "It is recommended" or "You should".
- When writing for one user group, reference other roles in third person.
- Never use gendered pronouns — restructure the sentence or use "they".
- No slash for choices — use "or" ("he or she" not "he/she").

## Clarity (DQTI)

- One idea per sentence; keep sentences under ~25 words where possible.
- Lead with the action or result, not background context.
- Use the simplest word ("use" not "utilize", "start" not "initiate").
- Avoid nominalizations ("create" not "the creation of").
- Use specific, concrete language — avoid vague terms ("several", "various").
- Avoid double negatives.

## Concreteness and task orientation (DQTI)

- Use specific examples with realistic values; name exact UI elements and fields.
- Focus on what the user can *do*, not what the system *is*.
- Lead procedures with imperative verbs ("Create a task", "Configure notifications").
- Provide enough context to act, but no more.
- Include a link to detailed help ("For more information, see [article].").

## Capitalization

- **Headings**: sentence case always ("Create a task", not "Create a Task").
- **Workfront terms**: capitalize only when referencing a UI element directly.
  - Direct: "Complete the Planned Completion Date field."
  - Indirect: "Each task must have a planned completion date."
  - Tip: if you can put "the" or "a" in front of the term, it's usually lowercase.
- **Buttons**: follow UI capitalization; all-caps buttons become sentence case.
- **Roles**: "System Administrator" for the role in the UI; "Workfront
  administrator" for the person.

## Headings

- Imperative command in sentence case, task-based ("Configure access levels").
- Overview articles end with "overview" ("Projects overview").
- Break long sections into multiple headings with clear subgoals.

## Cross-references and links

| Situation | Format |
|-----------|--------|
| Link after giving info | "For more information, see [Article name]." |
| Link without prior info | "For information, see [Article name]." |
| Link to a section in another article | "For more information, see [Section name] in [Article name]." |
| Link to a section in the same article | "For more information, see [Section name] in this article." |

- In a paragraph: inline. In a procedure step: on a new line after the step.
- Multiple links: use a bulleted list.
- Use "upper-right corner" / "upper-left corner" for screen positions.

## Bold and italics

- **Bold** clickable actions and UI elements **within procedure steps only**.
- Do not bold UI elements, dialog box names, page names, icon names, or menu
  names outside of procedure steps.
- Use *italics* for text the user should type ("Type *my.workfront.com*...").
- Never use italics for emphasis — restructure the sentence instead.

## Notes, tips, and warnings

Use sparingly — overuse makes them invisible.

- Maximum one note/tip/warning per section; never stack them.
- Combine related notes into one note with a bulleted list.
- Don't use notes to announce new functionality — rework the article text instead.

| Type | Purpose |
|------|---------|
| `>[!NOTE]` | Info that doesn't fit the paragraph; versioning/compatibility |
| `>[!TIP]` | Nice-to-have suggestions that make the user's life easier |
| `>[!IMPORTANT]` | Vital information for the step or procedure |
| `>[!WARNING]` | Alert the user about potential data loss |

## Procedures

- Use imperative command headings; introductions only when necessary.
- Preferred intro format: infinitive phrase + colon ("To create a temporary
  password:").
- Single-step procedures still use a numbered list.
- Use "type" or "select" — avoid vague words like "set" or "specify".
- Conditional steps: "(Conditional) If you are a member of more than one team,
  select...". Optional steps: "(Optional) To add an emoji, click...".
- Describe the system response before it happens or immediately after.
- Multiple methods: document the most straightforward way first, then use "Or".
- Menu/tab navigation: "Click **Email** > **Notifications**" (bold the names, not
  the brackets; spaces around brackets). Don't use brackets for Main Menu
  navigation — use the main menu snippet.

## Punctuation quick reference

| Rule | Example |
|------|---------|
| Oxford comma always | "motive, means, and opportunity" |
| Comma before "then" in procedures | "Click Setup, then click Interface." |
| Comma after year in a date mid-sentence | "The January 2, 2016, issue of..." |
| No comma with month-year only | "January 2016" |
| Colon before a list, lowercase after | "Select one of the following: option A" |
| No colon after procedure headings | "Create a task" |
| Em dashes sparingly | Restructure the sentence if possible |
| Periods in file extensions | "Upload a .pdf file" |

## Organization (DQTI)

- Logical structure with progressive disclosure (overview → details → reference).
- One topic per section; use lists for 3+ parallel items.
- Keep list items and their lead-in grammatically parallel.
- Use tables for structured comparisons or field descriptions.
- Avoid wall-of-text paragraphs — break into digestible chunks.

## Validation checklist

- [ ] Second person throughout, contractions used.
- [ ] Sentence case on all headings.
- [ ] Workfront terms capitalized correctly (direct vs. indirect reference).
- [ ] Bold only on clickable actions within procedure steps.
- [ ] Cross-references use the standard format.
- [ ] Notes/tips/warnings not stacked, max one per section.
- [ ] Oxford comma used consistently.
- [ ] Procedure steps use specific verbs (type, select, click).
- [ ] Conditional/optional steps labeled correctly.
- [ ] No gendered pronouns.
- [ ] Sentences are clear, concrete, and task-oriented; parallel structure holds.
