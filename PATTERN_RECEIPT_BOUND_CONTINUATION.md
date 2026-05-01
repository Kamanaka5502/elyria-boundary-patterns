# Pattern — Receipt-Bound Continuation

## Risk condition

A system continues execution without proving that prior steps were valid.

## Boundary question

Is continuation allowed based on a valid, replayable receipt from the prior step?

## Admissibility check

- prior receipt exists
- receipt integrity holds
- receipt matches current state assumptions
- continuation does not violate invariants

## Lawful outcomes

- EXECUTE — if receipt validates continuation
- REFUSE — if receipt is missing or invalid
- HALT — if receipt cannot be reconciled with current state

## Proof artifact

- receipt chain
- parent-child linkage between actions
- replay reproduces identical continuation outcome

## Private layer not exposed

- receipt signing mechanism
- chain validation logic
- state reconciliation internals
