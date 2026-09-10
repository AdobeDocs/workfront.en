# Writing Quality Reference

Detailed rules for the `writing-quality` skill. The SKILL.md file covers the most common rules; this file provides the complete reference for punctuation, terminology, capitalization examples, and procedure formatting.

---

## Punctuation

### Periods

- Use periods in a list if the items complete a sentence ("From the X menu, you can:")
- Use periods in a list if any item is a complete sentence
- Periods must not be formatted with the main content (Correct: Click **Done**. / Incorrect: Click **Done.**)
- Use periods in file extensions (.pdf)

### Commas

- Oxford comma always: "motive, means, and opportunity"
- Comma after introductory phrase: "To open a document, click Open."
- Comma after the year in a date mid-sentence: "The January 2, 2016, issue of..."
- Comma before "then" in procedures: "Click **Setup**, then click **Interface**."
- No comma with month-year only: "January 2016"

### Apostrophes

- Use in contractions: don't, they're, it's
- Singular possessive: add 's (Jen's computer)
- Plural possessive ending in s: add only ' (The Joneses' computer)
- Distinguish "it's" (it is) from "its" (belonging to it)

### Colons

- Lowercase after a colon unless followed by a direct quotation, proper noun, or bulleted list
- Use at the end of a sentence/fragment introducing a list
- No colon after procedure headings
- No colon to introduce visual elements or code segments

### Semicolons

- Connect two clauses without a conjunction
- Separate phrases containing their own punctuation
- Don't bold a semicolon following bolded text in procedures
- Don't include in a hyperlink

### Quotation Marks

- Refer to them as "quotation marks" (not "quotes")
- Closing quotation marks go outside commas and periods
- Question mark placement depends on whether the quotation or the sentence is the question

### Hyphens

- Avoid structures requiring hyphens when possible
- Hyphenate compound modifiers before a noun: "read-only memory"
- Hyphenate when one modifier is a participle: "copy-protected disk"
- Hyphenate when one modifier is a number: "12-point font"
- No hyphens in key combinations — use + (Ctrl+I)

### Em Dashes

Use sparingly. Consider restructuring the sentence instead.

### En Dashes

- Ranges: 2005–2013
- Minus sign or negative numbers
- Connect compound adjective to another word: "dialog box–type options"

### Ellipses

- Omitted code or syntax
- UI indication that a dialog box will appear
- Omitted text in quotations (add a period if replacing end of sentence)

### Slash

- No slash for choices — use "or" ("he or she" not "he/she")
- Use for combinations: on/off switch
- Use for internet addresses and fractions

---

## Capitalization Examples

### Workfront Terms — Direct vs. Indirect Reference

| Term | Direct (capitalize) | Indirect (lowercase) |
|------|---------------------|----------------------|
| Planned Completion Date | "Complete the **Planned Completion Date** field." | "Each task must have a planned completion date." |
| Layout Template | "In Setup, go to **Layout Templates**." | "Assign a layout template to each user." |
| Group Administrator | "Locate the **Group Administrator** field." | "Contact your group administrator." |
| Custom Form | "Attach the **Custom Form** to the project." | "You can create a custom form for any object." |

### Common Workfront Terms (capitalize when referencing UI)

- Custom Form
- Duration
- Planned Hours
- Planned Completion Date
- Hour Type
- Group Administrator / System Administrator
- Workfront administrator (the person, always lowercase "administrator")
- Reminder Notifications
- Layout Template
- Filter, View, Grouping (in context of Filters, Views, and Groupings)
- Resource Planner (Plans)

### Buttons

- Follow UI capitalization
- If button is all-caps in UI, write it in sentence case instead

---

## Terminology

### UI Elements

| Element | Correct Term |
|---------|-------------|
| Collapsible list of options | Menu (add "drop-down" for clarity when needed) |
| Unavailable commands | "unavailable" (never "dimmed," "disabled," or "greyed") |
| Popup with form fields | Dialog box |
| Unnamed buttons | Use the button's tooltip name |
| Error messages / toast notifications | "Message" ("A message displays notifying you...") |
| Text input | Field |

### Roles

| Context | Term |
|---------|------|
| The role in Workfront | System Administrator |
| The person who administers Workfront | Workfront administrator |

### Overwrite vs. Override

These are different words with different meanings — use the correct one for the context.

### File Extensions

Always use the file extension, not the acronym: "Upload a .pdf file" (not "Upload a PDF").

---

## Procedure Formatting

### Introductions

Include only when necessary. Preferred formats (in order):

1. Infinitive phrase + colon: "To create a temporary password for a user in your system:"
2. Complete sentence + period: "You must create temporary passwords for users in your system."
3. Infinitive phrase + "follow these steps" + colon: "To create a temporary password for a user, follow these steps:"

