# Comic Design Standard v1 — Design Status

## Contents

- [Two independent status axes](#two-independent-status-axes)
- [EXPLORATION](#exploration)
- [SELECTED](#selected)
- [APPROVED](#approved)
- [LOCKED](#locked)
- [SUPERSEDED](#superseded)
- [Recommended progression](#recommended-progression)
- [Conflict rule](#conflict-rule)
- [Version](#version)


This document defines the approval lifecycle for visual design artifacts in `comic-design-standard-v1`.

Design status is independent from narrative canon status.

## Two independent status axes

Use the story framework's canon states for factual truth:

- `CANON`
- `INFERENCE`
- `PROPOSAL`
- `CONFLICT`
- `OPEN`

Use these design states for visual approval:

- `EXPLORATION`
- `SELECTED`
- `APPROVED`
- `LOCKED`
- `SUPERSEDED`

A design may therefore be both:

```text
Canon state: CANON
Design state: EXPLORATION
```

For example, a character's role may be established canon while their visual appearance is still being explored.

## EXPLORATION

Use for sketches, alternative directions, tests, generated variations, mood studies, and other uncommitted visual ideas.

Exploration is expected to change freely.

Do not treat an exploration image as the definitive appearance of a character or location.

## SELECTED

Use when one direction has been chosen for further development but is not yet formally approved.

A selected design may still require:

- cleanup
- turnaround work
- color refinement
- material definition
- missing views
- continuity clarification
- creator approval

## APPROVED

Use when the creator has explicitly accepted the visual solution as the current project design.

Approved designs should become the preferred reference for future visual work.

Approval does not automatically mean every detail is immutable.

## LOCKED

Use when a design should not be changed without explicit authorization.

Typical uses:

- production has started
- the design appears repeatedly across finished assets
- continuity depends on exact proportions, markings, costume, colors, or props

A Skill may identify problems in a locked design but must not silently revise it.

## SUPERSEDED

Use when an older design has been replaced by a newer selected, approved, or locked design.

Keep superseded material for historical reference when useful, but do not use it as the current design source of truth.

## Recommended progression

```text
EXPLORATION
    │
    ▼
SELECTED
    │
    ▼
APPROVED
    │
    ▼
LOCKED
```

Any prior state may become `SUPERSEDED` after replacement.

Only the creator or an explicitly authorized workflow may promote a design to `APPROVED` or `LOCKED`.

## Conflict rule

If an attractive visual direction contradicts established canon, do not resolve the contradiction through design alone.

Mark the factual issue as `CONFLICT` and keep the visual work at an appropriate design state until the conflict is resolved.

## Version

Framework contract: `comic-design-standard-v1`
