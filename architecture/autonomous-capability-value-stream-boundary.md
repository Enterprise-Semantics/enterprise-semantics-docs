# Autonomous Capability vs Autonomous Value Stream Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013

## Semantic Levels

Autonomous Capability and Autonomous Value Stream operate at different semantic levels:

- **Autonomous Capability**: capability-level autonomy (what an Entity is able to achieve or enable with bounded independence)
- **Autonomous Value Stream**: end-to-end autonomous value realization (how stakeholder value is realized autonomously across stages)

## Boundary

An Autonomous Capability may enable an Autonomous Value Stream per CR-ES-013 §7:

```
Autonomous Capability
        |
        | enables
        v
Autonomous Value Stream
```

However, the converse is NOT true per ACAP-AUTO-NEG-013:

```
Autonomous Value Stream
        |
        | does NOT automatically make
        v
every enabling Capability autonomous
```

## Distinct Semantic Kinds

- Autonomous Capability is the capability boundary (enduring ability)
- Autonomous Value Stream is the value-stream boundary (end-to-end value realization)

A capability may be enabled by an Autonomous Value Stream without itself being an Autonomous Capability. An Autonomous Value Stream may use multiple Capabilities, only some of which may themselves be Autonomous Capabilities.

## See Also

- ADR-ES-013 §11
- CR-ES-013 §7 + ACAP-AUTO-CON-016 + ACAP-AUTO-NEG-013
- architecture/autonomous-capability-boundary.md
- concepts/autonomous-capability.md
- concepts/autonomous-value-stream.md (in the canonicalization pipeline)
