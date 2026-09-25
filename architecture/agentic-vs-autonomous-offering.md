# Agentic vs Autonomous Offering Orthogonality

Per ADR-ES-019 section 13 and CR-ES-019 section 12.

## 2x2 Matrix at Offering Boundary

```
                    AUTONOMOUS
                       |
             No        |        Yes
        +--------------+--------------+
Agentic |              |              |
   No   | Conventional | Autonomous   |
        | Offering     | Offering     |
        |              | (v1.8.0)     |
        +--------------+--------------+
   Yes  | Agentic      | Agentic +    |
        | Offering     | Autonomous   |
        | (v1.7.0)     | Offering     |
        |              | (compos-     |
        |              | itional)     |
        +--------------+--------------+
```

## Orthogonality

Per ADR-ES-019 section 13 + CR-ES-019 section 12 + AOFF-AUTO-CON-020 + AOFF-AUTO-NEG-001:

- Agentic Offering does NOT imply Autonomous Offering
- Autonomous Offering does NOT imply Agentic Offering
- An Offering may be both
- An Offering may be neither

The combined state is NOT a new foundational type. It is a contextual combination.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
