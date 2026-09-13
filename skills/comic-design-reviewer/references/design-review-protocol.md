# Design Review Protocol

## Contents

- [1. Review objective](#1-review-objective)
- [2. Establish the requirement set](#2-establish-the-requirement-set)
- [3. Reference roles](#3-reference-roles)
- [4. Review dimensions](#4-review-dimensions)
- [5. Existing-design fidelity](#5-existing-design-fidelity)
- [6. Transformation fidelity](#6-transformation-fidelity)
- [7. Character continuity](#7-character-continuity)
- [8. Environment continuity](#8-environment-continuity)
- [9. Cross-design cohesion](#9-cross-design-cohesion)
- [10. Repeatability](#10-repeatability)
- [11. Evidence and uncertainty](#11-evidence-and-uncertainty)
- [12. Severity calibration](#12-severity-calibration)
- [13. Approval readiness](#13-approval-readiness)
- [14. Review anti-patterns](#14-review-anti-patterns)

## 1. Review objective

Evaluate whether a design artifact faithfully satisfies its governing constraints and can function as a stable visual reference for future work.

Do not confuse subjective preference with a defect. A finding should connect to at least one of:

- canon or creator requirement
- design-state rule
- Style Pack rule
- Transformation Profile rule
- declared preservation anchor
- continuity requirement
- repeatability requirement
- production-readiness requirement

## 2. Establish the requirement set

Before judging the artifact, identify the strongest applicable sources.

Create an internal checklist of:

- locked or approved visual anchors
- explicit creator instructions
- narrative canon constraints
- active Style Pack rules
- active Transformation Profile rules
- selected references and their roles
- artifact-specific requirements
- expected design state

If governing sources disagree, report the conflict instead of inventing a compromise.

## 3. Reference roles

Treat references by role rather than as undifferentiated inspiration.

Common roles:

- identity
- silhouette
- proportions
- anatomy or mechanical construction
- costume or shell structure
- palette
- material
- texture
- linework
- rendering
- lighting
- pose
- expression
- spatial layout
- architecture
- signage
- atmosphere
- composition
- general inspiration

One image may serve several roles, but do not assume every visible property is binding.

## 4. Review dimensions

### Canon fit

Check whether the visual result contradicts explicit narrative facts or implies unsupported facts.

Examples:

- wrong age or physical state
- technology not established in the world
- faction insignia without canon support
- damage that implies an unrecorded event
- inaccessible architecture that contradicts story staging

### Design-state correctness

Check whether artifacts are labeled consistently with creator decisions.

Examples:

- an exploratory draft presented as approved
- a superseded reference still treated as current
- a locked design altered without authorization

### Style compliance

Check system-level adherence to the active visual language.

Review line, shape, color, materials, rendering, lighting, detail density, texture, and graphic language as applicable.

### Readability

Check whether important silhouettes, expressions, props, landmarks, and visual hierarchies remain legible at expected comic scale.

### Production usefulness

Check whether the design contains enough stable information for recurring depiction without requiring invention on every panel.

## 5. Existing-design fidelity

When a revision is based on an existing design, compare the result to declared preservation strengths.

### STRICT

Any unapproved change is normally `BLOCKING` if it affects identity or locked requirements.

### HIGH

Material changes are usually `MAJOR` unless clearly justified.

### MODERATE

Allow controlled reinterpretation while preserving recognizable design logic.

### FLEXIBLE

Variation is allowed as long as higher-order requirements remain satisfied.

Do not elevate incidental details from an exploratory reference into mandatory anchors without evidence.

## 6. Transformation fidelity

When a Transformation Profile applies, separate source fidelity from visual style.

For `photo-to-comic`, typical preservation checks may include:

- subject count
- recognizable identity when requested
- pose and gesture
- clothing structure
- important objects
- composition
- scene layout

The Style Pack may legitimately change:

- linework
- color treatment
- shading
- rendering
- texture simplification
- stylized proportions within profile limits

A style change is not automatically a fidelity failure.

For photos containing real people, restrict evaluation to observable, task-relevant visual features. Do not infer personality, ethnicity, health, religion, sexuality, political affiliation, or other sensitive/private traits from appearance.

## 7. Character continuity

For recurring character designs, compare stable anchors across views and variants.

Check:

- silhouette
- height and width relationships
- head-to-body ratio
- face/display geometry
- eye placement and shape
- distinctive marks
- palette blocks
- costume panels or shell construction
- limb and joint structure
- equipment attachment points
- repeated wear/damage patterns when approved
- front/side/back geometry

Distinguish pose perspective from actual proportion drift.

For expressive variants, allow deformation that preserves identity unless the style explicitly forbids it.

## 8. Environment continuity

Check whether recurring spaces can be reconciled into one plausible layout.

Check:

- entry/exit positions
- door and window relationships
- major levels
- stairways, lifts, bridges, corridors
- recurring furniture and machinery
- landmark placement
- directional signage
- relative scale
- sight lines needed by the story
- exterior/interior relationship

Atmosphere may vary by time, weather, lighting, or story beat. Geometry should not vary accidentally.

## 9. Cross-design cohesion

Compare characters, environments, props, and visual systems together.

Check:

- shared shape-language logic
- compatible technology level
- coherent material vocabulary
- scale relationships
- faction or institutional visual systems
- palette interaction
- signage and interface consistency
- whether character equipment appears designed for the same world

Do not require identical styling across every object. Cohesion allows controlled hierarchy and variation.

## 10. Repeatability

A visually attractive image may still be a weak design reference.

Ask whether another competent artist or model could reproduce the same identity from the available information.

Potential repeatability weaknesses:

- only one ambiguous view
- inconsistent proportions across references
- unclear back or side construction
- hidden attachment logic
- unresolved materials
- no scale anchor
- environment geometry only suggested through mood paintings
- style rules too vague to distinguish intended from accidental traits

Classify missing repeatability information according to its likely downstream cost.

## 11. Evidence and uncertainty

Use three evidence levels internally:

- **Observed** — directly visible or explicitly documented
- **Supported inference** — follows reasonably from multiple sources
- **Unverified** — cannot be confirmed with supplied material

Do not present supported inference as direct observation.

When evidence is missing, state what artifact or view would resolve the question.

## 12. Severity calibration

### BLOCKING

Use when approval or locked-design consistency is impossible without correction.

Examples:

- contradicts locked identity-critical geometry
- violates explicit canon requirement
- transformation loses the required subject identity
- environment geometry makes a required story action impossible

### MAJOR

Use when the issue materially weakens identity, style coherence, continuity, or repeatability.

Examples:

- side view changes character body construction
- recurring location changes entrance placement
- major palette or linework system violates active Style Pack
- selected reference roles are ignored

### MINOR

Use for local inconsistencies that do not threaten the design system.

Examples:

- one missing accent color
- small prop inconsistency
- isolated line-weight drift

### NOTE

Use for optional refinement, ambiguity, or future documentation needs.

## 13. Approval readiness

Recommend one state:

### NOT_READY

Use when one or more blocking issues exist, or major uncertainties prevent responsible approval.

### READY_WITH_MINOR_FIXES

Use when the design is structurally sound and only minor corrections remain.

### READY_FOR_APPROVAL

Use when no known blocking or material major issue remains and the artifact is documented sufficiently for creator review.

### CONSISTENT_WITH_LOCKED_DESIGN

Use when reviewing a derivative or repeat depiction against an already locked design and no meaningful deviation is found.

Never convert this recommendation into `APPROVED` or `LOCKED` automatically.

## 14. Review anti-patterns

Avoid:

- rewriting the design during review instead of reporting findings
- treating aesthetic preference as objective failure
- demanding all possible views for every early exploration
- using style compliance as an excuse to override locked identity
- averaging conflicting references instead of reporting conflict
- assuming an exploratory image establishes canon
- treating a photorealistic source as a requirement to remain photorealistic after transformation
- declaring production readiness when core views or spatial anchors remain contradictory
- assigning approval without the creator
