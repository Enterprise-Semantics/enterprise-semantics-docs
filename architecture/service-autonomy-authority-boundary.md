# Service Autonomy Authority Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Authority as a Boundary

Autonomous Service operates within defined Authority. Unlimited authority must fail conformance per CR-ES-015 §18.

```
Service Objective
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
Service Contract
   |
   v
Decision / Action
   |
   v
Service Outcome
   ^
   |
Adaptation (loop)
```

## Authority Properties

The Authority context of an Autonomous Service defines:

- permitted authority scope
- approval thresholds
- escalation triggers
- decision/action boundaries
- intervention triggers

## ASVC-AUTO-CON-008 (Authority Invariant)

Per CR-ES-015 §10, Autonomous Service operates within authority. The conformance invariant requires that:

- the Authority context is defined
- decisions/actions outside Authority escalate
- the Service does NOT proceed when Authority is exceeded

## ASVC-AUTO-NEG-012 (Unlimited Authority Forbidden)

Per CR-ES-015 §11, Autonomous Service does NOT have unlimited authority. Authority must be defined, bounded, and enforced. The release gate must fail if Autonomous Service is encoded as having unlimited authority.

## Escalation Boundary

The escalation boundary defines when control must transfer. Per CR-ES-015 §4:

- intervention_model: human intervention semantics
- escalation_boundary: when control must transfer

When the realization encounters:

- authority exceeded
- policy requires approval
- constraint violation
- ambiguous exception
- high-impact decision
- human escalation request

The Autonomous Service must transfer control, not proceed unilaterally.

## See Also

- ADR-ES-015 §6
- CR-ES-015 §4, §10, §11, §18
- ASVC-AUTO-CON-008 + ASVC-AUTO-CON-011 + ASVC-AUTO-CON-013 + ASVC-AUTO-NEG-012
- architecture/autonomous-service-boundary.md
- concepts/autonomous-service.md
