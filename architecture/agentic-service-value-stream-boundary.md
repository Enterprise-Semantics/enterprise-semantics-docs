# Agentic Service vs Agentic Value Stream Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Semantic Levels

Agentic Service and Agentic Value Stream operate at different semantic levels:

- **Agentic Service**: service-level delivery or interaction involving agentic behavior
- **Agentic Value Stream**: end-to-end stakeholder value realization materially involving agentic behavior

## Boundary

An Agentic Value Stream may use multiple Agentic Services per CR-ES-014 §7:

```
Agentic Value Stream
        |
        | uses
        v
Agentic Service (one or more)
```

However, the converse is NOT true per ASVC-NEG-005:

```
Agentic Service
        |
        | does NOT imply
        v
Agentic Value Stream
```

## Distinct Semantic Kinds

- Agentic Service is the service boundary
- Agentic Value Stream is the value-stream boundary

These are distinct semantic kinds. An Agentic Value Stream requires multiple services ; an Agentic Service alone does NOT establish an Agentic Value Stream.

## See Also

- ADR-ES-014 §10
- CR-ES-014 §7 + ASVC-NEG-005
- architecture/agentic-service-boundary.md
- concepts/agentic-service.md
- concepts/agentic-value-stream.md
