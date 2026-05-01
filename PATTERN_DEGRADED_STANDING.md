# Pattern — Degraded Standing

## Risk condition

An actor or system continues to operate even though its standing has partially degraded.

## Boundary question

Is the actor’s standing still sufficient to allow consequence to bind?

## Admissibility check

- current standing level
- required standing for requested action
- evidence supporting standing
- drift or decay in standing over time

## Lawful outcomes

- EXECUTE — if standing remains sufficient
- ESCALATE — if standing is degraded but recoverable
- REFUSE — if standing falls below admissible threshold

## Proof artifact

- standing snapshot in receipt
- degradation marker
- replay shows same degradation leads to same outcome

## Private layer not exposed

- standing scoring model
- decay functions
- authority derivation logic
