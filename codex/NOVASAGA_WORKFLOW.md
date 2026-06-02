# NovaSaga Workflow

## Purpose

This file defines how Codex agents should work inside NovaSaga during the clean restart.

## Start Here

1. Read root `AGENTS.md`.
2. For lore, canon, raw-note, archive, or wiki work, read `.agents/skills/novasaga-lore-curator/SKILL.md`.
3. Read `meta/CanonPolicy.md`.
4. Read `wiki/Home.md` before editing any other wiki page.

## Slash Prompt

When the current Codex client supports repo-local prompts, use:

```text
/novasaga-curate
```

The wrapper lives at `.codex/prompts/novasaga-curate.md` and delegates to the `novasaga-lore-curator` skill. If it does not appear in a session, use:

```text
/use novasaga-lore-curator
```

or explicitly ask Codex to use the skill.

## Operating Model

NovaSaga uses a project-specific LLM wiki workflow adapted from PTI's raw-to-wiki model:

```text
discussion or archive source -> raw note -> lore-curator pass -> compact linked wiki -> better writing/review prompts -> reviewed updates back into wiki
```

The active wiki should help agents reason about story direction. It should not preserve every old idea. The archive already preserves the pre-restart state.

## Raw-To-Wiki Flow

1. Add rough source material to `raw/` as a dated note when it comes from chat, review, archive synthesis, or user discussion.
2. Use the lore-curator skill to identify durable concepts.
3. Update existing wiki pages first.
4. Create new wiki pages only when an idea is stable and recurring.
5. Label continuity status as `Canon`, `Provisional`, `Candidate`, `Open question`, or `Deprecated`.
6. Use inline wiki-style links inside natural sentences.
7. Add source notes pointing back to `raw/` or archive files.
8. Keep technical/Codex details in `codex/`, not the creative wiki.

## Do Not

- Do not rewrite prose drafts unless the user asks.
- Do not delete archive material.
- Do not bulk-copy legacy files into active wiki.
- Do not treat legacy generated content as final truth.
- Do not create many empty pages just because a folder exists.
- Do not create `README.md` category nodes inside `wiki/`; use readable note names like `World.md` and `Characters.md` so Obsidian graph labels stay useful.

## Preferred Output For Wiki Tasks

When a wiki task completes, report:

- source material inspected;
- wiki pages changed;
- canon/provisional/open-question changes;
- raw notes added;
- what needs human or checker review next.

## Sync Rule

The user reads NovaSaga on mobile through Git sync and Obsidian. When a Codex run updates `wiki/`, `raw/`, `skills/`, `.agents/skills/`, `meta/`, or `codex/` for the active workflow, commit the completed change on `main` and push to `origin/main` unless the user explicitly asks to keep changes local.
