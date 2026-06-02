# NovaSaga Agent Instructions

## Project Identity

NovaSaga is a first-class novel-writing and worldbuilding workspace at `F:\Workspace\NovaSaga`.

The active wiki is a compact, interlinked knowledge graph for story thinking. It is not a dumping ground for old notes, draft prose, GitHub setup details, or product planning.

## Required Local Skill

For lore, canon, wiki, raw-note, or worldbuilding curation tasks, use the repo-local skill:

`F:\Workspace\NovaSaga\.agents\skills\novasaga-lore-curator\SKILL.md`

If the current Codex runtime does not auto-discover repo-local skills, open that file manually before editing `wiki/`.

## Repository Roles

- `wiki/` contains refined, linked story knowledge: canon, provisional ideas, unresolved questions, themes, world rules, characters, factions, events, cosmology, and artifacts.
- `raw/` contains source notes, summaries, imports, and rough thinking. Raw notes are source material, not final wiki pages.
- `archive/legacy-before-restart-2026-06-02/` preserves pre-restart material. Do not delete it and do not blindly restore it into active wiki.
- `drafts/` contains prose drafts. Do not rewrite prose drafts unless the user explicitly asks.
- `meta/` contains canon, tone, and restart policy.
- `codex/` contains agent workflow instructions.
- `.agents/skills/` contains Codex-discoverable local skills.
- `skills/` contains project skill documentation and mirrors for humans or tools that do not scan `.agents`.

## Working Rules

- Check `git status` before editing.
- Preserve uncertainty. Do not convert guesses into canon.
- Prefer improving existing durable pages over creating many tiny pages.
- Use inline wiki-style links inside natural sentences where they help reasoning.
- Keep technical, GitHub, and Codex setup details out of the creative wiki except when a wiki source note needs attribution.
- Keep archive references in `Source notes` sections or raw notes; do not paste large legacy sections into active wiki.
- Inside `wiki/`, prefer readable file names over `README.md` index files so Obsidian graph view remains usable on mobile.
- For wiki, raw-note, skill, or workflow updates intended for the user's mobile Obsidian sync, commit on `main` and push to `origin/main` unless the user explicitly asks to leave changes local.
