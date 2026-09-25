# Autonomous Offering / Autonomous Service Boundary

Per ADR-ES-019 section 10 and CR-ES-019 section 10.

## Distinction

Autonomous Offering concerns the broader proposition presented to a stakeholder. Autonomous Service concerns service realization. They operate at different semantic boundaries.

```
Autonomous Offering
   |
   v
may comprise / expose
   |
   v
Autonomous Product / Autonomous Service
```

## Boundary Preservation

Per ADR-ES-019 section 10 + AOFF-AUTO-NEG-003 + AOFF-AUTO-NEG-014:

- Autonomous Offering is NOT Autonomous Service
- Autonomous Service does NOT automatically make the whole Offering autonomous

## Validator Constraint

The validator must prevent:
- Autonomous Offering is-a Autonomous Service (AOFF-AUTO-NEG-003)
- Autonomous Service is-a Autonomous Offering (unless an explicitly modeled separate specialization establishes this)
- Autonomous Service automatically makes the whole Offering autonomous (AOFF-AUTO-NEG-014)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
