# Pattern — Privileged Access Boundary

## Risk condition

A user, model, service, or automated process attempts a high-privilege action that could bind consequence.

## Boundary question

Does the actor have valid authority, current standing, admissible scope, and sufficient evidence to complete the action?

## Admissibility check

- actor identity is known
- authority is current
- requested action is within declared scope
- evidence is fresh enough to support the transition
- policy does not prohibit the action
- receipt can be emitted before consequence binds

## Lawful outcomes

- EXECUTE — if authority, scope, evidence, and policy hold
- REFUSE — if authority or policy fails
- ESCALATE — if authority is unclear or evidence is incomplete
- REDIRECT — if the request can be repaired before binding

## Proof artifact

- intent receipt for every evaluation
- effect receipt only for EXECUTE
- replay condition: same authority, state, policy, and input must reproduce the same outcome

## Private layer not exposed

- production authority resolver
- private policy thresholds
- identity and signing infrastructure
- customer-specific access policy
