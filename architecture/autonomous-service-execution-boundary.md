# Autonomous Service Execution Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Execution Mechanism

Autonomous Service does NOT require a particular execution mechanism. The execution mechanism may include:

- Human
- Agent
- System
- Service
- Workflow
- Agentic Workflow

Autonomous Service is a semantic characteristic of service realization, not an implementation technology.

## Execution Boundary

The execution boundary is the seam between:

- the Autonomous Service semantic kind (what can be realized with material autonomous progression)
- the execution mechanism (how realization actually occurs)

The boundary is:

```
Autonomous Service (semantic)
        |
        v
   Execution mechanism (technology)
        |
        v
   Realization (observed outcome)
```

The execution mechanism may change without changing the Autonomous Service semantic kind.

## Materiality Rule

Per ADR-ES-015 §4 + CR-ES-015 §8, a Service shall NOT become Autonomous merely because it:

- uses AI
- uses automation
- uses an Agent
- uses an autonomous system
- runs without direct human supervision
- uses machine learning
- uses predefined decision rules

Material autonomous progression required in one or more of: decision execution, action execution, coordination, adaptation, exception handling, service progression toward objective.

## See Also

- ADR-ES-015 §4, §5, §9, §10
- CR-ES-015 §8
- architecture/autonomous-service-boundary.md
- architecture/service-autonomous-realization-boundary.md
- concepts/autonomous-service.md
