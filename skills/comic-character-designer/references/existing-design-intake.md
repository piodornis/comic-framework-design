# Existing Design Intake

## Contents

- [Purpose](#purpose)
- [Accepted draft types](#accepted-draft-types)
- [Intake sequence](#intake-sequence)
- [Reference roles](#reference-roles)
- [Preservation matrix](#preservation-matrix)
- [Multiple drafts](#multiple-drafts)
- [Refinement rules](#refinement-rules)
- [Real-person source material](#real-person-source-material)
- [Revision reporting](#revision-reporting)

## Purpose

Use existing designs as first-class project evidence rather than treating every character task as greenfield generation.

A supplied draft may be more authoritative than a textual description, or it may merely be an exploration. Determine its role before changing it.

## Accepted draft types

Accept:

- rough sketches
- polished illustrations
- character sheets
- turnarounds
- expression sheets
- costume studies
- 3D renders
- screenshots
- photos
- AI-generated concepts
- annotated images
- text descriptions of prior visual decisions

## Intake sequence

For each supplied draft:

1. identify the subject
2. identify design state if known
3. identify whether the image is current or historical
4. assign one or more reference roles
5. extract intended anchors
6. note uncertain or incidental details
7. compare against narrative canon
8. compare against the active Style Pack
9. record conflicts before revision

If design state is unstated, default to `EXPLORATION`.

## Reference roles

Use roles compatible with the framework visual-reference schema, including:

- `IDENTITY_REFERENCE`
- `POSE_REFERENCE`
- `COMPOSITION_REFERENCE`
- `COSTUME_REFERENCE`
- `STYLE_REFERENCE`
- `PALETTE_REFERENCE`
- `LINEWORK_REFERENCE`
- `MATERIAL_REFERENCE`
- `PROP_REFERENCE`
- `LIGHTING_REFERENCE`

Do not assume that every visible property in a reference is intended to survive.

## Preservation matrix

For important traits, classify preservation strength:

- `STRICT`
- `HIGH`
- `MODERATE`
- `FLEXIBLE`

Example:

```text
face geometry        STRICT
main silhouette      HIGH
coat color            HIGH
background            FLEXIBLE
lighting              FLEXIBLE
pose                   MODERATE
```

Use explicit creator instructions over inferred preservation strength.

## Multiple drafts

When multiple drafts exist, build a comparison before merging.

Track:

- common traits shared by all drafts
- traits unique to one draft
- direct contradictions
- likely accidental generation drift
- approved or locked features

Possible outcomes:

- preserve one draft as the master
- select traits from several drafts with explicit justification
- keep alternatives separate
- request a creator decision

Never average contradictory face, body, costume, or marking details automatically.

## Refinement rules

Before an image edit or new derivative, state internally which properties must stay fixed and which may change.

Prefer targeted changes over total regeneration when the existing draft already solves most of the design problem.

Examples:

- keep face and body, revise costume only
- preserve costume, improve proportions
- preserve silhouette, adapt rendering to a new Style Pack
- preserve identity, generate missing side and rear views

Do not replace a recognizable existing design merely because a different concept is visually attractive.

## Real-person source material

When photos of real people are used:

- treat them as visual references or transformation sources
- preserve only task-relevant observable appearance and user-provided facts
- do not infer sensitive attributes from appearance
- distinguish the real person's appearance from fictional character traits added by the project
- use a Transformation Profile when the task is a systematic photo-to-comic conversion

If a fictional costume, scar, insignia, or other story-bearing feature is added, treat the implied story fact as `PROPOSAL` unless already established.

## Revision reporting

After refining an existing design, report:

- preserved anchors
- changed elements
- unresolved differences
- new proposals
- any canon conflicts
- resulting design state
- recommended next artifact or review step
