# Autonomous Offering / Autonomous Value Stream Boundary

Per ADR-ES-019 section 11 and CR-ES-019 section 11.

## Distinction

Autonomous Value Stream describes autonomous behavior at the end-to-end value-realization boundary. Autonomous Offering describes autonomous behavior at the offering boundary.

```
Autonomous Value Stream
   |
   v
value realization journey
   |
   v
may involve
   |
   v
Autonomous Offering
```

## Boundary Preservation

Per ADR-ES-019 section 11 + AOFF-AUTO-NEG-005:

- Autonomous Offering is NOT Autonomous Value Stream
- Autonomous Value Stream is NOT Autonomous Offering
- An Autonomous Offering may participate in a conventional, Agentic, or Autonomous Value Stream

## Validator Constraint

The validator must prevent:
- Autonomous Offering is-a Autonomous Value Stream (AOFF-AUTO-NEG-005)
- Autonomous Value Stream is-a Autonomous Offering (unless an explicitly modeled separate specialization establishes this)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
