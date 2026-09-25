# Autonomous Product / Autonomous Capability Boundary

Per ADR-ES-017 §11 and CR-ES-017 §6 + §7.

## Distinction

Capability represents an enduring ability. Product represents an offered realization of value.

```
Capability
   |
   v
enables
   |
   v
Product
   |
   v
Autonomous Product

Autonomous Capability
   |
   v
may enable
   |
   v
Autonomous Product
```

## Boundary Preservation

Per ADR-ES-017 §11 + APROD-AUTO-CON-019 + APROD-AUTO-NEG-003:

- An Autonomous Capability does NOT automatically make every Product it enables autonomous
- Autonomous materiality must be demonstrated at the Product boundary
- Autonomous Product is NOT Autonomous Capability

## Validator Constraint

The validator must prevent:

- Autonomous Capability is-a Autonomous Product (APROD-AUTO-NEG-003)
- Autonomous Product is-a Autonomous Capability (APROD-AUTO-NEG-003)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
