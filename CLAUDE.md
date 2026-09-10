# Find candidate articles before creating new ones

When Courtney brings in new content to incorporate — an intake doc, customer or PM feedback, a Slack/transcript paste, screenshots with notes, support questions — **do not propose creating a new article first.** Search the repo and surface candidate existing articles where the content might fit.

## Required workflow

1. **Read the new content first** to identify topic, audience (admin vs end user), and the specific facts/steps it adds.
2. **Search `help/` for candidates** using grep and find. Look for articles that already cover the same feature, area, or workflow.
3. **Return a ranked list** of candidate articles (typically 3–7), each with:
   - The file path (clickable backtick path).
   - A 1-line reason it's a candidate (what section it would slot into, or why it's the closest topical match).
   - Any caveats (e.g., "audience mismatch — this is end-user, intake is admin-facing").
4. **Ask Courtney where to put it** before drafting or editing. Phrase the question explicitly, e.g., "Which of these should I draft into?" or "Want me to fit it into #2, or do you think it needs its own article?"
5. **Only suggest a new article** if no existing article is a reasonable fit, and explain why none of the candidates work.

Even if the content "obviously" belongs in a known article, still surface 2–3 alternatives so Courtney can confirm placement. This catches near-duplicates and places where content was already partially covered.

---

# Propose changes before editing help articles

When about to edit any `.md` help article under `help/`, **do not edit the file yet**. First, show what you plan to change and wait for explicit approval.

For every file you intend to touch:

1. Name the file (path).
2. Show the proposed change as a fenced diff/snippet — old text and new text — with enough surrounding context to be unambiguous.
3. Briefly state the reason (1 sentence).
4. End with an explicit ask, e.g., "Apply these changes?" or "Want me to proceed?"

Only after Courtney says yes (or "go", "apply", "do it", etc.) should you call the editing tools.

This applies to **every** edit on a help `.md` article — typos, link fixes, single-word swaps, terminology cleanups, new sections, and rewrites. No exceptions unless Courtney explicitly says "just fix it" or "don't ask, just edit" in the same turn.

For changes that span multiple articles: group the proposed diffs by file under one reply. If the set is large, list affected files first with a 1-line summary each, then show diffs in batches and confirm before each batch.

This does **not** block read-only research (grep, read) or drafting/exploration in chat (no file writes).

---

# Git commit messages

When drafting or generating a git commit message, follow this format.

## Subject line

- Around **50 characters or fewer**.
- Summarize the change in **imperative mood** (e.g. "Add…", "Fix…", "Refactor…").

## Body

- Leave one blank line after the subject before the body.
- Wrap lines at about **72 characters**.
- Use **bullet lines** for the explanation. Each bullet must start with exactly one of:
  - **📖** — use when the change **adds** something new: new files, new sections, new features, new headers, net-new lines, or other greenfield content.
  - **✏️** — use when the change **modifies** existing work: edits to existing lines, updates to existing sections, refactors, or changes to current content.

Example:
```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

---

# Pull requests (PRs)

## Deriving the Jira issue

- Derive the Jira issue ID from the **current Git branch name** (e.g. a segment matching `FFENT-8796`).
- **If the branch name includes a Jira ID:** Use that ID in the PR title and link it in `# Context` → `## Jira`.
- **If the branch name does not include a Jira ID:** Omit the Jira key from the PR title. Still include `## Jira` with exactly: `No ticket`.

## PR title

**With Jira ID:** `{type}/{JIRA-ID}- {short task description}`
Example: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`

**Without Jira ID:** `{type}- {short task description}`
Example: `docs- Refresh Object Composite API changelog`

### Commit types

- **feat** — adds a new feature
- **fix** — fixes a bug
- **refactor** — rewrites/restructures code without changing behavior
- **perf** — improves performance
- **style** — formatting/whitespace only; no meaning change
- **test** — adds or corrects tests
- **docs** — documentation only, new content added
- **build** — build tools, CI, dependencies, project version
- **ops** — infrastructure, deployment, backup, recovery
- **chore** — miscellaneous (e.g. `.gitignore`)

## PR body — required sections

### `# Summary`
Short overview of what changed and why.

### `# Changes`
Organized by file. For each touched file, use a level-2 heading with the path in backticks, then bullet points.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.
```

### `# Context`
Always include a `## Jira` subsection.

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Or if no ticket: `No ticket`
