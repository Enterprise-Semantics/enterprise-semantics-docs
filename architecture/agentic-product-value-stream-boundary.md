# Agentic Product / Agentic Value Stream Boundary

Per ADR-ES-016 §11 and CR-ES-016 §15.

## Distinction

Agentic Value Stream describes agentic behavior at the end-to-end value-realization boundary. Agentic Product describes agentic behavior at the product boundary.

```
Agentic Value Stream
   |
   v
realizes Stakeholder Value
   |
   v
may involve Agentic Product
```

## Boundary Preservation

Per ADR-ES-016 §11 + APROD-CON-016 + APROD-NEG-006 + APROD-NEG-015:

- Agentic Value Stream is NOT Agentic Product
- Agentic Product is NOT Agentic Value Stream
- A conventional Product may participate in an Agentic Value Stream
- An Agentic Product may participate in a conventional, Agentic, or Autonomous Value Stream

## Validator Constraint

The validator must prevent:

- Agentic Product is-a Agentic Value Stream (APROD-NEG-006)
- Agentic Value Stream is-a Agentic Product (APROD-NEG-006)
- Agentic Product automatically establishes Agentic Value Stream (APROD-NEG-015)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
