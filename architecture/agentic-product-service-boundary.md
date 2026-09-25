# Agentic Product / Agentic Service Boundary

Per ADR-ES-016 §9 and CR-ES-016 §13.

## Distinction

Product and Service must remain distinct.

```
PRODUCT
   |
   v
Agentic Product
   |
   v
may be delivered-through
   |
   v
SERVICE
   |
   v
Agentic Service
   |
   v
Autonomous Service
```

## Boundary Preservation

Per ADR-ES-016 §9 + APROD-NEG-003:

- An Agentic Service does NOT automatically make the Product Agentic
- An Agentic Product may employ conventional or agentic services
- The classification depends on where the material agentic behavior resides

## Validator Constraint

The validator must prevent:

- Agentic Service is-a Agentic Product (APROD-NEG-003)
- Agentic Product is-a Agentic Service (APROD-NEG-003)

unless an explicitly modeled separate specialization exists.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
