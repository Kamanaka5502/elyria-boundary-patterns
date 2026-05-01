# Pattern — Explicit Continuation Only

## Risk condition

A system proceeds after an invalid or uncertain state without an explicit decision.

## Boundary question

Is any continuation explicitly admitted and justified before it proceeds?

## Admissibility check

- invalid or uncertain state is detected
- explicit decision is required before proceeding
- no silent or implicit continuation occurs

## Lawful outcomes

- HALT — when the system cannot safely proceed
- RESTART — when a new valid state is established
- REFUSE — when continuation would violate constraints

## Proof artifact

- decision marker in receipt
- halt or restart indicator
- replay shows continuation only occurs after explicit decision

## Private layer not exposed

- detection internals
- recovery orchestration
- system state repair logic
