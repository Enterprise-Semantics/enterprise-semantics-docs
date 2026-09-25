# Autonomous Product / Autonomous Value Stream Boundary

Per ADR-ES-017 §11 and CR-ES-017 §6 + §7.

## Distinction

Autonomous Value Stream describes autonomous progression at the end-to-end value-realization boundary. Autonomous Product describes autonomous progression at the product boundary.

```
Autonomous Value Stream
   |
   v
realizes Stakeholder Value
   |
   v
may involve Autonomous Product
```

## Boundary Preservation

Per ADR-ES-017 §11 + APROD-AUTO-NEG-005 + APROD-AUTO-NEG-014:

- Autonomous Value Stream is NOT Autonomous Product
- Autonomous Product is NOT Autonomous Value Stream
- A conventional Product may participate in an Autonomous Value Stream
- An Autonomous Product may participate in a conventional, Autonomous, or Agentic Value Stream

## Validator Constraint

The validator must prevent:

- Autonomous Product is-a Autonomous Value Stream (APROD-AUTO-NEG-005)
- Autonomous Value Stream is-a Autonomous Product (APROD-AUTO-NEG-005)
- Autonomous Product automatically establishes Autonomous Value Stream (APROD-AUTO-NEG-014)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
