# Agentic Service Execution Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Execution Mechanism

Agentic Service does NOT require a particular execution mechanism. The execution mechanism may include:

- Human
- Agent
- System
- Service
- Workflow
- Agentic Workflow

Agentic Service is a semantic characteristic of service realization, not an implementation technology.

## Execution Boundary

The execution boundary is the seam between:

- the Agentic Service semantic kind (what can be realized with material agentic behavior)
- the execution mechanism (how realization actually occurs)

The boundary is:

```
Agentic Service (semantic)
        |
        v
   Execution mechanism (technology)
        |
        v
   Realization (observed outcome)
```

The execution mechanism may change without changing the Agentic Service semantic kind. A Service may transition between agentic and conventional execution while retaining its Agentic Service identity (subject to the materiality rule per ADR-ES-014 §4).

## Materiality Rule

A Service shall NOT become Agentic merely because it:

- uses AI
- uses automation
- uses an Agent
- uses ML
- exposes an API
- contains an AI model
- uses a conversational interface

Agentic behavior must be material to realization per ADR-ES-014 §4 + CR-ES-014 §8.

## See Also

- ADR-ES-014 §4, §5, §12, §13
- CR-ES-014 §8
- architecture/agentic-service-boundary.md
- architecture/service-agentic-realization-boundary.md
- concepts/agentic-service.md
