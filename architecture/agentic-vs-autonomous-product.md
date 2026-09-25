# Agentic Product vs Autonomous Product Orthogonality

Per ADR-ES-017 §2 + §3 + §8 and CR-ES-017 §7.

## 2x2 Matrix at Product Boundary

```
                    AUTONOMOUS
                       |
             No        |        Yes
        +--------------+--------------+
Agentic |              |              |
   No   | Conventional | Autonomous   |
        | Product      | Product      |
        |              | (v1.6.0)     |
        +--------------+--------------+
   Yes  | Agentic      | Agentic +    |
        | Product      | Autonomous   |
        | (v1.5.0)     | Product      |
        |              | (combined)   |
        +--------------+--------------+
```

## Orthogonality

Per ADR-ES-017 §2 + §3 + §8 + CR-ES-017 §7 + APROD-AUTO-CON-020 + APROD-AUTO-NEG-001:

- Autonomous Product does NOT imply Agentic Product
- Agentic Product does NOT imply Autonomous Product
- A Product may be both
- A Product may be neither

The fourth state (Agentic + Autonomous) is a combined semantic characterization, NOT a new foundational type.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
