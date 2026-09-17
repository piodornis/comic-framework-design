# Design Project

## Framework compatibility

- Story/project standard: `comic-project-standard-v1`
- Design standard: `comic-design-standard-v1`

## Project

- Title:
- Design phase: Exploration
- Primary language:

## Project entry points

- Narrative/project entry point: `project.md` (when present)
- Design entry point: `design-project.md`

For design work, read both when they are available and relevant. `project.md` governs narrative/project truth; `design-project.md` governs the active visual configuration and design-layer state. Do not use the design layer to silently override narrative canon.

## Active visual configuration

- Primary Style Pack:
- Secondary Style Pack, if any:
- Transformation Profile, if any:

## Approval policy

Use canon states:

- CANON
- INFERENCE
- PROPOSAL
- CONFLICT
- OPEN

Use design states:

- EXPLORATION
- SELECTED
- APPROVED
- LOCKED
- SUPERSEDED

Only the creator or an explicitly authorized workflow may promote work to `APPROVED` or `LOCKED`.

## Design paths

```text
design/
├── styles/
├── characters/
├── environments/
├── props/
├── references/
└── archive/
```

Follow the framework's `design-archive-policy.md` for superseded or historically retained design artifacts. Do not move material into `design/archive/` without explicit authorization.

## Character linkage

- Narrative profile: `characters/<character-id>/profile.md`.
- Visual record: `design/characters/<character-id>/design.md`.
- Images, available prompts and provenance: `design/characters/<character-id>/references/`.

Use identical IDs and reciprocal links. Keep one authoritative visual asset copy; do not mirror it in the Story directory. Record missing references explicitly. Shared type studies can have a study record without an invented named character. Document existing alternate paths rather than silently moving assets or changing approval states.

## Project-specific style notes

Add only project-specific rules here. Reusable visual-language rules belong in a Style Pack.

## Open design questions

- ...

## Optional page-production handoff

- Production entry point, when adopted: OPEN
- References/revisions and visual approval scope for the current handoff: OPEN
- Artwork/lettering separation and intentional in-world text exceptions: OPEN
- Protected image details, crop constraints and reserved text areas: OPEN
- Prior comic/layout example and its limited reference role, if any: OPEN

Final text, typography, native layout and printer parameters remain with their Story/Production owners. These notes do not imply production readiness or approval of an example's entire style.
