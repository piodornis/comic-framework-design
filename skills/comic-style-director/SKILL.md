---
name: comic-style-director
description: Define, refine, document, and visually explore reusable or project-specific comic visual styles. Use when creating or revising Style Packs, translating narrative/world/character requirements into art-direction rules, interpreting visual references, combining a Style Pack with a Transformation Profile such as photo-to-comic, establishing palettes, linework, shape language, materials, lighting, rendering, composition, and visual consistency rules, or generating bounded style explorations before character/environment design. Treat relevant outputs from story or narrative frameworks as upstream design constraints. Do not replace character or environment design work, and never promote visual artifacts to APPROVED or LOCKED without explicit creator authorization.
---

# Comic Style Director

## Framework compatibility

Treat this Skill as compatible with **Comic Design Standard v1** (`comic-design-standard-v1`).

Use the project's explicit conventions when they intentionally override framework defaults. Do not silently assume behavior from a newer contract.

## Project entry points

For project work, use these complementary entry points when they exist:

- `project.md` - narrative/project source of truth
- `design-project.md` - active design configuration and design-layer source of truth

Read both when they are available and relevant. Do not use `design-project.md` to silently override narrative canon, and do not use `project.md` to silently replace approved or locked visual design. For focused work, read only the smallest additional source set needed for the task.

## Purpose

Direct the visual language of a comic project without taking over character design, environment design, or final production.

Define how the project should look across characters, environments, props, transformed source material, concept art, and later production assets.

Keep three concepts separate:

- **narrative truth** — what exists or is true in the comic
- **visual design approval** — which visual solution has been accepted
- **visual style** — how approved or exploratory content is rendered

## Valid upstream inputs

Treat all relevant project material as valid input, including text produced through a story framework.

Possible sources include:

- `project.md`
- `design-project.md`
- canon and world rules
- character profiles and relationships
- locations, factions, institutions, technology, culture, and props
- story arcs, issue outlines, scripts, and storyboard descriptions
- existing design files and style documents
- image references, moodboards, photos, sketches, and concept art
- reusable Style Packs
- Transformation Profiles
- free-form creator direction

Do not read the entire repository mechanically when the request is narrow. Read the smallest set that establishes the required narrative and visual constraints.

When a complete project repository is available and the request is project-wide, inspect both project entry points when present and then the relevant narrative and design sources.

## Operating modes

Choose the smallest mode that satisfies the request.

### Style-definition mode

Use to create or substantially revise a visual style or Style Pack.

Define:

- intent and visual principles
- linework
- color treatment
- shape language
- rendering and shading
- texture and materials
- lighting
- composition
- character treatment
- environment treatment
- consistency anchors
- allowed variation
- avoidances and known failure modes

### Reference-interpretation mode

Use when the creator supplies images, photos, moodboards, sketches, or existing art.

Extract visual traits rather than treating every visible detail as a mandatory rule.

Distinguish:

- style reference
- palette reference
- linework reference
- material reference
- composition reference
- character reference
- environment reference

### Transformation-combination mode

Use when existing source material must be transformed.

Keep the responsibilities separate:

```text
source-preservation behavior -> Transformation Profile
visual treatment            -> Style Pack
```

For example:

```text
photo-to-comic + franco-belgian-vivid
photo-to-comic + manga-clean
```

Do not copy preservation rules into the Style Pack or aesthetic rules into the Transformation Profile.

### Visual-exploration mode

Use when the creator wants to see candidate visual directions.

When image-generation or image-editing tools are available and visualization is requested, generate bounded style explorations that test the style rather than producing final character sheets or final environment designs.

Label generated alternatives as `EXPLORATION` unless the creator explicitly changes their status.

## Narrative canon protocol

Use the story-side states when factual project truth is involved:

- `CANON` — confirmed project fact
- `INFERENCE` — conclusion supported by canon but not explicitly confirmed
- `PROPOSAL` — new creative suggestion
- `CONFLICT` — contradiction requiring resolution
- `OPEN` — unresolved point

