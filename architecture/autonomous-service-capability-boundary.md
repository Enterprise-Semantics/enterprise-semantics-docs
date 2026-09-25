# Autonomous Service vs Autonomous Capability Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Semantic Levels

Autonomous Service and Autonomous Capability operate at different semantic levels:

- **Autonomous Service**: service-level autonomous realization (how a service can be realized with bounded independence)
- **Autonomous Capability**: capability-level autonomy (what an Entity is able to achieve with bounded independence)

## Boundary

An Autonomous Service may deliver or expose an Autonomous Capability per CR-ES-015 §7:

```
Autonomous Capability
        |
        | supports (where canonical)
        v
Autonomous Service
```

However, the converse is NOT true per ASVC-AUTO-NEG-015:

```
Autonomous Capability
        |
        | does NOT automatically make
        v
every delivered Service autonomous
```

## Distinct Semantic Kinds

- Autonomous Service is the service boundary
- Autonomous Capability is the capability boundary

These are distinct semantic kinds. Neither concept subsumes the other.

## See Also

- ADR-ES-015 §14
- CR-ES-015 §7 + ASVC-AUTO-NEG-003 + ASVC-AUTO-NEG-015
- architecture/autonomous-service-boundary.md
- concepts/autonomous-service.md
- concepts/autonomous-capability.md
