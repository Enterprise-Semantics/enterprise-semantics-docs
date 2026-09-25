# Agentic Organization / Agentic Enterprise Boundary

Per ADR-ES-020 section 5 and CR-ES-020 section 9.

## Distinction

Agentic Enterprise describes enterprise-wide value realization and operation. Agentic Organization describes agentic behavior at the organizational coordination and operating boundary.

```
Agentic Organization
   |
   v
organizational operating boundary
   |
   v
may be part of
   |
   v
Agentic Enterprise
```

## Boundary Preservation

Per ADR-ES-020 section 5 + AORG-NEG-004:

- Agentic Organization is NOT Agentic Enterprise
- Agentic Enterprise may comprise multiple Agentic Organizations
- Agentic Organization does NOT automatically establish Agentic Enterprise

## Validator Constraint

The validator must prevent:
- Agentic Organization is-a Agentic Enterprise (AORG-NEG-004)
- Agentic Enterprise is-a Agentic Organization (unless explicitly modeled)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
