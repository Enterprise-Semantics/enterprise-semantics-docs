# Agentic Organization / Agent Boundary

Per ADR-ES-020 section 6 and CR-ES-020 section 12.

## Distinction

Agent is an acting entity. Agentic Organization is an organization-level operating mode that incorporates material agentic behavior in organizational coordination.

```
Agent
   |
   v
may operate within
   |
   v
Agentic Organization
```

## Boundary Preservation

Per ADR-ES-020 section 6 + AORG-NEG-001 + AORG-NEG-009:

- Agentic Organization is NOT an Agent
- An Agent is NOT an Agentic Organization
- An Organization does NOT become Agentic merely because it contains an Agent

## Validator Constraint

The validator must prevent:
- Agentic Organization is-a Agent (AORG-NEG-001)
- Agent is-a Agentic Organization (unless explicitly modeled)
- Organization containing an Agent automatically becomes Agentic Organization (AORG-NEG-009)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
