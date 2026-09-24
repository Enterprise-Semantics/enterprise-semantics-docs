# Service Authority Escalation Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Authority as a Boundary

Agentic Service operates within defined Authority and supports defined Escalation.

```
Service Intent
   |
   v
Service Context
   |
   v
Authority Context
   |
   v
Decision / Action
   |
   v
Service Outcome
   ^
   |
Contextual Adaptation (loop)
```

## Authority Properties

The Authority context of an Agentic Service defines:

- permitted authority scope
- approval thresholds
- escalation triggers
- decision/action boundaries
- intervention triggers

## Escalation Boundary

The escalation boundary defines when control must transfer. Per CR-ES-014 §4:

- intervention_model: human intervention semantics
- escalation_boundary: when control must transfer

When the realization encounters:

- authority exceeded
- policy requires approval
- constraint violation
- ambiguous exception
- human escalation request

The Agentic Service must transfer control, not proceed unilaterally.

## Material Agentic Behavior

Per ASVC-CON-004 to ASVC-CON-008, material agentic behavior includes:

- contextual interpretation
- delegated-intent interpretation
- dynamic action selection
- agentic coordination
- adaptive service behavior
- contextual exception interpretation
- bounded service decision-making

## See Also

- ADR-ES-014 §5, §14
- CR-ES-014 §4, §10, §17
- ASVC-CON-009 + ASVC-CON-010
- architecture/agentic-service-boundary.md
- concepts/agentic-service.md
