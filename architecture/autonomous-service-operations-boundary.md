# Autonomous Service vs Autonomous Operations Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Semantic Levels

Autonomous Service and Autonomous Operations operate at different semantic levels:

- **Autonomous Service**: service-level autonomous realization
- **Autonomous Operations**: agentic/independent operating mode for ongoing operational activity

## Boundary

Autonomous Operations may support an Autonomous Service per CR-ES-015 §7:

```
Autonomous Operations
        |
        | supports
        v
Autonomous Service
```

However, the converse is NOT true per ASVC-AUTO-NEG-013:

```
Autonomous Operations
        |
        | do NOT automatically make every Service autonomous
        v
```

## Distinct Semantic Kinds

- Autonomous Service is the service boundary
- Autonomous Operations is the operations boundary

These are distinct semantic kinds per ADR-ES-015 §12.

## See Also

- ADR-ES-015 §12
- CR-ES-015 §7 + ASVC-AUTO-NEG-004 + ASVC-AUTO-NEG-013
- architecture/autonomous-service-boundary.md
- concepts/autonomous-service.md
- concepts/autonomous-operations.md
