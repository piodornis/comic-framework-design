# Comic Design Standard v1 — Visual Reference Schema

This schema defines how visual references should be documented so Skills know what each reference is meant to influence.

## Why reference roles matter

A single image may contain many unrelated visual properties.

Do not assume that everything visible in a reference should be copied or preserved.

Assign an explicit role.

## Recommended roles

- `IDENTITY_REFERENCE` — preserve recognizable subject identity or design identity
- `POSE_REFERENCE` — preserve or study pose and body language
- `COMPOSITION_REFERENCE` — preserve or study framing and spatial arrangement
- `COSTUME_REFERENCE` — preserve or study clothing or costume
- `STYLE_REFERENCE` — guide visual language
- `PALETTE_REFERENCE` — guide color relationships
- `LINEWORK_REFERENCE` — guide contour and ink treatment
- `MATERIAL_REFERENCE` — guide surface rendering
- `ENVIRONMENT_REFERENCE` — guide architecture, spatial mood, or location details
- `PROP_REFERENCE` — guide object construction
- `LIGHTING_REFERENCE` — guide light direction, contrast, or atmosphere

A reference may have more than one role when stated explicitly.

## Recommended metadata

```markdown
# Reference Record

- File: ...
- Subject: ...
- Role: IDENTITY_REFERENCE
- Preservation strength: STRICT / HIGH / MODERATE / FLEXIBLE
- Applies to: ...
- Do use: ...
- Do not infer: ...
- Rights / provenance notes: optional
- Notes: ...
```

## Preservation scope

Specify the exact properties that matter.

Example:

```text
Role: IDENTITY_REFERENCE
Do use: facial structure, hairstyle, glasses, approximate age presentation
Do not use: background, lighting, color grade
```

## Real-person references

For photographs of real people:

- preserve only the characteristics required by the design task
- do not infer sensitive traits from appearance
- distinguish observed appearance from user-provided character information
- record consent or usage-rights notes when the project needs that information

## Reference priority

When references disagree, use this order unless the project defines another rule:

1. locked or approved project design
2. explicit creator instruction
3. selected project reference
4. current exploration reference
5. general inspiration reference

Report unresolved contradictions as `CONFLICT` rather than blending them silently.

## Version

Framework contract: `comic-design-standard-v1`

## Previous comics and production examples

When a supplied comic page or layout file is a reference, state the precise visual properties to study and those not to inherit. Existing reference roles with a narrow `Applies to`/`Do use` scope are sufficient; do not invent a universal layout-reference approval state. Print settings, font availability and page dimensions require separate Production verification. See [Design inputs for page production](production-handoff.md).

## Current construction references and superseded studies

For props with an evolution folder, identify the active construction reference and exact version, plus superseded/rejected studies that must not guide new panels. Directory recency or a visually attractive sketch does not override an explicit selection. Separate mechanical construction from scene staging and general style references.

Record which dimensions and attachments remain fixed, which parts may rotate/translate, and which features should become occluded in each view. If references conflict, identify the affected property and scope rather than averaging incompatible constructions. A creator-directed change is recorded as a new decision; it does not silently rewrite historical approval evidence.
