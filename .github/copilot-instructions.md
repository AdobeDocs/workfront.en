# Copilot instructions for workfront.en

This repository contains the Adobe Workfront English documentation. The rules
below apply to every request in this workspace. Topic-specific standards live in
`.github/instructions/*.instructions.md` and load automatically when you edit
matching files.

## Find candidate articles before creating new ones

When new content comes in — an intake doc, customer or PM feedback, a
Slack/transcript paste, screenshots with notes, or support questions — **do not
propose creating a new article first.** Search the repo and surface candidate
existing articles where the content might fit.

Required workflow:

1. **Read the new content first** to identify topic, audience (admin vs. end
   user), and the specific facts or steps it adds.
2. **Search `help/` for candidates** using grep and file search. Look for
   articles that already cover the same feature, area, or workflow.
3. **Return a ranked list** of candidate articles (typically 3–7), each with:
   - The file path (as a clickable link).
   - A one-line reason it's a candidate (what section it would slot into, or why
     it's the closest topical match).
   - Any caveats (for example, "audience mismatch — this is end-user, intake is
     admin-facing").
4. **Ask where to put it** before drafting or editing. Phrase the question
   explicitly, for example "Which of these should I draft into?" or "Want me to
   fit it into #2, or do you think it needs its own article?"
5. **Only suggest a new article** if no existing article is a reasonable fit, and
   explain why none of the candidates work.

Even if the content "obviously" belongs in a known article, still surface 2–3
alternatives so placement can be confirmed. This catches near-duplicates and
places where content was already partially covered.

## Propose changes before editing help articles

When about to edit any `.md` help article under `help/`, **do not edit the file
yet.** First, show what you plan to change and wait for explicit approval.

For every file you intend to touch:

1. Name the file (path).
2. Show the proposed change as a fenced diff/snippet — old text and new text —
   with enough surrounding context to be unambiguous.
3. Briefly state the reason (one sentence).
4. End with an explicit ask, for example "Apply these changes?" or "Want me to
   proceed?"

Only after explicit approval ("yes", "go", "apply", "do it", etc.) should you
call the editing tools.

This applies to **every** edit on a help `.md` article — typos, link fixes,
single-word swaps, terminology cleanups, new sections, and rewrites. No
exceptions unless the user explicitly says "just fix it" or "don't ask, just
edit" in the same turn.

For changes that span multiple articles, group the proposed diffs by file under
one reply. If the set is large, list affected files first with a one-line summary
each, then show diffs in batches and confirm before each batch.

This does **not** block read-only research (grep, read) or drafting/exploration
in chat (no file writes).

## Fill in gaps intelligently

When intent is clear from context, commit to the best-practice answer rather than
presenting option menus. Apply the writing standards (see
`.github/instructions/writing-quality.instructions.md`) proactively — do not wait
to be reminded to follow them. Match new text to the surrounding article's
headings, terminology, and structure. Only ask when a genuine ambiguity would
change the outcome.

## Git commit messages

### Subject line

- Around **50 characters or fewer**.
- Summarize the change in **imperative mood** ("Add…", "Fix…", "Refactor…").

### Body

- Leave one blank line after the subject before the body.
- Wrap lines at about **72 characters**.
- Use **bullet lines** for the explanation. Each bullet must start with exactly
  one of:
  - **📖** — when the change **adds** something new: new files, new sections, new
    features, new headers, net-new lines, or other greenfield content.
  - **✏️** — when the change **modifies** existing work: edits to existing lines,
    updates to existing sections, refactors, or changes to current content.

Example:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

## Pull requests

### Deriving the Jira issue

- Derive the Jira issue ID from the **current Git branch name** (for example a
  segment matching `FFENT-8796`).
- **If the branch name includes a Jira ID:** use that ID in the PR title and link
  it in `# Context` → `## Jira`.
- **If the branch name does not include a Jira ID:** omit the Jira key from the PR
  title. Still include `## Jira` with exactly `No ticket`.

### PR title

- **With Jira ID:** `{type}/{JIRA-ID}- {short task description}`
  - Example: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`
- **Without Jira ID:** `{type}- {short task description}`
  - Example: `docs- Refresh Object Composite API changelog`

Commit types: **feat** (new feature), **fix** (bug fix), **refactor** (restructure
without behavior change), **perf** (performance), **style** (formatting only),
**test** (tests), **docs** (documentation only, new content), **build** (build/CI/
dependencies), **ops** (infrastructure/deployment), **chore** (miscellaneous).

### PR body — required sections

- `# Summary` — short overview of what changed and why.
- `# Changes` — organized by file. For each touched file, use a level-2 heading
  with the path in backticks, then bullet points.
- `# Context` — always include a `## Jira` subsection with the linked issue, or
  `No ticket`.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```
