# Agentic Organization / Agentic Operations Boundary

Per ADR-ES-020 section 7 and CR-ES-020 section 10.

## Distinction

Agentic Operations describes the operating mode of operational activity. Agentic Organization describes the broader organizational coordination boundary.

```
Agentic Organization
   |
   v
organizational boundary
   |
   v
may operate through
   |
   v
Agentic Operations
```

## Boundary Preservation

Per ADR-ES-020 section 7 + AORG-NEG-003 + AORG-NEG-014:

- Agentic Organization is NOT Agentic Operations
- Agentic Operations does NOT automatically make the Organization agentic

## Validator Constraint

The validator must prevent:
- Agentic Organization is-a Agentic Operations (AORG-NEG-003)
- Agentic Operations is-a Agentic Organization (unless explicitly modeled)
- Agentic Operations automatically makes the Organization agentic (AORG-NEG-014)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
