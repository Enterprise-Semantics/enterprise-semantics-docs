# Agentic Product vs Autonomous Product Orthogonality

Per ADR-ES-016 §12 and CR-ES-016 §9.

## 2x2 Matrix at Product Boundary

```
                    AUTONOMOUS
                       |
             No        |        Yes
        +--------------+--------------+
Agentic |              |              |
   No   | Conventional | Autonomous   |
        | Product      | Product      |
        |              | (deferred)   |
        +--------------+--------------+
   Yes  | Agentic      | Agentic +    |
        | Product      | Autonomous   |
        | (this ADR)   | Product      |
        |              | (future)     |
        +--------------+--------------+
```

## Orthogonality

Per ADR-ES-016 §12 + CR-ES-016 §9 + APROD-CON-019 + APROD-NEG-011:

- Agentic Product does NOT imply Autonomous Product
- Autonomous Product does NOT imply Agentic Product
- A Product may be both
- A Product may be neither

Autonomous Product is NOT established by this ADR. Per ADR-ES-016 §19, Autonomous Product is held for a separate ADR.

## Future State

The fourth state (Agentic + Autonomous) is a compositional future state, NOT a new subtype.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
