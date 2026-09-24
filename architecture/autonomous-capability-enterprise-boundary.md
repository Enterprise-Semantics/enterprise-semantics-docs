# Autonomous Capability vs Autonomous Enterprise Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013

## Semantic Levels

Autonomous Capability and Autonomous Enterprise operate at different semantic levels:

- **Autonomous Capability**: capability-level autonomy (what an Entity is able to achieve or enable with bounded independence)
- **Autonomous Enterprise**: enterprise-level autonomous progression (how the enterprise as a whole progresses autonomously)

## Boundary

The boundary is strict per ACAP-AUTO-NEG-006:

```
Autonomous Capability
        |
        | does NOT establish
        v
Autonomous Enterprise
```

A single Autonomous Capability does NOT establish an Autonomous Enterprise. Conversely, an Autonomous Enterprise may contain capabilities whose realization remains human-dependent.

## Distinct Semantic Kinds

- Autonomous Capability is the capability boundary
- Autonomous Enterprise is the enterprise boundary

These are distinct semantic kinds. An Autonomous Enterprise requires Autonomous Capabilities at multiple levels, including operations, value streams, and organization. Capability-level autonomy alone is necessary but not sufficient for enterprise-level autonomy.

## See Also

- ADR-ES-013 §12
- CR-ES-013 ACAP-AUTO-NEG-006
- ADR-ES-011 (Autonomous Enterprise Semantic Grounding)
- architecture/autonomous-capability-boundary.md
- concepts/autonomous-capability.md
- concepts/autonomous-enterprise.md (in the canonicalization pipeline)
