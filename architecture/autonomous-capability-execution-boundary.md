# Autonomous Capability Execution Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013

## Execution Mechanism

Autonomous Capability does NOT require a particular execution mechanism. The execution mechanism may be:

- human-supported
- automated
- agentic
- system-mediated
- service-mediated
- hybrid

Autonomous Capability is a semantic characteristic of capability realization, not an implementation technology.

## Execution Boundary

The execution boundary is the seam between:

- the Autonomous Capability semantic kind (what can be realized with bounded independence)
- the execution mechanism (how realization actually occurs)

The boundary is:

```
Autonomous Capability (semantic)
        |
        v
   Execution mechanism (technology)
        |
        v
   Realization (observed outcome)
```

The execution mechanism may change without changing the Autonomous Capability semantic kind. A Capability may transition between autonomous, agentic, and conventional execution while retaining its Autonomous Capability identity (subject to the materiality rule per ADR-ES-013 §4).

## Materiality Rule

A Capability shall NOT become Autonomous merely because it:

- uses AI
- uses automation
- uses an Agent
- uses ML
- exposes an API
- contains an AI model

Autonomous behavior must be material to realization per ADR-ES-013 §4 + CR-ES-013 §8.

## See Also

- ADR-ES-013 §3.3, §5
- CR-ES-013 §8
- architecture/autonomous-capability-boundary.md
- architecture/capability-autonomous-realization-boundary.md
- concepts/autonomous-capability.md
