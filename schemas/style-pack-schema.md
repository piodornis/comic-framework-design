# Comic Design Standard v1 — Style Pack Schema

## Contents

- [Design goals](#design-goals)
- [Recommended location](#recommended-location)
- [Required metadata](#required-metadata)
- [Recommended sections](#recommended-sections)
- [Consistency anchors](#consistency-anchors)
- [Variation allowance](#variation-allowance)
- [What not to include](#what-not-to-include)
- [Versioning](#versioning)
- [Version](#version)


A Style Pack is a reusable visual-language package that can be combined with original design work or a Transformation Profile.

## Design goals

A Style Pack should:

- be independent from one specific comic whenever it is stored in the framework
- describe visual treatment rather than source-preservation behavior
- be usable by character and environment design workflows
- define enough constraints for consistent repeated application
- remain readable without a specific image-generation model

## Recommended location

Framework-reusable pack:

```text
style-packs/<style-id>/
└── style.md
```

Project-specific pack:

```text
comic-project/design/styles/<style-id>/
├── style.md
└── references/
```

## Required metadata

A Style Pack should identify:

- `id`
- human-readable name
- style family
- design state
- style strength
- intended use
- framework contract

## Recommended sections

Use the fields from `visual-style-schema.md` and add:

- compatibility notes
- preferred source types, if relevant
- consistency anchors
- variation allowance
- known failure modes

## Consistency anchors

Define the characteristics that should survive repeated generations or manual redraws.

Examples:

- line weight hierarchy
- palette behavior
- edge treatment
- face simplification level
- shadow geometry
- material rendering
- silhouette readability
- background detail density

## Variation allowance

State which elements may vary without breaking the style.

Examples:

- local accent colors
- hatching density
- atmospheric effects
- panel-specific lighting intensity

## What not to include

Do not include:

- narrative canon unrelated to appearance
- one project's character biographies
- production-tool-specific commands unless the pack explicitly targets that tool
- source-preservation rules that belong in a Transformation Profile

## Versioning

Style Packs may evolve independently from the framework.

Recommended metadata:

```text
Style ID: franco-belgian-vivid
Style version: 1.0
Framework: comic-design-standard-v1
```

When a later version changes the visual identity substantially, preserve the prior version or mark it `SUPERSEDED` according to project needs.

## Version

Framework contract: `comic-design-standard-v1`
