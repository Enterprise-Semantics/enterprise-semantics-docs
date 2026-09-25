# Autonomous Service vs Autonomous Value Stream Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Semantic Levels

Autonomous Service and Autonomous Value Stream operate at different semantic levels:

- **Autonomous Service**: service-level autonomous realization
- **Autonomous Value Stream**: end-to-end autonomous value realization

## Boundary

An Autonomous Value Stream may use multiple Autonomous Services per CR-ES-015 §7:

```
Autonomous Value Stream
        |
        | uses (one or more)
        v
Autonomous Service
```

However, the converse is NOT true per ASVC-AUTO-NEG-014:

```
Autonomous Value Stream
        |
        | does NOT automatically make
        v
every participating Service autonomous
```

## Distinct Semantic Kinds

- Autonomous Service is the service boundary
- Autonomous Value Stream is the value-stream boundary

These are distinct semantic kinds.

## See Also

- ADR-ES-015 §13
- CR-ES-015 §7 + ASVC-AUTO-NEG-005 + ASVC-AUTO-NEG-014
- architecture/autonomous-service-boundary.md
- concepts/autonomous-service.md
- concepts/autonomous-value-stream.md
