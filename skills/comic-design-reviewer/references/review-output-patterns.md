# Review Output Patterns

## Contents

- [Focused review](#focused-review)
- [Comparative review](#comparative-review)
- [Project-wide review](#project-wide-review)
- [Finding format](#finding-format)
- [Clean review format](#clean-review-format)
- [Missing-evidence format](#missing-evidence-format)

## Focused review

Use for one artifact or a small related set.

```markdown
# Design Review — <artifact>

## Scope
- Artifact: <path or description>
- Design state: <state>
- Active Style Pack: <id>
- Transformation Profile: <id or none>
- Governing references: <brief list>

## Readiness
`READY_WITH_MINOR_FIXES`

## Findings

### D-001 — <short title>
- Severity: MAJOR
- Category: Character continuity
- Artifact: <specific view>
- Expected: <requirement>
- Observed: <what is visible>
- Why it matters: <impact>
- Suggested direction: <correction direction, not silent rewrite>
- Canon impact: none / PROPOSAL / CONFLICT / OPEN
- Design-state impact: <e.g. approval should wait>

## Strengths retained
- <requirement that is satisfied>

## Open questions
- <question>
```

## Comparative review

```markdown
# Comparative Design Review

## Candidates
- A: <artifact>
- B: <artifact>

## Governing requirements
- <requirement>

## Comparison
| Criterion | A | B |
| --- | --- | --- |
| Identity fidelity | strong | moderate |
| Style compliance | moderate | strong |
| Repeatability | strong | strong |

## Findings
<finding blocks>

## Recommendation
<only if requested>

State tradeoffs explicitly. Do not mark the recommended candidate APPROVED.
```

## Project-wide review

```markdown
# Project Design Review

## Scope
- Characters reviewed: <n>
- Environments reviewed: <n>
- Style Packs: <ids>
- Transformation Profiles: <ids>

## Overall readiness
`NOT_READY`

## Blocking findings
<finding blocks>

## Major findings
<finding blocks>

## Minor findings
<finding blocks>

## Cross-design observations
- <cohesion or compatibility note>

## Missing coverage
- <missing sheet/view/reference>

## Approval candidates
- <artifact>: READY_FOR_APPROVAL

## Unresolved narrative/design questions
- <question>
```

## Finding format

Use stable identifiers for findings when the review may be repeated.

```markdown
### Finding D-001

- Severity: BLOCKING | MAJOR | MINOR | NOTE
- Category: <review category>
- Artifact: <file, image, view, or component>
- Expected: <governing requirement>
- Observed: <evidence>
- Why it matters: <consequence>
- Suggested direction: <bounded correction guidance>
- Canon impact: none | INFERENCE | PROPOSAL | CONFLICT | OPEN
- Design-state impact: <effect on approval readiness>
```

Keep `Observed` factual. Put interpretation in `Why it matters`.

## Clean review format

When no material problems are found, do not invent findings to fill space.

```markdown
# Design Review — <artifact>

## Readiness
`READY_FOR_APPROVAL`

No blocking, major, or minor findings identified against the supplied requirements.

## Verified
- <locked or approved anchors preserved>
- <Style Pack compliance verified>
- <Transformation Profile fidelity verified, if applicable>
- <repeatability sufficient for current stage>

## Notes
- <optional NOTE-level observation>
```

## Missing-evidence format

Use when the requested review cannot be completed responsibly.

```markdown
## Review limitation

The following cannot be verified with the supplied material:

- Side-view construction — no side view or geometry reference supplied.
- Rear entrance position — no map, reverse angle, or textual constraint supplied.

These are `OPEN` review points, not failures.

Recommended evidence:
- <specific missing reference>
```
