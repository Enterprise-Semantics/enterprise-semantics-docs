# Agentic Service vs Agentic Capability Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Semantic Levels

Agentic Service and Agentic Capability operate at different semantic levels:

- **Agentic Service**: service-level delivery or interaction involving agentic behavior
- **Agentic Capability**: enduring ability to achieve or enable an Outcome through material agentic realization

## Boundary

A capability may be delivered through an Agentic Service per CR-ES-014 §7:

```
Agentic Capability
        |
        | delivered-through
        v
Agentic Service
```

However, an Agentic Service may expose or enable capabilities that are not themselves Agentic Capabilities. The relationship is support, not inheritance.

## Distinct Semantic Kinds

- Agentic Service is the service boundary
- Agentic Capability is the capability boundary

These are distinct semantic kinds. Agentic Capability supports Agentic Service delivery ; Agentic Service supports Agentic Capability realization.

## See Also

- ADR-ES-014 §7
- CR-ES-014 §7 + ASVC-CON-016 + ASVC-NEG-002
- architecture/agentic-service-boundary.md
- concepts/agentic-service.md
- concepts/agentic-capability.md
