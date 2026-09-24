# Agent

## Definition

Per CR-ES-004 §5 + ADR-ES-004 §5:

> An Agent is an Entity capable of interpreting delegated intent,
> selecting or coordinating actions, and acting within defined
> authority toward an intended outcome.

## Distinctions

- **Agent != AI Agent**, per ADR-ES-004 §10 (AG-INV-004)
- **Agent != Process**, per ADR-ES-004 §13
- **Agent != Activity**, per ADR-ES-004 §9
- **Agent != System**, per ADR-ES-004 §5, System may support or implement an Agent

## Specialisations

- An Agent may be: human, software-based, computational, organizational, or socio-technical
- **AI Agent**, a possible specialization of Agent (not the definition)
- **Autonomous Agent**, out of scope for CR-ES-004, governed by prospective ADR-ES-007

## Relationships

Per CR-ES-004 §10, the 8 Agent subject-level predicates:

- `interprets`, Intent
- `pursues`, external:concept:goal
- `acts-within`, Authority
- `selects`, Action
- `coordinates`, Action
- `agent-produces`, external:concept:outcome
- `adapts-to`, external:concept:context
- `receives`, Intent

## Governance

- **Established:** this file, concept documentation for CR-ES-004 §5
- **Source:** enterprise-semantics/concepts/agent.concept.yaml
- **Governing ADR:** ADR-ES-004 §5
- **Governing CR:** CR-ES-004 §5

## See also

- [Agentic](./agentic.md), the semantic property / mode of operation
- [Intent](./intent.md), the delegated objective
- [Authority](./authority.md), the bounded scope of permitted action
- [Action](./action.md), the semantic unit of agentic action selection
- [Agentic Boundary](../architecture/agentic-boundary.md), boundary tests

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)