---
description: Curate new NovaSaga raw notes into the active lore-record wiki.
---

Use the repo-local `novasaga-lore-curator` skill:

`.agents/skills/novasaga-lore-curator/SKILL.md`

Then run one curation pass on NovaSaga's active wiki.

Scope:

- Pull latest `origin/main` first.
- Inspect new or recently changed notes under `raw/`.
- Curate into existing active wiki pages before creating new pages.
- Do not rewrite `drafts/`.
- Do not delete or bulk-restore `archive/`.
- Keep archive/raw as source evidence.
- Use lore-record tone: `Known`, `Suspected`, `Disputed`, `Unresolved`.
- Avoid project-note phrasing such as "the story should" or "NovaSaga is about".
- Use orchestration when useful: a read-only explorer/checker sub-agent may inspect raw notes and recommend target pages while the main agent owns edits.
- Commit on `main` and push to `origin/main` when done, unless explicitly told to keep changes local.

Arguments or focus from user:

`$ARGUMENTS`
