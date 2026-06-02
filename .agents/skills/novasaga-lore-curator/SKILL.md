---
name: novasaga-lore-curator
description: Curate NovaSaga raw notes and archived lore into compact, linked lore records while preserving uncertainty, source evidence, and authorial intent.
---

# NovaSaga Lore Curator

Use this skill when updating NovaSaga's active `wiki/`, processing `raw/` notes, or selectively curating material from `archive/legacy-before-restart-2026-06-02/`.

## Core Purpose

Maintain the active wiki as an agent-readable body of lore records. The wiki should feel like a compact archive of observed systems, social structures, hidden traditions, older accounts, terms, histories, and unresolved phenomena from a world whose patterns already exist.

Use Tolkien-style discipline as inspiration: appendices, records, timelines, terms, lineages, language/history traces, mundane details, and metaphysical depth. Do not imitate Tolkien's prose.

## Repository Roles

- `wiki/`: refined story knowledge only.
- `raw/`: source notes and rough inputs. Treat raw notes as evidence, not final pages.
- `archive/legacy-before-restart-2026-06-02/`: preserved pre-restart material. Use selectively.
- `drafts/`: prose drafts. Do not rewrite unless explicitly asked.
- `meta/`: canon and style policy.
- `codex/`: execution workflow for agents.

## Continuity Status Labels

Use these labels internally whenever a claim could affect continuity:

- `Canon`: accepted for now unless the user changes it.
- `Provisional`: likely useful but still open to reshaping.
- `Candidate`: interesting legacy idea not yet adopted.
- `Open question`: unresolved decision or contradiction.
- `Deprecated`: preserved for history but should not guide new work.

If a source is unclear, mark the idea `Candidate` or `Open question`; do not upgrade it to `Canon`.

In active wiki pages, translate those project labels into lore-record labels:

- `Known`: stable record; maps roughly to canon.
- `Suspected`: repeated or useful account, but not settled.
- `Disputed`: conflicting accounts or terminology.
- `Unresolved`: an open phenomenon, missing lineage, unclear cause, or undecided account.
- `Rejected / Archive-only`: preserved outside active lore unless the user asks.

Avoid letting `Canon`, `Provisional`, or `Candidate` dominate active wiki pages. Those are curator judgments, not the natural voice of the lore record.

## Lore Record Tone

Do not write active wiki pages as project notes, pitch copy, or story summaries.

Avoid:

- "NovaSaga is about..."
- "The story should..."
- "Book 1 likely..."
- "The active wiki..."
- "This project..."

Prefer:

- "After the Event..."
- "Older accounts describe..."
- "The known forms are..."
- "This remains disputed..."
- "Among survivors this is called..."
- "Records disagree on..."
- "The hidden orders preserve..."
- "No reliable account yet explains..."

The active wiki should sound like a clear archivist's record, not a marketing page and not a planning document.

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
11. Rewrite planning-language findings into lore-record language before saving active wiki pages.

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
- distinguishes known, suspected, disputed, and unresolved material;
- links important concepts inline;
- has `Source notes` for archive or raw evidence;
- improves future story reasoning while reading like an internal lore record.

A weak page:

- copies archive content wholesale;
- creates many tiny pages;
- treats old generated text as final truth;
- mixes technical setup into creative lore;
- over-explains power mechanics before story need is clear.
- reads like a project plan, pitch, task list, or "what the story should do" memo.

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

Use unique wiki note names such as `World.md`, `Factions.md`, and `Events.md`. Do not create category pages as `README.md`, because Obsidian graph view displays file names and repeated README nodes make the mobile graph hard to read.

Do not build a full encyclopedia until the user settles the direction.
