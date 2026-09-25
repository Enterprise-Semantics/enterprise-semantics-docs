# Autonomous Offering / Autonomous Product Boundary

Per ADR-ES-019 section 9 and CR-ES-019 section 9.

## Distinction

An Offering may comprise or include multiple Products. An Autonomous Offering may contain Autonomous Products without itself being an Autonomous Product.

```
Offering
   |
   v
may comprise / include
   |
   v
Product
   |
   v
Autonomous Product

Offering
   |
   v
Autonomous Offering
```

## Boundary Preservation

Per ADR-ES-019 section 9 + AOFF-AUTO-NEG-002 + AOFF-AUTO-NEG-013:

- Autonomous Offering is NOT Autonomous Product
- Autonomous Product does NOT automatically make the whole Offering autonomous
- An Offering can be autonomous because of how the overall proposition is configured, composed, interacted with, fulfilled, or adapted, even where its constituent Products are not individually autonomous

## Validator Constraint

The validator must prevent:
- Autonomous Offering is-a Autonomous Product (AOFF-AUTO-NEG-002)
- Autonomous Product is-a Autonomous Offering (unless an explicitly modeled separate specialization establishes this)
- Autonomous Product automatically makes the whole Offering autonomous (AOFF-AUTO-NEG-013)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
