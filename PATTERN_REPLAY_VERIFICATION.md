# Pattern — Replay Verification

## Risk condition

A system produces outcomes that cannot be reproduced under identical conditions.

## Boundary question

Does the same state, governing field, and input produce the same outcome?

## Admissibility check

- state signature consistency
- governing policy identity
- input equivalence
- receipt integrity

## Lawful outcomes

- EXECUTE — if replay matches
- REFUSE — if mismatch indicates inconsistency
- HALT — if replay cannot be performed

## Proof artifact

- replay result marker (MATCH / MISMATCH)
- receipt linkage
- deterministic outcome record

## Private layer not exposed

- replay engine implementation
- internal hashing and verification methods
- environment normalization logic
