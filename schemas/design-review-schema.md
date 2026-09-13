# Comic Design Standard v1 — Design Review Schema

This schema defines a structured review for character, environment, style, and transformation work.

A design review is read-only by default.

## Review categories

Check as relevant:

- canon fit
- design-state correctness
- Style Pack compliance
- Transformation Profile compliance
- identity or source fidelity
- silhouette/readability
- palette consistency
- linework/rendering consistency
- materials and surface logic
- character continuity
- environment continuity
- cross-design cohesion
- repeatability across future images
- missing required views or references
- unintended narrative implications

## Severity

Use:

- `BLOCKING` — prevents approval or contradicts a locked/canon requirement
- `MAJOR` — materially weakens consistency or repeatability
- `MINOR` — local issue worth correcting
- `NOTE` — observation, optional improvement, or future consideration

Severity does not replace canon or design status.

## Recommended finding format

```markdown
### Finding D-001

- Severity: MAJOR
- Category: Style compliance
- Artifact: character-b21/front-view
- Expected: bold clean outer contours with simplified interior linework
- Observed: painterly soft edges dominate the silhouette
- Why it matters: the character no longer matches the active Style Pack
- Suggested direction: restore contour hierarchy without changing the approved proportions
- Canon impact: none
- Design-state impact: approval should wait
```

## Review summary

Conclude with:

- overall readiness
- blocking findings
- major findings
- minor findings
- approval recommendation
- unresolved canon or design questions

Recommended approval recommendations:

- `NOT_READY`
- `READY_WITH_MINOR_FIXES`
- `READY_FOR_APPROVAL`
- `CONSISTENT_WITH_LOCKED_DESIGN`

The reviewer recommends; the creator approves.

## Version

Framework contract: `comic-design-standard-v1`
