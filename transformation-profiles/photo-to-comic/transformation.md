# Transformation Profile — Photo to Comic

## Contents

- [Purpose](#purpose)
- [Accepted Inputs](#accepted-inputs)
- [Preserve](#preserve)
  - [STRICT when explicitly identified by the user or project](#strict-when-explicitly-identified-by-the-user-or-project)
  - [HIGH by default](#high-by-default)
  - [MODERATE by default](#moderate-by-default)
- [Transform](#transform)
- [May Reinterpret](#may-reinterpret)
- [Real People](#real-people)
- [Multi-Image Consistency](#multi-image-consistency)
- [Avoid](#avoid)
- [Output Expectations](#output-expectations)
- [Style-Pack Integration](#style-pack-integration)


> **Profile ID:** `photo-to-comic`
> **Profile version:** 1.0
> **Framework:** `comic-design-standard-v1`

## Purpose

Transform one or more source photographs into comic-design imagery while preserving the source information that makes the subject, pose, clothing, objects, composition, and scene recognizable.

This profile is style-neutral. Combine it with a Style Pack such as `franco-belgian-vivid`, a future manga pack, or a project-specific visual style.

## Accepted Inputs

- portrait photographs
- full-body photographs
- group photographs
- environment photographs
- object or prop photographs
- multiple photographs intended as one visually consistent batch

## Preserve

### STRICT when explicitly identified by the user or project

- identity-defining features
- required costume or uniform elements
- required logos or markings when legally and project-wise appropriate
- story-critical objects
- creator-specified composition constraints

### HIGH by default

- recognizable subject identity
- number of main subjects
- pose and gesture
- clothing and major accessories
- major objects
- overall composition
- spatial relationships between subjects
- understandable scene context

### MODERATE by default

- exact facial micro-texture
- background fine detail
- minor fabric folds
- photographic lighting artifacts
- small incidental objects

## Transform

Apply the selected Style Pack to:

- linework
- color treatment
- shading
- rendering density
- texture
- edge treatment
- visual simplification
- atmospheric effects
- background graphicness

The transformed result should read as intentional comic art rather than a photo with a weak filter.

## May Reinterpret

When compatible with preservation requirements and the selected Style Pack:

- background simplification
- nonessential clutter
- small lighting inconsistencies
- depth-plane separation
- minor pose cleanup
- minor expression simplification

Do not reinterpret a detail when doing so changes a story fact or damages identity fidelity.

## Real People

When photographs contain real people:

- preserve recognizable visual identity when requested
- preserve pose, clothing, and composition according to the stated priority
- do not infer sensitive traits, biography, personality, or identity facts from appearance
- distinguish source-visible details from story or character information supplied separately

If the project turns a real person into a fictional character, keep fictional additions separate from observed source facts.

## Multi-Image Consistency

For a batch:

- use one Style Pack unless explicitly instructed otherwise
- keep linework strength consistent
- keep color intensity and rendering logic consistent
- preserve each source image's individual composition unless a shared redesign is requested
- use stable treatment for repeated people, clothing, props, and locations

When the same person appears across several photographs, treat identity consistency as a high-priority cross-image constraint.

## Avoid

- silently changing the number or identity of subjects
- replacing clothing or important objects without instruction
- adding scars, weapons, insignia, injuries, or other story-significant details without marking them as `PROPOSAL`
- turning recognizable people into unrelated fictional faces
- weak stylization that leaves the result primarily photographic when the task requests a clear comic conversion
- franchise-specific additions not present in the source or project

## Output Expectations

For design exploration, return or document:

- selected Style Pack
- relevant source references
- preservation priorities
- transformation notes
- resulting design state
- any introduced `PROPOSAL`, `CONFLICT`, or `OPEN` points

Generated images may be stored as exploration assets until explicitly promoted to `SELECTED`, `APPROVED`, or `LOCKED`.

## Style-Pack Integration

Example combinations:

```text
photo-to-comic + franco-belgian-vivid
photo-to-comic + manga-clean
photo-to-comic + project-specific-style
```

The Transformation Profile must not duplicate the Style Pack's aesthetic rules.
