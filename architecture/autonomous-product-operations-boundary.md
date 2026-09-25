# Autonomous Product / Autonomous Operations Boundary

Per ADR-ES-017 §11 + §13 and CR-ES-017 §6 + §7.

## Distinction

Autonomous Operations represents the operating environment or mode of autonomous operational realization. It is NOT a Product subtype.

```
Autonomous Product
   |
   v
may depend on / use
   |
   v
Autonomous Operations
```

## Boundary Preservation

Per ADR-ES-017 §11 + APROD-AUTO-NEG-004 + APROD-AUTO-NEG-013:

- Autonomous Operations is NOT a Product subtype
- Autonomous Product is NOT Autonomous Operations
- Autonomous Product may be supported by Autonomous Operations
- Autonomous Operations does NOT automatically make every Product autonomous

## Validator Constraint

The validator must prevent:

- Autonomous Product is-a Autonomous Operations (APROD-AUTO-NEG-004)
- Autonomous Operations is-a Autonomous Product
- Autonomous Operations automatically makes every Product autonomous (APROD-AUTO-NEG-013)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