### Step Conventions

- Use numbered lists for all procedures, even single-step ones
- Bold clickable actions and UI elements within steps
- Use specific action verbs: "type," "select," "click" — avoid "set" or "specify"
- Describe system responses before they happen or immediately after

Example of system response placement:

```
1. Click **Sharing**.
2. In the **Task Access** dialog box, enter the name of the user you want to give task access to.
```

### Conditional and Optional Steps

```
3. (Conditional) If you are a member of more than one team, select...
3. (Optional) To add an emoji, click...
3. (Conditional and optional) If you want to add a note...
```

### Substeps and Field Lists

Introduce with an imperative command (Configure, Specify, Do), then list fields:

```
1. Specify the following:
   a. **Favorite color**: Select your favorite color from the drop-down menu.
   b. **Favorite song**: Type your favorite song.
```

### Multiple Methods

Document the most straightforward way first:

```
1. In the **Main Menu**, click **Home**.

   Or

   Click the **Home** icon in the upper-left corner.
```

### Right Angle Brackets

- Show menu/tab navigation: "Click **Email** > **Notifications**"
- Bold button names, not brackets
- Spaces around brackets
- Don't use for Main Menu — use the main menu snippet

---

## Bold and Italics Reference

### Bold — Use for:

| Context | In Steps | Outside Steps |
|---------|----------|---------------|
| Clickable buttons/links | Bold | Don't bold |
| Menu names | Bold | Don't bold |
| Icon names | Bold | Don't bold |
| Dialog box names | Bold | Don't bold |
| Page names | Bold | Don't bold |
| Field names in field lists | Bold + colon | Don't bold |

### Italics — Use for:

- Text the user should type: "Type *my.workfront.com* in the URL box"
- Never for emphasis — restructure the sentence instead

---

## Notes, Tips, Warnings — Detailed Guidance

### When to Use Each

**Note** (`>[!NOTE]`):
- Information that doesn't fit the paragraph context
- Avoid user frustration or wasted time ("You must have a team license to complete this task.")
- Versioning or compatibility info ("This functionality is available only in the Legacy Proofing Viewer.")

**Tip** (`>[!TIP]`):
- Suggestions that make the user's life easier but aren't crucial
- Example: "You can share multiple documents at the same time by holding the Shift key."

**Important** (`>[!IMPORTANT]`):
- Vital information for the step or procedure

**Warning** (`>[!WARNING]`):
- Alert the user about potential data loss

### Rules

- One per section maximum
- Never stack multiple notes/tips/warnings
- Combine related notes into one with a bulleted list
- Don't use notes to announce new features — rework the article text

---

## Cross-Reference Patterns

| Situation | Pattern |
|-----------|---------|
| After giving information | "For more information, see [Article name](link)." |
| Without prior information | "For information, see [Article name](link)." |
| To a section in another article | "For more information, see [Section] in [Article name](link)." |
| To a section in the same article | "For more information, see [Section] in this article." |

Placement:
- In paragraphs: inline
- In procedure steps: new line after the step
- Multiple references: bulleted list

---

## DQTI Quality Characteristics

### Easy to Use

| Characteristic | Key Questions |
|---------------|---------------|
| Task orientation | Does this focus on what the user can do? Is the heading an imperative verb? |
| Accuracy | Does terminology match the UI exactly? Are technical details correct? |
| Completeness | Is there enough info to act? Is there unnecessary info to remove? |

### Easy to Understand

| Characteristic | Key Questions |
|---------------|---------------|
| Clarity | Is each sentence one idea? Are words simple and direct? |
| Concreteness | Are there specific examples? Are UI elements named exactly? |
| Style | Active voice? Present tense? Consistent terminology? |

### Easy to Find

| Characteristic | Key Questions |
|---------------|---------------|
| Organization | Logical structure? Progressive disclosure? Newest first where applicable? |
| Retrievability | Can a reader scan headings and understand the content? Are links provided? |
| Visual effectiveness | Lists for 3+ items? Tables for comparisons? No wall-of-text paragraphs? |

---

## Common Fixes

| Issue | Fix |
|-------|-----|
| "We're excited to introduce..." | Remove marketing language — state the feature directly |
| "The configuration of X was updated" | "You can now configure X" (active, task-oriented) |
| "It is recommended that..." | "We recommend..." |
| "Users can utilize the feature to..." | "You can use the feature to..." |
| "set the value" / "specify the option" | "type the value" / "select the option" |
| "disabled" / "greyed out" | "unavailable" |
| "dropdown" (standalone) | "menu" or "drop-down menu" |
| "he/she" | "they" or restructure |
| Stacked notes | Combine into one note with bullets |
| Bold outside procedure steps | Remove bold |
