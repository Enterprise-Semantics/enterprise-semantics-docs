# Capability Autonomy Authority Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013

## Authority as a Boundary

Autonomous Capability operates within defined Authority. Unlimited authority must fail conformance per CR-ES-013 §17.

```
Objective
   |
   v
Authority
   |
   v
Policy
   |
   v
Constraints
   |
   v
Governance
   |
   v
Decision / Action
   |
   v
Outcome
   ^
   |
Adaptation (loop)
```

## Authority Properties

The Authority context of an Autonomous Capability defines:

- permitted authority scope
- approval thresholds
- escalation triggers
- decision/action boundaries
- intervention triggers

## ACAP-AUTO-CON-007 (Authority Invariant)

Per CR-ES-013 §9, Autonomous Capability operates within authority. The conformance invariant requires that:

- the Authority context is defined
- decisions/actions outside Authority escalate
- the Capability does NOT proceed when Authority is exceeded

## ACAP-AUTO-NEG-011 (Unlimited Authority Forbidden)

Per CR-ES-013 §10, Autonomous Capability does NOT imply unlimited authority. Authority must be defined, bounded, and enforced. The release gate must fail if Autonomous Capability is encoded as having unlimited authority.

## Escalation Boundary

The escalation boundary defines when control must transfer. Per CR-ES-013 §4:

- intervention_model: human intervention semantics
- escalation_boundary: when control must transfer

When the realization encounters:

- authority exceeded
- policy requires approval
- constraint violation
- ambiguous exception
- human escalation request

The Autonomous Capability must transfer control, not proceed unilaterally.

## See Also

- ADR-ES-013 §3.4
- CR-ES-013 §4, §9, §10, §17
- ACAP-AUTO-CON-007 + ACAP-AUTO-NEG-011 + ACAP-AUTO-CON-012
- architecture/autonomous-capability-boundary.md
- concepts/autonomous-capability.md
