# Agentic Offering vs Autonomous Offering Orthogonality

Per ADR-ES-018 §6 and CR-ES-018 §14.

## 2x2 Matrix at Offering Boundary

```
                    AUTONOMOUS
                       |
             No        |        Yes
        +--------------+--------------+
Agentic |              |              |
   No   | Conventional | Autonomous   |
        | Offering     | Offering     |
        |              | (deferred)   |
        +--------------+--------------+
   Yes  | Agentic      | Agentic +    |
        | Offering     | Autonomous   |
        | (v1.7.0)     | Offering     |
        |              | (future)     |
        +--------------+--------------+
```

## Orthogonality

Per ADR-ES-018 §6 + CR-ES-018 §14 + AOFF-CON-019 + AOFF-NEG-011:

- Agentic Offering does NOT imply Autonomous Offering
- Autonomous Offering does NOT imply Agentic Offering
- An Offering may be both
- An Offering may be neither

Autonomous Offering is NOT established by this ADR. Per ADR-ES-018 §14, Autonomous Offering is held for a separate ADR.

## Future State

The fourth state (Agentic + Autonomous) is a compositional future state, NOT a new subtype.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
