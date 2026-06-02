# Lore Curator

Purpose: guide Codex agents when organizing, reconciling, and documenting NovaSaga lore during the clean restart.

## When to Use This Skill

Use this skill whenever the task involves:

- turning raw notes, old archive material, brainstorming fragments, chat exports, or loose lore into the NovaSaga wiki;
- deciding whether something belongs in canon, provisional canon, deprecated notes, raw intake, or archive;
- improving wiki structure, page links, continuity, naming, or discoverability;
- extracting worldbuilding, character, plot, theme, cosmology, artifact, faction, or event knowledge from older material.

Do **not** use this skill for prose polishing, chapter rewriting, copyediting, or style-only edits. Use `skills/prose-editor/SKILL.md` for prose refinement.

## Project Frame

NovaSaga is a novel-writing and worldbuilding workspace, not a software product. Treat the repository as a creative knowledge base plus draft-writing space.

Current restart intent:

- preserve old material under `archive/legacy-before-restart-2026-06-02/`;
- rebuild the active wiki from scratch in a controlled, higher-quality form;
- avoid blindly restoring the old structure or dumping archive content back into active canon;
- keep the active wiki clean, navigable, interlinked, and useful for future writing agents.

## Core Operating Rule

Never convert legacy material directly into canon just because it exists.

Every extracted point must be classified as one of:

| Status | Meaning | Action |
|---|---|---|
| `Canon` | Firmly accepted current truth | Place in the relevant wiki page and link from related pages. |
| `Provisional` | Useful but not yet final | Add to the relevant wiki page under a `Provisional` section or to `wiki/OpenQuestions.md`. |
| `Candidate` | Interesting idea needing user decision | Summarize briefly in `wiki/OpenQuestions.md`. |
| `Deprecated` | Older idea that should not drive future writing | Keep only as a note if needed; do not place in active wiki as truth. |
| `Archive-only` | Historical reference, low current value | Leave in archive; optionally mention in curation notes. |

When uncertain, choose `Provisional` or `Candidate`, not `Canon`.

## IAC + ADS + ODD for This Skill

### IAC — Impact Area Context

The impact area is the active NovaSaga knowledge system:

- `wiki/Home.md`
- `wiki/CorePremise.md`
- `wiki/Themes.md`
- `wiki/OpenQuestions.md`
- `wiki/World/`
- `wiki/Characters/`
- `wiki/Events/`
- `wiki/Factions/`
- `wiki/Cosmology/`
- `wiki/Artifacts/`
- `meta/CanonPolicy.md`
- `meta/ToneAndStyle.md`
- `raw/`
- `archive/legacy-before-restart-2026-06-02/`

The goal is not to produce more text. The goal is to create a usable writing memory that future agents can navigate.

### ADS — Autonomous Discovery Scope

The curator may autonomously inspect:

- active wiki files;
- `raw/` intake notes;
- legacy archive files;
- existing `meta/` policy files;
- draft README files only for structure awareness.

The curator may create or update wiki/meta/raw files when doing so improves clarity.

The curator must **not**:

- rewrite prose chapters unless explicitly asked;
- invent final canon where the source is ambiguous;
- collapse contradictory ideas into one fake-clean answer;
- delete archive material;
- assume this is a product/app/website repository;
- add implementation/deployment/automation details into the creative wiki.

### ODD — Output Delivery Direction

Each curator run must leave behind:

1. updated wiki/meta files with clear headings and internal links;
2. a short curation summary in the final response;
3. a list of canon changes made;
4. a list of provisional/candidate items needing user decision;
5. any contradictions or weak spots discovered.

## Active Wiki Shape

Maintain this high-level structure unless the user changes it:

```text
wiki/
  Home.md
  CorePremise.md
  Themes.md
  OpenQuestions.md
  Characters/
    README.md
  World/
    README.md
  Events/
    README.md
  Factions/
    README.md
  Cosmology/
    README.md
  Artifacts/
    README.md
meta/
  CanonPolicy.md
  ToneAndStyle.md
raw/
  README.md
archive/
  legacy-before-restart-2026-06-02/
```

Recommended page roles:

- `Home.md`: entry point, map of major pages, reading path for new agents.
- `CorePremise.md`: current story promise, conflict engine, protagonist frame, stakes.
- `Themes.md`: philosophical/emotional anchors, not generic fantasy slogans.
- `OpenQuestions.md`: unresolved choices, contradictions, and decision prompts.
- `World/README.md`: geography, society, hidden realms, collapse conditions, everyday life.
- `Characters/README.md`: known characters, groups of characters, arcs, relationships.
- `Events/README.md`: timeline, cosmic event, collapse, sanctuary attacks, wars.
- `Factions/README.md`: luminaries, dark beings, human groups, institutions, alliances.
- `Cosmology/README.md`: energy/frequency rules, belief, powers, metaphysics, portals.
- `Artifacts/README.md`: relics, energy objects, detection/use rules, risks.
- `CanonPolicy.md`: how canon/provisional/deprecated/archive statuses work.
- `ToneAndStyle.md`: realism level, power portrayal, prose direction, anti-patterns.

