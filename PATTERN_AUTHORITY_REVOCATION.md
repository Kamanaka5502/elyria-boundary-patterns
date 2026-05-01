# Pattern — Authority Revocation

## Risk condition

Authority changes after a decision is prepared but before consequence binds.

## Boundary question

Does the actor still have valid authority at the moment of binding?

## Admissibility check

- authority state at evaluation
- authority state at commit boundary
- revocation signals between evaluation and execution
- policy response to revocation

## Lawful outcomes

- REFUSE — if authority has been revoked
- HALT — if revocation occurs mid-transition
- EXECUTE — only if authority remains valid at commit

## Proof artifact

- receipt includes authority state snapshot
- replay verifies revocation produces refusal

## Private layer not exposed

- revocation propagation timing
- authority resolution logic
- internal policy graph
