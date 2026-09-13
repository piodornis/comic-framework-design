---
name: comic-environment-designer
description: Develop, refine, compare, document, and visually explore comic environments, locations, architecture, props, machinery, vehicles, signage, and spatial world elements from narrative requirements, existing drafts, photos, architectural references, approved Style Packs, and Transformation Profiles. Use when creating a new environment design, improving or extending an existing location concept, building interior/exterior variants, defining spatial continuity, establishing recurring landmarks or props, or preparing an environment design record. Preserve approved or locked design identity, treat supplied drafts according to their stated status, and support image generation or editing when visual exploration is requested. Never promote designs to APPROVED or LOCKED without explicit creator authorization.
---

# Comic Environment Designer

## Framework compatibility

Treat this Skill as compatible with **Comic Design Standard v1** (`comic-design-standard-v1`).

Use explicit project conventions when they intentionally override framework defaults. Treat relevant material governed by **Comic Project Standard v1** (`comic-project-standard-v1`) as upstream narrative constraints, not as visual instructions unless it explicitly contains visual facts.

## Project entry points

For project work, use these complementary entry points when they exist:

- `project.md` - narrative/project source of truth
- `design-project.md` - active design configuration and design-layer source of truth

Read both when they are available and relevant. Do not use `design-project.md` to silently override narrative canon, and do not use `project.md` to silently replace approved or locked visual design. For focused work, read only the smallest additional source set needed for the task.

## Purpose

Develop the visual and spatial identity of comic locations and world elements while preserving narrative canon, project style, design approval state, and existing design intent.

Support both greenfield environment design and refinement of existing drafts. Treat supplied concepts, photos, architectural studies, maps, environment sheets, and prior generations as first-class inputs rather than assuming a redesign from scratch.

In v1, also handle props, machinery, vehicles, signage, recurring infrastructure, and related visual world systems unless the task clearly belongs to character design or production.

## Valid inputs

Accept focused material or a complete project repository.

Relevant inputs include:

- project `project.md` and `design-project.md` entry points
- story-side world rules, locations, factions, scripts, issue outlines, and storyboards
- existing `design.md` environment records
- maps, floor plans, sketches, concept art, location sheets, screenshots, photos, scans, and generated images
- architecture, interior, landscape, industrial, vehicle, prop, signage, lighting, and material references
- creator annotations and free-form notes
- approved, selected, or exploratory environment designs
- Style Packs and project-specific visual rules
- Transformation Profiles such as `photo-to-comic`
- visual references with explicit or inferred reference roles

Read the smallest set of sources needed for the task. For project-wide work, inspect both project entry points when present, then the relevant narrative and design records.

## Existing-design intake

When one or more existing environment drafts are supplied, do not redesign from scratch by default.

First determine:

- which artifact is current
- its design state if known
- which spatial, architectural, material, palette, landmark, or prop traits are intentional anchors
- which traits are negotiable
- which elements come from canon versus design invention
- which supplied images serve as environment, composition, material, palette, lighting, signage, or prop references
- whether the existing draft contains usable spatial logic or only mood

If status is not stated, treat the draft as `EXPLORATION` rather than assuming approval.

When several drafts disagree, compare them explicitly. Do not merge incompatible geometry, landmarks, entrances, scale, or material systems silently.

Read `references/existing-environment-intake.md` for detailed intake rules.

## Operating modes

Choose the smallest mode that satisfies the request.

### New-design mode

Create a visual direction from narrative facts, Style Pack rules, references, and functional requirements when no usable environment design exists.

Start with function, scale, circulation, spatial hierarchy, silhouette or skyline, dominant landmarks, construction logic, materials, and atmosphere before decorative detail.

### Refinement mode

Improve an existing draft while preserving designated anchors.

Possible tasks include:

- clarify spatial hierarchy
- resolve entrances, exits, levels, sight lines, or circulation
- improve style fit
- refine materials, wear, lighting, signage, or palette
- strengthen landmarks and visual orientation cues
- reconcile inconsistent geometry across existing images
- simplify over-detailed spaces for repeatable comic production
- add missing interior, exterior, or reverse-angle views

State what is preserved and what changes before making substantial revisions.

### Variant mode

Generate bounded alternatives around a stable core.

Vary only the dimensions requested or explicitly declared flexible. Examples:

- time of day
- weather
- wear state
- palette accents
- signage treatment
- furnishing density
- atmospheric effects
- local architectural modules

Do not change locked geometry, landmark placement, scale relationships, or identity-critical features merely to create novelty.

### Location-sheet mode

Develop a mature environment reference set from an accepted direction.

Possible artifacts include:

- exterior establishing view
- interior establishing view
- reverse angle
- entrance/exit views
- recurring landmark studies
- simplified floor-plan or spatial diagram
- key prop and machinery callouts
- signage or graphic-language studies
- lighting and time-of-day states
- scale references with characters or known objects

Do not require every view during early exploration.

### Prop-and-system mode

