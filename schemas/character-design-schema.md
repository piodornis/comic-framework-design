# Comic Design Standard v1 — Character Design Schema

## Contents

- [Recommended location](#recommended-location)
- [Story linkage and asset ownership](#story-linkage-and-asset-ownership)
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

## Story linkage and asset ownership

Use the same `<character-id>` as `characters/<character-id>/profile.md`. Link this narrative source from `design.md`, and link the design record from the profile. The profile retains narrative authority; the design record retains visual authority. A visual proposal does not fill an `OPEN` narrative field automatically.

Keep images, available generation prompts and asset provenance in this record's `references/` directory. Do not duplicate visual files in the Story character directory. Missing images or original prompts should be recorded explicitly, not fabricated. Optional character/design indexes link to these records rather than duplicating their contents.

Generic body-type or ensemble studies are not automatically named characters. They may use a clearly labelled study directory or the project's shared `design/references/` convention without an invented narrative profile.

Preserve established project paths unless reorganization is requested. For an authorized move, update active references, preserve image bytes and approval states, and record old/new paths with checksums where useful. Preserve original prompt and provenance records as historical evidence; a migration map may resolve their old paths. A later filename or a directory change does not select or approve a variant.

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
