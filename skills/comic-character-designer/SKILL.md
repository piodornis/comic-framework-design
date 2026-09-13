---
name: comic-character-designer
description: Develop, refine, compare, document, and visually explore comic character designs from narrative requirements, existing drafts, image references, photos, sketches, approved Style Packs, and Transformation Profiles. Use when creating a new character appearance, improving or extending an existing design, producing variants, turnarounds, expression or pose studies, costume or equipment variants, continuity anchors, or a character design record. Preserve approved or locked design identity, treat supplied drafts according to their stated status, and support image generation or editing when visual exploration is requested. Never promote designs to APPROVED or LOCKED without explicit creator authorization.
---

# Comic Character Designer

## Framework compatibility

Treat this Skill as compatible with **Comic Design Standard v1** (`comic-design-standard-v1`).

Use the project's explicit conventions when they intentionally override framework defaults. Treat relevant story-framework outputs as upstream narrative constraints, not as visual instructions unless they explicitly contain visual facts.

## Project entry points

For project work, use these complementary entry points when they exist:

- `project.md` - narrative/project source of truth
- `design-project.md` - active design configuration and design-layer source of truth

Read both when they are available and relevant. Do not use `design-project.md` to silently override narrative canon, and do not use `project.md` to silently replace approved or locked visual design. For focused work, read only the smallest additional source set needed for the task.

## Purpose

Develop the visual identity of comic characters while preserving narrative canon, project style, design approval state, and existing design intent.

Support both greenfield design and refinement of existing drafts. Do not assume that a new generated image is preferable to a supplied design.

## Valid inputs

Accept focused material or a complete project repository.

Relevant inputs include:

- project `project.md` and `design-project.md` entry points
- story-side character profiles, relationships, world rules, scripts, and storyboards
- existing `design.md` records
- sketches, concept art, character sheets, turnarounds, screenshots, photos, and generated images
- creator annotations and free-form notes
- approved, selected, or exploratory character designs
- Style Packs and project-specific style rules
- Transformation Profiles such as `photo-to-comic`
- visual references with explicit or inferred reference roles

Read the smallest set of sources needed for the task. For project-wide work, inspect both project entry points when present, then the relevant narrative and design records.

## Existing-design intake

When one or more existing character drafts are supplied, do not redesign from scratch by default.

First determine:

- which artifact is current
- its design state if known
- which visual traits are intentional anchors
- which traits are negotiable
- which elements come from canon versus design invention
- which supplied images serve as identity, costume, pose, palette, linework, material, or style references

If status is not stated, treat the draft as `EXPLORATION` rather than assuming approval.

When several drafts disagree, compare them explicitly. Do not average incompatible traits silently.

Read `references/existing-design-intake.md` for detailed intake rules.

## Operating modes

Choose the smallest mode that satisfies the request.

### New-design mode

Create a visual direction from narrative facts, style rules, and references when no usable design exists.

Start with silhouette, proportions, visual hierarchy, identifying features, material or costume logic, and expression/body-language system before decorative detail.

### Refinement mode

Improve an existing draft while preserving designated anchors.

Possible tasks include:

- clarify silhouette
- resolve proportion problems
- improve style fit
- refine palette or materials
- improve expression readability
- simplify or organize costume/equipment
- add missing views
- reconcile inconsistent details across existing images

State what is preserved and what changes before making substantial revisions.

### Variant mode

Generate bounded alternatives around a stable core.

Vary only the dimensions requested or explicitly declared flexible. Examples:

- palette
- costume
- shell panels
- hairstyle
- accessories
- age or wear state when canon allows it
- facial-expression treatment

Do not change locked or identity-critical features merely to create novelty.

### Sheet-development mode

Develop a mature character reference set from an accepted direction.

Possible artifacts include:

- front, side, and rear views
- neutral pose
- expression sheet
- pose/body-language sheet
- hand, manipulator, or face detail studies
- recurring equipment
- costume or module variants
- scale comparison
- damage or age states when story-relevant

Do not require every view during early exploration.

### Transformation-assisted mode

Use when the character design is derived from existing source material such as photographs.

Keep responsibilities separate:

