# Comic Design Standard v1 - Design Project Structure

## Contents

- [Purpose](#purpose)
- [Project entry points](#project-entry-points)
- [Recommended project layout](#recommended-project-layout)
- [Source-of-truth boundaries](#source-of-truth-boundaries)
- [Read order](#read-order)
- [Story-to-design handoff](#story-to-design-handoff)
- [Design-to-production handoff](#design-to-production-handoff)
- [Focused versus project-wide work](#focused-versus-project-wide-work)
- [File behavior](#file-behavior)
- [Migration and compatibility](#migration-and-compatibility)
- [Version](#version)

This document defines the project-level structure and handoff rules for design work compatible with `comic-design-standard-v1`.

## Purpose

Keep narrative truth, visual design decisions, and later production work connected without making one framework responsible for all three layers.

The comic project repository remains the source of truth for project-specific material.

The design framework adds a design layer to that repository rather than creating a second competing project model.

## Project entry points

Use two complementary entry points when both are present:

- `project.md` - narrative/project source of truth and the entry point for story-side constraints
- `design-project.md` - active design configuration and the entry point for visual-development state

For design work, inspect both when they are available and relevant.

Do not let `design-project.md` override narrative canon established by `project.md` or other higher-priority story records.

Do not let `project.md` silently replace an explicitly approved or locked visual design unless the project records a deliberate change.

## Recommended project layout

A combined comic project may use:

```text
comic-project/
├── project.md
├── canon/
├── characters/
├── relationships/
├── locations/
├── factions/
├── story/
├── issues/
├── style/
├── design-project.md
└── design/
    ├── styles/
    ├── characters/
    ├── environments/
    ├── props/
    ├── references/
    └── archive/
```

The exact story-side folders may vary when the project intentionally uses another compatible structure.

## Character records across layers

For each named character, use matching IDs in `characters/<character-id>/profile.md` and `design/characters/<character-id>/design.md`; visual assets and available prompts belong in `design/characters/<character-id>/references/`. Link both records to each other, and avoid duplicate asset copies. See [Character Design Schema](character-design-schema.md) for ownership, missing references and migration guidance.

This is a recommended combined layout, not a requirement to migrate existing projects. Story-only projects may keep their visual references with their character profiles. Generic type studies need no invented individual character profile.

## Source-of-truth boundaries

Use the story/project layer for facts such as:

- who a character is
- what exists in the world
- relationships and history
- required locations or objects
- plot requirements
- issue and storyboard intent

Use the design layer for visual decisions such as:

- active Style Packs
- Transformation Profiles
- approved appearance
- silhouette and proportion anchors
- palettes and materials
- environment geometry
- visual references
- design approval state

A visual choice that creates a new factual claim remains `PROPOSAL`, `INFERENCE`, `OPEN`, or `CONFLICT` until resolved through the project's narrative process.

## Read order

For a project-wide design task, use this default order unless the project defines another precedence:

1. `project.md`
2. `design-project.md`
3. relevant canon, character, world, location, issue, or storyboard sources
4. approved or locked design records
5. selected project design and visual references
6. active reusable Style Packs and Transformation Profiles
7. current exploration material

For a focused task, read only the smallest subset required to establish the relevant constraints.

When two high-priority sources disagree, report `CONFLICT` rather than merging them silently.

## Story-to-design handoff

Story material should provide constraints rather than finished visual solutions unless a visual fact is already established.

A handoff may include:

- character role and physical facts
- relationship or status cues that should be visually legible
- world rules and technology
- location function and spatial requirements
- recurring props or equipment
- story tone
- script and storyboard needs
- explicit visual canon

The design workflow may propose visual solutions for these constraints but must not silently rewrite narrative truth.

## Design-to-production handoff

The design layer should hand production enough approved or locked material to reproduce the intended visual identity consistently.

A production handoff may include:

- active Style Pack and version
- active Transformation Profile, when relevant
- approved or locked character designs
- approved or locked environment designs
- prop and equipment references
- continuity anchors
- visual-reference roles and preservation strengths
- unresolved design questions that production must not guess about

Production should not treat `EXPLORATION` or `SELECTED` material as final unless explicitly authorized.

## Focused versus project-wide work

A focused task may concern one character, one location, one Style Pack, one source photo, or one design revision.

A project-wide task may establish or review the visual system across the complete project.

Do not mechanically read the complete repository for every focused request.

Do inspect both entry points before broad design changes that may affect multiple areas.

## File behavior

Default to non-destructive work.

Do not silently:

- overwrite approved or locked files
- rename or move design records
- delete or archive prior versions
- change approval states
- commit or push Git changes

Follow `design-archive-policy.md` when archival or replacement work is explicitly requested.

## Migration and compatibility

When a project already has a design structure, preserve it when practical.

Do not automatically migrate files into this layout.

If a structural migration would improve compatibility, propose the migration and identify affected paths before making changes.

## Version

Framework contract: `comic-design-standard-v1`