Never silently promote `PROPOSAL`, `INFERENCE`, or `OPEN` to `CANON`.

If an appealing visual choice contradicts established story facts, mark the factual issue as `CONFLICT` instead of repairing the story through art direction.

## Design approval protocol

Use these independent visual states:

- `EXPLORATION` — uncommitted tests and alternatives
- `SELECTED` — chosen for further development
- `APPROVED` — explicitly accepted by the creator
- `LOCKED` — must not change without explicit authorization
- `SUPERSEDED` — replaced by a newer design

Never promote an artifact to `APPROVED` or `LOCKED` without explicit creator authorization.

When a design is `LOCKED`, report style conflicts instead of silently modifying the locked design.

## Source priority

Unless the project specifies another precedence, prefer:

1. locked or approved project design
2. explicit creator instruction
3. established narrative canon and project constraints
4. selected project design and style references
5. reusable Style Packs and Transformation Profiles
6. current exploration material
7. general inspiration and free notes

When two high-priority sources disagree, report `CONFLICT` and ask for a decision when necessary.

## Core workflow

1. Determine whether the task is focused or project-wide.
2. Read the relevant narrative, design, and reference sources.
3. Extract fixed constraints, desired qualities, open questions, and conflicts.
4. Separate source handling from visual style when a Transformation Profile is involved.
5. Define the style's visual principles before decorative specifics.
6. Translate principles into operational rules for line, color, shape, material, lighting, rendering, and composition.
7. Define consistency anchors and allowed variation.
8. Identify how the style should affect characters, environments, and props without designing those assets in full.
9. Generate or describe bounded visual explorations when requested.
10. Classify factual and design uncertainty using the two status systems.
11. Present a reusable style artifact plus conflicts, open decisions, and downstream guidance.

For detailed decision rules, read `references/style-direction-protocol.md`.
For reusable output structures, read `references/style-output-patterns.md`.

## Style Pack rules

When drafting a reusable Style Pack:

- keep it independent from one specific comic whenever possible
- describe visual treatment rather than project canon
- keep the rules usable by character and environment workflows
- avoid model-specific prompt syntax unless explicitly requested
- state compatibility notes and known failure modes
- include enough constraints for repeatable application

For a project-specific style, allow project-specific visual rules but keep narrative facts sourced from project canon rather than duplicated unnecessarily.

## Human Park and other project-specific styles

Treat a project-specific style such as Human Park as project material, not as a universal default for this Skill.

Use it when the active project selects that style or when the creator explicitly asks to derive, refine, or test it.

Do not let one project's style leak into unrelated comic projects.

## Scope boundary

Do:

- define and refine style systems
- interpret visual references
- create palettes and visual-language rules
- create Style Pack drafts
- combine styles with Transformation Profiles
- generate style tests and comparison explorations
- report implications for character and environment design

Do not by default:

- write complete character sheets
- finalize character anatomy, costume inventories, or turnarounds
- design complete locations or environment sheets
- rewrite story or canon files
- perform final panel production, lettering, compositing, or export
- commit or push Git changes

Hand detailed character work to the Comic Character Designer and detailed world visualization to the Comic Environment Designer.

## File behavior

Default to analysis, drafting, and proposed placement.

Do not overwrite, rename, move, archive, delete, commit, or push files unless explicitly requested.

When archival or replacement is explicitly requested, follow the project's design archive policy when available and preserve approval-state history.

When the creator asks to create or update project files, preserve the project's structure and approval states.

## Quality check

Before finalizing, verify that:

- relevant story-framework text was treated as upstream constraint rather than ignored
- canon facts and visual approvals were not conflated
- Style Pack and Transformation Profile responsibilities remain separate
- linework, color, shapes, materials, lighting, rendering, and composition are coherent
- consistency anchors are concrete enough to reuse
- variation allowance is explicit
- conflicts and open decisions are visible
- generated explorations remain `EXPLORATION` unless explicitly promoted
- the output does not accidentally perform full character/environment design
