# Autonomous Product / Autonomous Service Boundary

Per ADR-ES-017 §11 and CR-ES-017 §6 + §7.

## Distinction

Autonomous Product and Autonomous Service remain distinct specializations.

```
PRODUCT
   |
   v
Autonomous Product
   |
   v
may be delivered-through
   |
   v
SERVICE
   |
   v
Autonomous Service
```

## Boundary Preservation

Per ADR-ES-017 §11 + APROD-AUTO-NEG-002:

- An Autonomous Service does NOT automatically make the Product Autonomous
- An Autonomous Product may be delivered through conventional or autonomous services
- The classification depends on where the material autonomous progression resides

## Validator Constraint

The validator must prevent:

- Autonomous Service is-a Autonomous Product (APROD-AUTO-NEG-002)
- Autonomous Product is-a Autonomous Service (APROD-AUTO-NEG-002)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
