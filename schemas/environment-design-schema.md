# Comic Design Standard v1 — Environment Design Schema

## Contents

- [Recommended location](#recommended-location)
- [Minimum fields](#minimum-fields)
- [Recommended `design.md`](#recommended-designmd)
- [Spatial continuity](#spatial-continuity)
- [World-rule boundary](#world-rule-boundary)
- [Version](#version)


This schema defines visual-design records for locations, architecture, interiors, exteriors, recurring world spaces, props, machinery, and related environmental elements.

## Recommended location

```text
comic-project/design/environments/<environment-id>/
├── design.md
└── references/
```

Project-wide props may live under:

```text
comic-project/design/props/<prop-id>/
```

In v1, the environment-design workflow may handle props, vehicles, machinery, signage, and related visual systems unless a separate specialist becomes necessary.

## Minimum fields

Record:

- environment identifier
- narrative source reference
- canon state of relevant facts
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

## Recommended `design.md`

```markdown
# Environment Design — Environment ID

> **Canon state:** CANON / mixed / draft
> **Design state:** EXPLORATION / SELECTED / APPROVED / LOCKED / SUPERSEDED
> **Style Pack:** ...

## Narrative Source
...

## Function
...

## Visual Concept
...

## Spatial Logic
...

## Scale
...

## Architecture / Structural Language
...

## Palette
...

## Materials and Wear
...

## Lighting and Atmosphere
...

## Landmarks
...

## Props / Machinery
...

## Signage / Graphic Language
...

## Required Views
- ...

## Continuity Anchors
- ...

## Open Design Questions
- ...

## References
- ...
```

## Spatial continuity

Environment concepts should distinguish visual mood from usable spatial logic.

When a location recurs, define enough stable geometry to support consistent staging:

- entrances and exits
- major levels
- recurring furniture or machinery
- dominant landmarks
- sight lines when story-relevant
- relative scale

Do not invent unnecessary architectural detail only to make the document look complete.

## World-rule boundary

If visual design implies a new technology, resource, social convention, or world rule, report the implication instead of silently establishing it.

## Version

Framework contract: `comic-design-standard-v1`
