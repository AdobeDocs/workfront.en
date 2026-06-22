---
name: writing-quality
description: Review and improve technical writing quality for Workfront how-to articles and general documentation. Applies the Workfront Documentation Style Guide and principles from Developing Quality Technical Information. Use when editing, reviewing, or writing how-to articles, overview articles, reference articles, or general documentation. Do not use for release notes — use the release-notes-formatter skill instead.
---

# Writing Quality

Reviews and improves Workfront documentation using the Workfront Documentation Style Guide and DQTI principles.

## Workflow

When reviewing or editing content:

1. Read the target file
2. Apply the rules below — fix issues directly or flag them
3. Preserve the author's intent and technical accuracy
4. For detailed terminology, punctuation, and procedure rules, see .claude/commands/_writing-quality-reference.md

## Voice & Point of View

- Use **second person** ("You can...") when addressing the reader
- Use contractions for a conversational tone (don't, can't, it's, they're)
- Use "We recommend" for best practices — not "It is recommended" or "You should"
- When writing for one user group, reference other roles in third person ("You can view... However, the Workfront administrator can restrict...")
- Never use gendered pronouns — restructure the sentence or use "they"
- No slash for choices — use "or" ("he or she" not "he/she")

## Clarity (DQTI)

- One idea per sentence
- Keep sentences under ~25 words where possible
- Lead with the action or result, not background context
- Use the simplest word that conveys the meaning ("use" not "utilize", "start" not "initiate", "about" not "regarding")
- Avoid nominalizations ("create" not "the creation of", "configure" not "the configuration of")
- Use specific, concrete language — avoid vague terms ("several", "various", "some")
- Avoid double negatives
- Use optional pronouns ("that", "who") to add clarity to sentence structure

## Concreteness (DQTI)

- Use specific examples instead of abstract descriptions
- Include realistic values in examples
- Name the exact UI elements, fields, and areas

## Task Orientation (DQTI)

- Focus on what the user can *do*, not what the system *is*
- Lead procedures with imperative verbs ("Create a task", "Configure notifications")
- Provide enough context for the user to act, but no more
- Include a link to detailed help ("For more information, see [article].")

## Capitalization

- **Headings**: Sentence case always ("Create a task" not "Create a Task")
- **Workfront terms**: Capitalize only when referencing a UI element directly
  - Direct reference: "Complete the Planned Completion Date field."
  - Indirect reference: "Each task must have a planned completion date."
  - Tip: if you can put "the" or "a" in front of the term, it usually should be lowercase
- **Buttons**: Follow UI capitalization, except all-caps buttons → sentence case
- **Roles**: "System Administrator" for the role in the UI; "Workfront administrator" for the person

## Headings

- Use imperative command in sentence case ("Create a task", "Configure access levels")
- Headings should be task-based — describe what the user will accomplish
- Overview articles end with "overview" ("Projects overview")
- Break long sections into multiple headings with clear subgoals

## Cross-References & Links

Use these exact patterns:

| Situation | Format |
|-----------|--------|
| Link after giving info | "For more information, see [Article name]." |
| Link without prior info | "For information, see [Article name]." |
| Link to a section in another article | "For more information, see [Section name] in [Article name]." |
| Link to a section in the same article | "For more information, see [Section name] in this article." |

- In a paragraph: inline with the text
- In a procedure step: on a new line after the step
- Multiple links: use a bulleted list
- Use "upper-right corner" / "upper-left corner" for screen positions

## Bold & Italics

- **Bold** clickable actions and UI elements within procedure steps only
- Do not bold UI elements outside of procedure steps
- Do not bold dialog box names, page names, icon names, or menu names outside steps
- Use *italics* for text the user should type ("Type *my.workfront.com* in the URL box")
- Never use italics for emphasis — restructure the sentence instead

## Notes, Tips, and Warnings

Use sparingly — overuse makes them invisible to readers.

- Maximum one note/tip/warning per section
- Never stack multiple notes
- Combine related notes into one note with a bulleted list
- Don't use notes to announce new functionality — rework the article text instead

| Type | Purpose |
|------|---------|
| `>[!NOTE]` | Info that doesn't fit the paragraph; avoid frustration; versioning/compatibility |
| `>[!TIP]` | Nice-to-have suggestions that make the user's life easier |
| `>[!IMPORTANT]` | Vital information for the step or procedure |
| `>[!WARNING]` | Alert the user about potential data loss |

## Procedures

- Use imperative command headings ("Create a task")
- Introductions only when necessary — the heading should suffice
- Preferred intro format: infinitive phrase + colon ("To create a temporary password:")
- Single-step procedures still use a numbered list
- Use "type" or "select" — avoid vague words like "set" or "specify"
- Conditional steps: "(Conditional) If you are a member of more than one team, select..."
- Optional steps: "(Optional) To add an emoji, click..."
- Describe the system response before it happens or immediately after
- Multiple methods: document the most straightforward way first, then use "Or"

### Right Angle Brackets in Procedures

- Use `>` to show menu/tab navigation: "Click **Email** > **Notifications**"
- Bold the button names, not the brackets
- Include spaces around brackets
- Don't use brackets for Main Menu navigation — use the main menu snippet

## Punctuation Quick Reference

| Rule | Example |
|------|---------|
| Oxford comma always | "motive, means, and opportunity" |
| Comma before "then" in procedures | "Click Setup, then click Interface." |
| Comma after year in a date mid-sentence | "The January 2, 2016, issue of..." |
| No comma with month-year only | "January 2016" |
| Colon before a list, lowercase after | "Select one of the following: option A" |
| No colon after procedure headings | "Create a task" (not "Create a task:") |
| Em dashes sparingly | Restructure the sentence if possible |
| Periods in file extensions | "Upload a .pdf file" |

For complete punctuation and terminology rules, see .claude/commands/_writing-quality-reference.md.

## Completeness (DQTI)

- Include all information the user needs to understand and act
- Don't include information the user doesn't need
- Always provide a "For more information" link to detailed documentation
- Document system defaults: "(Default)" in lists, or describe in the sentence

## Organization (DQTI)

- Logical structure with progressive disclosure (overview → details → reference)
- Newest content first for time-ordered pages (e.g., release notes)
- One topic per section
- Use lists for 3+ parallel items
- Use tables for structured comparisons or field descriptions
- Avoid wall-of-text paragraphs — break into digestible chunks

## Article Types

| Type | Purpose | Title Convention |
|------|---------|-----------------|
| Overview | Context, diagrams, how things work — no procedures | Ends with "overview" |
| How-to | Specific task with clear steps | Imperative verb |
| Get started | Setup info + links for new users | "Get started with..." |
| Reference | Field descriptions in tables | Descriptive noun phrase |

## Validation Checklist

After editing, verify:

- [ ] Second person throughout ("you"), contractions used
- [ ] Sentence case on all headings
- [ ] Workfront terms capitalized correctly (direct vs. indirect reference)
- [ ] Bold only on clickable actions within procedure steps
- [ ] Cross-references use standard format ("For more information, see...")
- [ ] Notes/tips/warnings not stacked, max one per section
- [ ] Oxford comma used consistently
- [ ] Procedure steps use specific verbs (type, select, click — not "set" or "specify")
- [ ] Conditional/optional steps labeled correctly
- [ ] No gendered pronouns
- [ ] Sentences are clear, concrete, and task-oriented
