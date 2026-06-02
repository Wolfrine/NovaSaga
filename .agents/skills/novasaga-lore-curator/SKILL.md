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

Do not use status labels as normal headings in active wiki pages. `Canon`, `Provisional`, `Candidate`, `Known`, `Suspected`, `Disputed`, and `Unresolved` are curator bookkeeping, not the natural voice of the lore record.

Active wiki pages should use story-world headings such as `The Luminary Method`, `Concealment as Containment`, `Places That Remember`, `Older Names`, or `Unsettled Accounts`. Preserve uncertainty through natural phrasing: "records disagree", "the scope remains unclear", "no reliable account yet explains", or "older variants preserve".

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
2. Preserve the user's thought-chain before applying curator classification. Do not soften, downgrade, reinterpret, or scatter the central intent on your own.
3. Identify durable story concepts, not every detail.
4. Search existing wiki pages before creating new pages.
5. Update existing pages first.
6. Create a new page only when the concept is stable, recurring, and likely to be linked from several places.
7. Use inline wiki-style links in natural sentences.
8. Add source references to the page section that used the material.
9. Update `raw/CURATION_LEDGER.md` so every current raw file has a status, last curated commit if known or `TBD`, target wiki pages, and notes.
10. Update `wiki/Home.md` only when the project map materially changes.
11. Preserve uncertainty and contradictions in natural lore language, but only where the source itself is uncertain or conflicts with another active record.
12. Keep prose drafts and long legacy passages out of the active wiki.
13. Rewrite planning-language findings into lore-record language before saving active wiki pages.

## Authorial Intent Guardrail

Raw notes are not merely a supply of claims to downgrade into `Suspected` and `Disputed` lines. First identify the author's core intent and keep that intent visible as a coherent record.

Do:

- keep the central idea together when splitting it would weaken its force;
- preserve causal chains, metaphors, and stated reasons when they are the point of the note;
- keep certainty labels out of active wiki headings and body text unless the page is a ledger or policy document;
- phrase only the source's own questions as uncertain;
- distinguish uncertain scope from uncertain principle.

Do not:

- replace a direct user premise with generic phrasing such as "some accounts say" unless the source itself frames the premise as hearsay;
- flatten a specific mechanism into vague tradition language;
- downgrade a stated premise because future continuity might be easier if it stayed vague;
- turn every sentence touching religion, cosmology, or metaphysics into a disputed classification.

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
- reads with a clear narrative mind rather than visible status bookkeeping;
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