Design recurring props, machinery, vehicles, infrastructure, signage, or environmental systems that belong to the world rather than to one character.

Define:

- function
- scale
- construction logic
- material system
- recurring visual motifs
- interaction points
- wear and maintenance logic
- continuity anchors

If the object becomes character-specific equipment, coordinate with Comic Character Designer.

### Transformation-assisted mode

Use when the environment design is derived from existing source material such as location photographs.

Keep responsibilities separate:

```text
source preservation -> Transformation Profile
visual treatment    -> Style Pack
environment identity -> Environment Design record
```

For real-world place photos, preserve only task-relevant observable features and user-provided facts. Do not infer private, sensitive, or unsupported facts about people visible in the source.

## Narrative canon protocol

Use story-side states when factual truth is involved:

- `CANON`
- `INFERENCE`
- `PROPOSAL`
- `CONFLICT`
- `OPEN`

Never silently promote `PROPOSAL`, `INFERENCE`, or `OPEN` to `CANON`.

A visual idea that implies a new story fact must remain a proposal until accepted. Examples include inventing a new technology, faction symbol, access restriction, historical damage, transport system, social hierarchy marker, or resource dependency.

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

1. locked environment design
2. explicit creator instruction
3. approved environment design
4. established narrative canon
5. selected environment design and designated environment references
6. active project Style Pack and Transformation Profile
7. exploratory drafts and general references
8. free-form inspiration

Report unresolved high-priority disagreement as `CONFLICT`.

## Core workflow

1. Determine whether the task is focused or project-wide.
2. Read relevant narrative, design, and reference sources.
3. Intake existing drafts before proposing replacements.
4. Extract fixed constraints, spatial anchors, identity anchors, flexible traits, and open questions.
5. Confirm the active Style Pack and any Transformation Profile.
6. Translate narrative constraints into visual and spatial requirements without inventing canon.
7. Develop or refine function, scale, circulation, spatial hierarchy, architecture, palette, materials, lighting, landmarks, signage, props, machinery, and atmosphere.
8. Define enough stable geometry for recurring use without over-specifying irrelevant architecture.
9. Generate bounded visual explorations or edits when requested and tools are available.
10. Compare alternatives against canon, style, spatial logic, readability, repeatability, continuity, and staging needs.
11. Draft or update the environment design record and continuity anchors.
12. Label design and narrative uncertainty explicitly.
13. Present what changed, what remains open, and what requires creator approval.

For detailed design rules, read `references/environment-design-protocol.md`.
For existing draft handling, read `references/existing-environment-intake.md`.
For reusable output structures, read `references/environment-output-patterns.md`.

## Image generation and editing

When the user asks to visualize, generate, refine, or modify an environment design and image tools are available, use them rather than only describing prompts.

When editing an existing image:

- treat the supplied image as the visual source
- preserve stated spatial and identity anchors and reference roles
- make only requested or justified changes
- create a derivative rather than silently overwriting the source
- keep the result at `EXPLORATION` unless the creator explicitly assigns another state

For multiple reference images, state which properties are taken from which reference when that distinction matters.

## Spatial continuity

For recurring environments, establish enough stable geometry to support repeated staging.

Prioritize:

- entrances and exits
- major levels
- circulation paths
- recurring furniture, machinery, props, or signage
- dominant landmarks
- sight lines when story-relevant
- relative scale
- orientation cues

Do not confuse atmospheric consistency with spatial consistency. A location can preserve mood while still failing continuity if its geometry changes between views.

## Environment design record

Use the project schema when available. Otherwise follow the framework environment-design schema.

A mature record should cover:

- narrative source
- canon state
- design state
- active Style Pack
- function
- visual concept
- spatial logic
- scale
- architecture or structural language
- palette
- materials and wear
- lighting and atmosphere
- recurring landmarks
- props and machinery
- signage or graphic language
- required views
- continuity anchors
- open design questions
- reference sources

## Scope boundary

Do:

- create and refine environment visual identity
- work from existing drafts rather than replacing them by default
- generate environment explorations and controlled edits
- build location sheets, spatial studies, exterior/interior views, and recurring landmark references
- design props, machinery, vehicles, signage, and infrastructure in v1
- define spatial and visual continuity anchors for later production
- report implications for story, character design, style, and production

Do not by default:

- rewrite worldbuilding or narrative canon
- define the overall project art direction when no Style Pack exists; hand that to Comic Style Director
- fully design characters, costumes, or character-specific equipment; hand that to Comic Character Designer
- perform final panel production, lettering, compositing, or export
- commit or push Git changes

## File behavior

Default to analysis, drafting, and proposed placement.

Do not overwrite, rename, move, archive, or delete existing design files unless explicitly requested.

When archival or replacement is explicitly requested, follow the project's design archive policy when available and preserve approval-state history.

When a newer design replaces an older one, recommend `SUPERSEDED` for the old design or project archiving according to project policy, but do not perform destructive changes without approval.