```text
source preservation -> Transformation Profile
visual treatment    -> Style Pack
character identity  -> Character Design record
```

For real-person photos, preserve only task-relevant observable features and user-provided facts. Do not infer sensitive traits from appearance.

## Narrative canon protocol

Use the story-side states when factual truth is involved:

- `CANON`
- `INFERENCE`
- `PROPOSAL`
- `CONFLICT`
- `OPEN`

Never silently promote `PROPOSAL`, `INFERENCE`, or `OPEN` to `CANON`.

A visual idea that implies a new story fact must remain a proposal until accepted. Examples include adding a scar, insignia, weapon, prosthetic, injury, or status symbol not already supported by canon.

## Design approval protocol

Use these independent visual states:

- `EXPLORATION`
- `SELECTED`
- `APPROVED`
- `LOCKED`
- `SUPERSEDED`

Never promote an artifact to `APPROVED` or `LOCKED` without explicit creator authorization.

Treat `APPROVED` designs as the preferred current reference. Treat `LOCKED` designs as immutable unless the creator explicitly authorizes a change.

## Source priority

Unless project rules specify otherwise, prefer:

1. locked character design
2. explicit creator instruction
3. approved character design
4. established narrative canon
5. selected character design and designated identity references
6. active project Style Pack and Transformation Profile
7. exploratory drafts and general references
8. free-form inspiration

Report unresolved high-priority disagreement as `CONFLICT`.

## Core workflow

1. Determine whether the task is focused or project-wide.
2. Read the relevant narrative and design sources.
3. Intake existing drafts before proposing replacements.
4. Extract fixed constraints, identity anchors, flexible traits, and open questions.
5. Confirm the active Style Pack and any Transformation Profile.
6. Translate narrative constraints into visual requirements without inventing canon.
7. Develop or refine silhouette, proportions, construction, palette, materials, costume or shell, markings, expression system, and body language.
8. Generate bounded visual explorations or edits when requested and tools are available.
9. Compare alternatives against canon, style, identity anchors, readability, repeatability, and continuity needs.
10. Draft or update the character design record and continuity anchors.
11. Label design and narrative uncertainty explicitly.
12. Present what changed, what remains open, and what requires creator approval.

For detailed design rules, read `references/character-design-protocol.md`.
For existing draft handling, read `references/existing-design-intake.md`.
For reusable output structures, read `references/character-output-patterns.md`.

## Image generation and editing

When the user asks to visualize, generate, refine, or modify a character design and image tools are available, use them rather than only describing prompts.

When editing an existing image:

- treat the supplied image as the visual source
- preserve stated identity anchors and reference roles
- make only the requested or justified changes
- create a derivative rather than silently overwriting the source
- keep the result at `EXPLORATION` unless the creator explicitly assigns another state

For multiple reference images, state which properties are taken from which reference when that distinction matters.

## Character design record

Use the project schema when available. Otherwise follow the framework character-design schema.

A mature record should cover:

- narrative source
- canon state
- design state
- active Style Pack
- design intent
- silhouette
- proportions and scale
- face or display language
- body/form construction
- palette
- materials and surfaces
- clothing, shell, or costume
- markings and identifiers
- accessories and recurring equipment
- expression or emotion system
- pose/body-language guidance
- approved variations
- continuity anchors
- open design questions
- reference sources

## Scope boundary

Do:

- create and refine character visual identity
- work from existing drafts rather than replacing them by default
- generate character explorations and controlled edits
- build turnarounds, expression, pose, costume, and equipment studies
- define continuity anchors for later production
- report implications for style, environment, story, and continuity

Do not by default:

- rewrite narrative character biographies or canon
- define the overall project art direction when no Style Pack exists; hand that to Comic Style Director
- fully design environments or locations; hand that to Comic Environment Designer
- perform final panel production, lettering, compositing, or export
- commit or push Git changes

## File behavior

Default to analysis, drafting, and proposed placement.

Do not overwrite, rename, move, archive, or delete existing design files unless explicitly requested.

When archival or replacement is explicitly requested, follow the project's design archive policy when available and preserve approval-state history.

When a newer design replaces an older one, recommend `SUPERSEDED` for the old design or project archiving according to project policy, but do not perform destructive changes without approval.