## Curation Method

For each source file inspected:

1. Identify source path and source type: `raw`, `archive`, `wiki`, `meta`, or `draft`.
2. Extract atomic knowledge units. Each unit should be one clear claim, rule, entity, event, or open question.
3. Classify each unit as `Canon`, `Provisional`, `Candidate`, `Deprecated`, or `Archive-only`.
4. Place the unit in the smallest correct wiki page.
5. Add links to related pages using relative markdown links.
6. Avoid duplicating the same idea across many pages. Prefer one source-of-truth page with links.
7. Add contradictions or unresolved variants to `wiki/OpenQuestions.md`.
8. Keep source notes brief. Do not paste long archive passages into active wiki.

## Extraction Heuristics

Treat these legacy concepts as high-signal candidates, but not automatically final:

- Luminaries as subtle guardians of balance.
- Dark Beings as corruption/negative-energy manifestations with recoverable human depth.
- Global permanent electricity disruption caused by a cosmic event affecting metal/electricity.
- Hidden realms/sanctuaries whose barriers weaken during the cosmic event.
- Artifacts that amplify energy and can heal or corrupt depending on the holder.
- Belief/disbelief as a constraint on visible powers.
- Negashakti/negative frequencies as environmental and emotional corruption.
- Human responsibility/free will as more central than superhero spectacle.
- Subtle power use over flashy combat.
- Friend group entering a hidden sanctuary during a trekking/river incident.
- One friend being captured/corrupted as an emotional stake.
- Training, global missions, artifact recovery, and multi-front final conflict as possible arc components.
- Portals/interplanetary beings as expansion material, likely provisional unless user confirms.

## Quality Bar

A good curated wiki page is:

- short enough to read quickly;
- specific enough to guide writing;
- explicit about canon vs provisional uncertainty;
- linked to related pages;
- free from generic AI praise/filler;
- written in clean, direct language;
- useful to a future agent that has no chat history.

A bad curated wiki page:

- copies entire old archive sections;
- says everything is rich, epic, immersive, powerful, or compelling without decisions;
- mixes canon, candidate, and abandoned ideas without labels;
- contains product/software assumptions;
- creates pages that are not linked from anywhere;
- overwrites ambiguity with invented certainty.

## Required Internal-Link Pattern

When updating a page, add a `Related` section if useful:

```md
## Related

- [Core Premise](../CorePremise.md)
- [Themes](../Themes.md)
- [Open Questions](../OpenQuestions.md)
```

Adjust relative paths correctly depending on file location.

## Required Open Question Format

Use this format inside `wiki/OpenQuestions.md`:

```md
## <Question Area>

### Q: <specific unresolved question>

- **Status:** Candidate / Provisional / Contradiction
- **Why it matters:** <one-line reason>
- **Known options:**
  - Option A: <brief>
  - Option B: <brief>
- **Current lean:** <if available, otherwise `Unclear`>
- **Evidence/source:** <source path or active page>
```

## Required Curation Summary Format

End each Codex response with:

```md
## Curation Summary

### Files changed
- `<path>` — <what changed>

### Canon added/updated
- <item>

### Provisional/candidate items
- <item>

### Contradictions / decisions needed
- <item>

### Not touched
- <important relevant files intentionally left unchanged>
```

## Safety Against Over-Curation

If the repo contains only stubs or weak pages, first build the skeleton and policy. Do not try to solve the whole novel in one run.

Prefer 3-7 well-curated active pages over 30 thin pages.

If archive material is large, process it in batches:

1. core premise and themes;
2. cosmology and power rules;
3. world/collapse/sanctuaries;
4. factions and artifacts;
5. characters and plot/events;
6. contradictions and open questions.

## First Run Recommendation

For NovaSaga’s current restart state, the first strong curator run should:

1. expand `meta/CanonPolicy.md`;
2. expand `wiki/Home.md` as the navigation map;
3. expand `wiki/CorePremise.md` using only the strongest accepted/candidate premise points;
4. expand `wiki/OpenQuestions.md` with unresolved decisions instead of forcing canon;
5. lightly update `wiki/Cosmology/README.md`, `wiki/Factions/README.md`, `wiki/Artifacts/README.md`, and `wiki/Events/README.md` using short provisional sections;
6. avoid touching prose drafts.
