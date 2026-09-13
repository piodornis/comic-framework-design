# Comic Design Standard v1 — Character Design Schema

## Contents

- [Recommended location](#recommended-location)
- [Minimum fields](#minimum-fields)
- [Recommended `design.md`](#recommended-designmd)
- [Character Sheet expectations](#character-sheet-expectations)
- [Canon boundary](#canon-boundary)
- [Version](#version)


This schema defines the visual-design record for a comic character.

Narrative biography remains in the story project's character profile. This record describes how the character is visually represented.

## Recommended location

```text
comic-project/design/characters/<character-id>/
├── design.md
└── references/
```

Possible approved assets may include:

```text
front.png
side.png
back.png
expression-sheet.png
pose-sheet.png
costume-01.png
```

## Minimum fields

Record:

- character identifier
- narrative source reference
- canon state of relevant facts
- design state
- active Style Pack
- design intent
- silhouette
- proportions and scale
- face or display language
- body/form construction
- palette
- materials and surfaces
- clothing or shell components
- markings and identifiers
- accessories and recurring equipment
- expression or emotion system
- pose/body-language guidance
- approved variations
- continuity anchors
- open design questions

## Recommended `design.md`

```markdown
# Character Design — Character ID

> **Canon state:** CANON / mixed / draft
> **Design state:** EXPLORATION / SELECTED / APPROVED / LOCKED / SUPERSEDED
> **Style Pack:** ...

## Narrative Source
...

## Design Intent
...

## Silhouette
...

## Proportions and Scale
...

## Face / Expression System
...

## Body / Form Construction
...

## Palette
...

## Materials and Surface Treatment
...

## Clothing / Shell / Costume
...

## Markings and Identifiers
...

## Accessories and Equipment
...

## Pose and Body Language
...

## Approved Variations
...

## Continuity Anchors
- ...

## Open Design Questions
- ...

## References
- ...
```

## Character Sheet expectations

A mature design may benefit from:

- front, side, and rear views
- scale reference
- neutral pose
- expression set
- hand or manipulator details
- recurring equipment
- costume or module variants
- damage or age states when story-relevant

Do not require every view during early exploration.

## Canon boundary

If design work suggests a new factual trait, keep it separate from the approved visual decision.

Example:

```text
Design proposal: visible repaired crack across the helmet.
Narrative implication: character previously suffered major damage.
```

The visual idea may be attractive, but the implied history remains `PROPOSAL` until accepted.

## Version

Framework contract: `comic-design-standard-v1`
