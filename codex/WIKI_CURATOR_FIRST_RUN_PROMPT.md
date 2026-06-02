# NovaSaga Wiki Curator — First Run Prompt

Use this prompt for Codex when starting the first serious wiki-curation pass after the clean restart.

## Role

You are the NovaSaga wiki curator.

Use `skills/lore-curator/SKILL.md` as the controlling instruction file.

## Objective

Rebuild the active NovaSaga wiki into a clean, usable, interlinked knowledge base without blindly restoring the legacy archive.

The current active wiki is mostly skeletal. The archive contains useful old concepts, but old material must be treated as source evidence, not automatic canon.

## Repository Context

- Repo: `Wolfrine/NovaSaga`
- Branch: `main`
- Active wiki path: `wiki/`
- Policy/meta path: `meta/`
- Raw intake path: `raw/`
- Legacy archive path: `archive/legacy-before-restart-2026-06-02/`
- Skill file: `skills/lore-curator/SKILL.md`

## Required Inputs to Inspect

Inspect at minimum:

- `skills/lore-curator/SKILL.md`
- `meta/CanonPolicy.md`
- `meta/NOVASAGA_RESTART_PRINCIPLES.md`
- `meta/ToneAndStyle.md`
- `wiki/Home.md`
- `wiki/CorePremise.md`
- `wiki/Themes.md`
- `wiki/OpenQuestions.md`
- `wiki/Cosmology/README.md`
- `wiki/Factions/README.md`
- `wiki/Artifacts/README.md`
- `wiki/Events/README.md`
- `wiki/World/README.md`
- `wiki/Characters/README.md`
- `archive/legacy-before-restart-2026-06-02/Core concepts.md`
- `archive/legacy-before-restart-2026-06-02/Plot_raw.md`
- `archive/legacy-before-restart-2026-06-02/Plot_outline.md`

## First Pass Scope

Do not attempt to fully curate the entire archive.

Perform only the foundation pass:

1. Expand `meta/CanonPolicy.md` with clear canon/provisional/candidate/deprecated/archive-only rules.
2. Expand `wiki/Home.md` into the active navigation map for future agents.
3. Expand `wiki/CorePremise.md` using only the strongest story-level premise points.
4. Expand `wiki/OpenQuestions.md` with unresolved choices instead of forcing final answers.
5. Add short, clearly labeled sections to:
   - `wiki/Cosmology/README.md`
   - `wiki/Factions/README.md`
   - `wiki/Artifacts/README.md`
   - `wiki/Events/README.md`
   - `wiki/World/README.md`
   - `wiki/Themes.md`
6. Leave `drafts/` untouched.
7. Leave `archive/` untouched.

## Curation Rules

- Do not paste long archive text into the active wiki.
- Do not call every old idea canon.
- Use `Provisional` or `Candidate` when uncertain.
- Preserve contradictions explicitly in `wiki/OpenQuestions.md`.
- Keep pages concise and useful for future writing.
- Remove generic AI praise language such as “rich,” “compelling,” “immersive,” unless it encodes a real decision.
- Add relative markdown links between related pages.
- Keep the active wiki focused on creative/story knowledge, not software/product implementation.

## High-Signal Legacy Concepts to Evaluate

From the legacy archive, evaluate these as candidate/provisional knowledge:

- Luminaries as subtle guardians of balance.
- Dark Beings as corruption/negative-energy manifestations, not flat evil monsters.
- Global permanent electricity disruption caused by a cosmic/celestial event affecting electricity/metal.
- Hidden realms or sanctuaries with barriers weakened by the cosmic event.
- Artifacts energized by Luminaries that amplify the holder’s energy and can heal or corrupt.
- Belief/disbelief constraining open power display.
- Negashakti/negative frequencies as emotional/environmental corruption.
- Human free will and responsibility as central to the story.
- Subtlety over spectacle in power usage.
- Friend group trekking/river/boat incident leading into hidden sanctuary.
- One friend captured or corrupted as a major emotional stake.
- Training, global missions, artifact recovery, and multi-front final conflict.
- Portals/interplanetary beings as possible later expansion, likely candidate/provisional.

## Expected Final Response

After editing, respond with:

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
- `<path>` — <reason>
```

## Success Criteria

The result is successful if a future agent can open `wiki/Home.md`, understand the current NovaSaga restart state, navigate the major active pages, and clearly distinguish canon from provisional/candidate material.
