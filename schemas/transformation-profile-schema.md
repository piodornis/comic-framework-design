# Comic Design Standard v1 — Transformation Profile Schema

A Transformation Profile defines how existing source material should be interpreted and preserved while it is converted into a new visual treatment.

It does not define the visual style itself.

## Core principle

Separate:

```text
source handling → Transformation Profile
visual language → Style Pack
```

This allows one profile to work with many visual styles.

## Required fields

A Transformation Profile should define:

- profile identifier and name
- accepted source types
- preservation priorities
- transformable properties
- optional reinterpretation areas
- forbidden or high-risk changes
- multi-source consistency rules
- output expectations
- compatibility with Style Packs

## Recommended structure

```markdown
# Transformation Profile Name

> **Profile ID:** example-profile
> **Framework:** comic-design-standard-v1

## Purpose
...

## Accepted Inputs
- ...

## Preserve
- ...

## Transform
- ...

## May Reinterpret
- ...

## Avoid
- ...

## Multi-Image Consistency
- ...

## Output Expectations
- ...

## Style-Pack Integration
- ...
```

## Preservation strength

A profile may classify preservation requirements as:

- `STRICT` — change only when explicitly requested
- `HIGH` — preserve unless technically impossible or visually contradictory
- `MODERATE` — retain recognizability while allowing stylization
- `FLEXIBLE` — may change to support the design goal

## Real-person references

When the source contains real people, describe only visually observable or user-provided design information.

Do not invent identity facts or sensitive personal attributes from appearance.

A transformation profile may preserve recognizable visual identity, pose, clothing, and composition without making claims about the person's background or traits.

## New facts introduced by transformation

A visually useful addition may accidentally imply a new story fact.

Examples:

- adding a scar
- changing a uniform insignia
- adding a weapon
- removing a mobility aid

Treat such additions as `PROPOSAL` or `CONFLICT` where appropriate rather than silently establishing them.

## Version

Framework contract: `comic-design-standard-v1`
