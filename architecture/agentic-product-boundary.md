# Agentic Product Boundary

Per ADR-ES-016 §1 + §2 + §3 + §7 + §20 and CR-ES-016 §3 + §8 + §30.

## Position

Agentic Product belongs at the Product realization boundary. It is a contextual specialization of Product, NOT a parallel construct.

## Boundaries

Agentic Product is distinct from:

- Agent (per ADR-ES-016 §5 + APROD-NEG-001)
- Agentic Capability (per ADR-ES-016 §10 + APROD-NEG-002)
- Agentic Service (per ADR-ES-016 §9 + APROD-NEG-003)
- Agentic Workflow (per ADR-ES-016 §5 + APROD-NEG-004)
- Agentic Operations (per ADR-ES-016 §5 + APROD-NEG-005)
- Agentic Value Stream (per ADR-ES-016 §11 + APROD-NEG-006)
- Autonomous Product (per ADR-ES-016 §12 + APROD-NEG-011)
- AI Product (per ADR-ES-016 §13 + APROD-NEG-007)
- Automated Product (per ADR-ES-016 §14 + APROD-NEG-009)

## Realization Pattern

Per ADR-ES-016 §8 + CR-ES-016 §5:

```
Product Intent
   |
   v
Agentic Product
   |
   v
Product Context
   |
   v
Interpret Intent
   |
   v
Assess Context
   |
   v
Select / Coordinate Action
   |
   v
Product Execution
   |
   v
Product Outcome
   |
   v
Adapt / Escalate
   <loop>
```

## Materiality

Per ADR-ES-016 §6 + CR-ES-016 §27, material agentic realization requires substantive evidence in one or more of:

- intent interpretation
- contextual interpretation
- dynamic action selection
- agentic coordination
- contextual adaptation
- exception interpretation
- bounded decision-making
- escalation

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
