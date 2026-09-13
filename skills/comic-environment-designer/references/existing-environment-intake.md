# Existing Environment Intake

## Contents

- [Purpose](#purpose)
- [Default assumption](#default-assumption)
- [Intake sequence](#intake-sequence)
- [Reference roles](#reference-roles)
- [Preservation strengths](#preservation-strengths)
- [Geometry versus mood](#geometry-versus-mood)
- [Multiple drafts](#multiple-drafts)
- [Photos and real locations](#photos-and-real-locations)
- [Refinement brief](#refinement-brief)
- [Do not overwrite source intent](#do-not-overwrite-source-intent)

## Purpose

Use this guide whenever the user supplies an existing environment design, photo, architectural sketch, map, floor plan, location sheet, prop concept, or earlier generated image.

## Default assumption

Treat supplied work as intentional source material.

Do not replace it with a new design merely because a different solution appears more polished.

If status is unknown, treat it as `EXPLORATION`.

## Intake sequence

Before redesigning, identify:

1. source artifact and date/version when known
2. design state
3. intended reference role
4. fixed anchors
5. flexible dimensions
6. known problems
7. story-side constraints
8. active Style Pack
9. requested outcome

If the user only asks for a small revision, do not expand the scope unnecessarily.

## Reference roles

Map supplied material to explicit roles when possible:

- `ENVIRONMENT_REFERENCE`
- `COMPOSITION_REFERENCE`
- `MATERIAL_REFERENCE`
- `PALETTE_REFERENCE`
- `LIGHTING_REFERENCE`
- `PROP_REFERENCE`
- `STYLE_REFERENCE`

A floor plan may serve spatial continuity without being a style reference. A mood image may guide atmosphere without defining geometry.

## Preservation strengths

Use these levels when helpful:

- `STRICT` — preserve exactly unless impossible
- `HIGH` — preserve identity; minor cleanup allowed
- `MODERATE` — preserve the general relationship or motif
- `FLEXIBLE` — use as inspiration only

Apply strengths to individual traits, not only to the whole image.

Example:

```text
STRICT: entrance position, central turbine, floor levels
HIGH: major material system, skyline silhouette
MODERATE: signage density
FLEXIBLE: props, weather, local clutter
```

## Geometry versus mood

Record whether the source is authoritative for:

- geometry
- atmosphere
- both
- neither

Do not infer spatial layout from a cinematic single-angle image unless the project accepts that interpretation.

Likewise, do not discard a useful spatial diagram because it lacks visual style.

## Multiple drafts

When several drafts exist, compare them rather than blending them automatically.

Create a short matrix when useful:

| Trait | Draft A | Draft B | Status |
| --- | --- | --- | --- |
| Main entrance | left wall | central | conflict |
| Central landmark | turbine | turbine | stable |
| Floor count | two | three | conflict |
| Palette | cool | cool | stable |

Resolve only with explicit creator instruction or clear source priority.

## Photos and real locations

When using photos:

- distinguish observable visual facts from project invention
- preserve only the features relevant to the task
- use a Transformation Profile when the task is a transformation rather than redesign
- do not infer sensitive traits about people visible in the image
- do not treat incidental signage, branding, or private information as desired design content unless requested and appropriate

If the creator wants a fictionalized location inspired by a real place, identify which features should remain recognizable and which should be transformed.

## Refinement brief

Before substantial edits, summarize the working brief:

```text
Source: existing location concept
Design state: SELECTED
Preserve strictly: layout, entry bridge, central shaft
Preserve highly: concrete/steel material logic, scale
Flexible: signage, secondary props, light color
Change requested: improve style fit and add reverse angle
Story constraints: no new security technology
```

Use this brief to prevent accidental drift.

## Do not overwrite source intent

When a refinement produces a new derivative:

- preserve the source artifact
- keep the new result separate
- state what changed
- state what remained fixed
- keep the derivative at `EXPLORATION` unless the creator promotes it
- recommend `SUPERSEDED` only after replacement is intentional
