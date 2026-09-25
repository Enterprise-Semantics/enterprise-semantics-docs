# Agentic Offering / Agentic Service Boundary

Per ADR-ES-018 §4 and CR-ES-018 §9.

## Distinction

Agentic Offering concerns the broader proposition presented to a stakeholder. Agentic Service concerns service realization. They operate at different semantic boundaries.

```
Agentic Offering
   |
   v
may comprise / expose
   |
   v
Agentic Product / Agentic Service
```

## Boundary Preservation

Per ADR-ES-018 §4 + AOFF-NEG-003 + AOFF-NEG-015:

- Agentic Offering is NOT Agentic Service
- Agentic Service does NOT automatically make the whole Offering agentic

## Validator Constraint

The validator must prevent:
- Agentic Offering is-a Agentic Service (AOFF-NEG-003)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
