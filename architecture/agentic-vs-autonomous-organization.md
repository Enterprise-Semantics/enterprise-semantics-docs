# Agentic vs Autonomous Organization Orthogonality

Per ADR-ES-020 section 8.

## 2x2 Matrix at Organization Boundary

```
                    AUTONOMOUS
                       |
             No        |        Yes
        +--------------+--------------+
Agentic |              |              |
   No   | Conventional | Autonomous   |
        | Organization | Organization |
        |              | (deferred)   |
        +--------------+--------------+
   Yes  | Agentic      | Agentic +    |
        | Organization | Autonomous   |
        | (v1.9.0)     | Organization |
        |              | (future)     |
        +--------------+--------------+
```

## Orthogonality

Per ADR-ES-020 section 8 + AORG-NEG-013:

- Agentic Organization does NOT imply Autonomous Organization
- Autonomous Organization does NOT imply Agentic Organization
- An Organization may be both
- An Organization may be neither

Autonomous Organization is NOT established by this ADR. Per ADR-ES-020 section 17, Autonomous Organization is held for a separate ADR.

## Future State

The fourth state (Agentic + Autonomous) is a compositional future state, NOT a new subtype.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
