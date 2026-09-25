# Agentic Organization / Agentic Workflow Boundary

Per ADR-ES-020 section 11 and CR-ES-020 section 11.

## Distinction

Agentic Workflow describes agentic behavior at the workflow execution boundary. Agentic Organization describes agentic behavior at the organizational coordination boundary.

```
Agentic Organization
   |
   v
organizational boundary
   |
   v
may use
   |
   v
Agentic Workflow
```

## Boundary Preservation

Per ADR-ES-020 section 11 + AORG-NEG-002 + AORG-NEG-015:

- Agentic Organization is NOT Agentic Workflow
- Agentic Workflow does NOT automatically make the Organization agentic

## Validator Constraint

The validator must prevent:
- Agentic Organization is-a Agentic Workflow (AORG-NEG-002)
- Agentic Workflow is-a Agentic Organization (unless explicitly modeled)
- Agentic Workflow automatically makes the Organization agentic (AORG-NEG-015)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
