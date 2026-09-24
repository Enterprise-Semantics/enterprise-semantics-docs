# Agentic Service vs Agentic Operations Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Semantic Levels

Agentic Service and Agentic Operations operate at different semantic levels:

- **Agentic Service**: service-level delivery or interaction involving agentic behavior
- **Agentic Operations**: agentic operating mode for ongoing operational activity

## Boundary

An Agentic Service may operate within Agentic Operations per CR-ES-014 §7:

```
Agentic Operations
        |
        | contains
        v
Agentic Service (one or more)
```

However, the converse is NOT true per ASVC-NEG-004:

```
Agentic Operations
        |
        | do NOT make every Service Agentic
        v
```

## Distinct Semantic Kinds

- Agentic Service is the service boundary
- Agentic Operations is the operations boundary

These are distinct semantic kinds. An Agentic Service is a service-level construct ; Agentic Operations is an operations-level construct.

## See Also

- ADR-ES-014 §9
- CR-ES-014 §7 + ASVC-NEG-004
- architecture/agentic-service-boundary.md
- concepts/agentic-service.md
- concepts/agentic-operations.md
