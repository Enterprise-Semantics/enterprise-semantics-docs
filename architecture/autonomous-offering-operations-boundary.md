# Autonomous Offering / Autonomous Operations Boundary

Per ADR-ES-019 section 12 and CR-ES-019 section 12.

## Distinction

Autonomous Operations represents the operating environment or mode of operational realization. It is NOT an Offering subtype.

```
Autonomous Offering
   |
   v
may depend upon
   |
   v
Autonomous Operations
```

## Boundary Preservation

Per ADR-ES-019 section 12 + AOFF-AUTO-NEG-004:

- Autonomous Operations is NOT a subtype of Offering
- Autonomous Offering is NOT Autonomous Operations

## Validator Constraint

The validator must prevent:
- Autonomous Offering is-a Autonomous Operations (AOFF-AUTO-NEG-004)
- Autonomous Operations is-a Autonomous Offering (unless an explicitly modeled separate specialization establishes this)
- Autonomous Operations automatically makes the Offering autonomous (AOFF-AUTO-NEG-015)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
