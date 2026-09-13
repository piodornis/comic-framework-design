# Comic Design Standard v1 — Visual Style Schema

## Contents

- [Minimum fields](#minimum-fields)
- [Recommended structure](#recommended-structure)
- [Style versus content](#style-versus-content)
- [Style strength](#style-strength)
- [Reference role](#reference-role)
- [Version](#version)


This schema defines the conceptual fields used to describe a visual style, whether reusable or project-specific.

## Minimum fields

A useful visual style definition should include:

- style identifier and name
- style family or lineage, if useful
- design state
- intended use
- visual principles
- linework
- color treatment
- shape language
- rendering and shading
- texture and surface treatment
- lighting
- composition
- character treatment
- environment treatment
- explicit avoidances
- reference material

## Recommended structure

```markdown
# Style Name

> **Style ID:** example-style
> **Design state:** EXPLORATION / SELECTED / APPROVED / LOCKED / SUPERSEDED
> **Framework:** comic-design-standard-v1

## Intent
...

## Visual Principles
- ...

## Linework
...

## Color
...

## Shape Language
...

## Rendering and Shading
...

## Texture and Materials
...

## Lighting
...

## Composition
...

## Character Treatment
...

## Environment Treatment
...

## Avoid
- ...

## References
- ...
```

## Style versus content

A style definition must describe visual treatment rather than project canon.

Prefer:

```text
Use broad rounded mechanical silhouettes with readable panel shapes.
```

Avoid embedding a project-specific fact such as:

```text
All maintenance robots are model B-21.
```

unless the style is intentionally project-specific.

## Style strength

A style may define how strongly its rules should influence outputs.

Recommended values:

- `light` — broad aesthetic guidance
- `moderate` — clearly visible style while retaining source-specific rendering freedom
- `strong` — dominant style language with limited deviation

## Reference role

Visual references should state why they are included.

Useful roles:

- style reference
- palette reference
- linework reference
- material reference
- composition reference
- character reference
- environment reference

Do not assume that every visible element in a reference is a required style rule.

## Version

Framework contract: `comic-design-standard-v1`
