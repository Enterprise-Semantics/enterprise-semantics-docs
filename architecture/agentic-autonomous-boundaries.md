# Agentic/Autonomous Boundaries

Per ADR-ES-022 + CR-ES-022 section 9.

## Four-State Characterization (per ADR-ES-022 section 5)

Where both dimensions are semantically applicable:

| Agentic | Autonomous | Characterization |
|---|---|---|
| No | No | Conventional |
| Yes | No | Agentic |
| No | Yes | Autonomous |
| Yes | Yes | Agentic + Autonomous |

This is a semantic characterization, not a mandatory four-class inheritance hierarchy.

## Cross-Cutting Patterns

### Agentic Pattern (per ADR-ES-022 section 7)

Agentic specializations SHOULD consistently evaluate:
Intent, Context, Delegation, Authority, Interpretation, Action Selection, Coordination, Adaptation, Intervention, Escalation, Outcome.

### Autonomous Pattern (per ADR-ES-022 section 8)

Autonomous specializations SHOULD consistently evaluate:
Objective, Context, Autonomy Scope, Decision Scope, Action Scope, Coordination Scope, Adaptation Scope, Authority, Policy, Constraint, Governance, Intervention, Escalation, Observation, Outcome.

Not every concept requires every property.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
