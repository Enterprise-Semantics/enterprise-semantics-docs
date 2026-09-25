# Agentic Offering Boundary

Per ADR-ES-018 §1 + §2 + §3 + §10 + §14 and CR-ES-018 §3 + §7 + §21.

## Position

Agentic Offering belongs at the Offering boundary. It is a contextual specialization of Offering, NOT a parallel construct.

## Boundaries

Agentic Offering is distinct from:
- Agent (per ADR-ES-018 §15 + AOFF-NEG-001)
- Agentic Product (per ADR-ES-018 §3 + AOFF-NEG-002)
- Agentic Service (per ADR-ES-018 §4 + AOFF-NEG-003)
- Agentic Workflow (per ADR-ES-018 §11 + AOFF-NEG-004)
- Agentic Operations (per ADR-ES-018 §12 + AOFF-NEG-005)
- Agentic Value Stream (per ADR-ES-018 §12 + AOFF-NEG-006)
- Agentic Enterprise (per ADR-ES-018 §13 + AOFF-NEG-013)
- AI Offering (per ADR-ES-018 §7 + AOFF-NEG-007)
- Automated Offering (per ADR-ES-018 §8 + AOFF-NEG-009)
- Autonomous Offering (per ADR-ES-018 §6 + AOFF-NEG-011)

## Realization Pattern

Per ADR-ES-018 §11:

```
Stakeholder Intent
   |
   v
Agentic Offering
   |
   v
Interpret Context
   |
   v
Configure / Compose
   |
   v
Select / Coordinate
   |
   v
Fulfill
   |
   v
Observe Outcome
   |
   v
Adapt / Escalate
   <loop>
```

## Materiality

Per ADR-ES-018 §5 + §13, material agentic realization requires substantive evidence in one or more of:
- interpreting stakeholder intent
- dynamically configuring an offering
- dynamically composing product/service components
- selecting fulfillment arrangements
- coordinating multiple services
- adapting an offering to context
- interpreting exceptions
- dynamically determining permitted response paths

## Foundational Dependency Gate

Per ADR-ES-018 §16 + CR-ES-018 §2, this ADR depends on Offering being canonical. As of 2026-09-25, the parent Offering concept is NOT yet canonical in Enterprise-Semantics. Per user directive message 1552900782440058902, the dependency is documented rather than blocking implementation.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
