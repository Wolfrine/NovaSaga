---
name: novasaga-lore-curator
description: Curate NovaSaga raw notes and archived lore into a compact, linked novel-writing wiki while preserving canon status, uncertainty, source references, and authorial intent.
---

# NovaSaga Lore Curator

Use this skill when updating NovaSaga's active `wiki/`, processing `raw/` notes, or selectively curating material from `archive/legacy-before-restart-2026-06-02/`.

## Core Purpose

Maintain the active wiki as an agent-readable story knowledge graph. The wiki should help future writing and review agents understand current direction, accepted facts, provisional ideas, unresolved questions, tone, and continuity boundaries without needing chat history.

## Repository Roles

- `wiki/`: refined story knowledge only.
- `raw/`: source notes and rough inputs. Treat raw notes as evidence, not final pages.
- `archive/legacy-before-restart-2026-06-02/`: preserved pre-restart material. Use selectively.
- `drafts/`: prose drafts. Do not rewrite unless explicitly asked.
- `meta/`: canon and style policy.
- `codex/`: execution workflow for agents.

## Canon Status Labels

Use these labels whenever a claim could affect continuity:

- `Canon`: accepted for now unless the user changes it.
- `Provisional`: likely useful but still open to reshaping.
- `Candidate`: interesting legacy idea not yet adopted.
- `Open question`: unresolved decision or contradiction.
- `Deprecated`: preserved for history but should not guide new work.

If a source is unclear, mark the idea `Candidate` or `Open question`; do not upgrade it to `Canon`.

## Raw-To-Wiki Workflow

1. Read the raw note or archive source fully enough to understand context.
2. Identify durable story concepts, not every detail.
3. Search existing wiki pages before creating new pages.
4. Update existing pages first.
5. Create a new page only when the concept is stable, recurring, and likely to be linked from several places.
6. Use inline wiki-style links in natural sentences.
7. Add source references to the page section that used the material.
8. Update `wiki/Home.md` only when the project map materially changes.
9. Preserve uncertainty and contradictions.
10. Keep prose drafts and long legacy passages out of the active wiki.

## Linking Rules

Use links where they improve traversal:

```md
The [[Factions|Luminaries]] operate through subtle [[Cosmology|energy resonance]] rather than spectacle.
```

Avoid link dumps:

```md
Related:
- Luminaries
- Energy
- Artifacts
```

Allowed exceptions: `wiki/Home.md` and deliberate index pages may group links, but they should still be meaningful.

## Page Quality Rules

A good NovaSaga wiki page:

- is short enough for future agents to read quickly;
- distinguishes canon from provisional material;
- links important concepts inline;
- has `Source notes` for archive or raw evidence;
- improves future story reasoning.

A weak page:

- copies archive content wholesale;
- creates many tiny pages;
- treats old generated text as final truth;
- mixes technical setup into creative lore;
- over-explains power mechanics before story need is clear.

## First-Pass Curation Bias

During the clean restart, favor durable foundations:

- core premise;
- themes;
- Luminaries and dark beings;
- global electricity collapse;
- hidden realms and sanctuaries;
- artifacts;
- Book 1 candidate arc;
- current open questions.

Do not build a full encyclopedia until the user settles the direction.
