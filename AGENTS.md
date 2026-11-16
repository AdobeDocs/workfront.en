# AGENTS.md

Agent guidance for the **workfront.en** repository (Adobe Workfront English
documentation). This file points to the canonical instructions so any agent —
regardless of which convention file it reads — follows the same rules.

## Canonical instruction files

- **Repo-wide rules**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
  — candidate-article search, propose-before-edit, commit-message and PR formats,
  and "fill in gaps intelligently."
- **Writing standards** (auto-applies to `help/**/*.md`):
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
  with full detail in
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **Release notes** (auto-applies to `product-announcements/product-releases/**`):
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md).
- **Preview-highlighting cleanup** (on-demand workflow):
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md).

## Non-negotiable behaviors

1. **Find candidate articles before creating new ones.** When new content comes
   in, search `help/` and surface a ranked list of existing articles it might fit,
   then ask where it belongs before drafting.
2. **Propose changes before editing any help `.md` article.** Show the proposed
   diff and wait for explicit approval. The only exception is when I say "just fix
   it" or "don't ask, just edit" in the same turn. Read-only research and in-chat
   drafting are always fine.
3. **Fill in gaps intelligently.** When intent is clear, commit to the
   best-practice answer and match the surrounding article's headings,
   terminology, and structure instead of presenting option menus.
4. **Apply the writing standards proactively** on every `help/` edit — don't wait
   to be reminded.

## Commit and PR conventions

See [.github/copilot-instructions.md](.github/copilot-instructions.md) for the full
commit-message format (imperative subject ≤ ~50 chars; 📖 for additions, ✏️ for
modifications) and PR structure (Jira ID from branch name; `# Summary`,
`# Changes` by file, `# Context` → `## Jira`).
