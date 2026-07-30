---
name: add-mini-tocs
description: >-
  Adds mini tables of contents to Markdown documents. For each heading at ##
  level or deeper that has direct subheadings one level deeper, inserts a
  bulleted link list immediately before the first child heading. Only links
  headings at the same child level — does not mix heading depths in the same
  list. Use when the user asks you to add mini TOCs, add subheading lists, or
  add navigation lists to a document.
---

# Add mini TOCs

Scans a Markdown file and inserts a mini table of contents under each qualifying heading that has direct subheadings.

## Workflow

1. Read the target file.
2. Identify every heading at `##` level or deeper that has at least one direct child heading (one `#` level deeper).
3. For each such parent heading, build a bulleted list of links to its direct children only.
4. Insert the list immediately before the first child heading, after any introductory text that follows the parent heading.
5. If a mini TOC already exists in that position, compare it against the current child headings in that section. If the list is out of date (missing entries, extra entries, or incorrect links), replace it with the updated list. If it already matches, skip.
6. Write the updated file.

## Scope

- **Never** create a mini TOC under the `#` article title. Mini TOCs are only added under `##` headings and deeper.
- A `##` heading gets a list of its `###` direct children.
- A `###` heading gets a list of its `####` direct children.
- And so on for deeper levels.

## Link format

Each entry in the list uses this exact format:

```
* [Heading text](#anchor)
```

### Anchor generation rules

Convert the heading text to an anchor as follows:

1. Lowercase all text.
2. Remove any characters that are not letters, numbers, spaces, or hyphens.
3. Replace spaces with hyphens.
4. Remove any backtick-wrapped code formatting (keep the text inside).

Example: `### Create or edit a function` → `#create-or-edit-a-function`

## Nesting rules

- Only link **direct children** (one level deeper than the parent) in each list.
- Do not include grandchildren or deeper headings in the same list.
- If those child headings themselves have children, they get their own separate mini TOC inserted beneath them.

**Example structure:**

```
## Manage a package          ← parent: gets a list of ### headings
### Functions                ← child of ##, parent of ####: gets a list of #### headings
#### Create a function       ← child of ###
#### Delete a function       ← child of ###
### Variables                ← child of ##
### History                  ← child of ##
```

Results in:

Under `## Manage a package`:

```
* [Functions](#functions)
* [Variables](#variables)
* [History](#history)
```

Under `### Functions`:

```
* [Create a function](#create-a-function)
* [Delete a function](#delete-a-function)
```

## Placement

Insert the mini TOC list immediately before the first child heading. If there is introductory text between the parent heading and the first child heading, the list goes after that text, directly above the first child heading. Always include a blank line before and after the mini TOC list.

## What to skip

- `#` headings (the article title): never add a mini TOC here.
- Parent headings with only one direct child: skip — a single-item list adds no navigation value.
- Sections with no child headings: skip.
