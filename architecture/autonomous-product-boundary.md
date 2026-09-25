# Autonomous Product Boundary

Per ADR-ES-017 §1 + §2 + §3 + §7 + §20 and CR-ES-017 §2 + §6 + §17.

## Position

Autonomous Product belongs at the Product realization boundary. It is a contextual specialization of Product, NOT a parallel construct.

## Boundaries

Autonomous Product is distinct from:

- Agentic Product (per ADR-ES-017 §2 + §3 + §8 + APROD-AUTO-NEG-001)
- Autonomous Service (per ADR-ES-017 §11 + APROD-AUTO-NEG-002)
- Autonomous Capability (per ADR-ES-017 §11 + APROD-AUTO-NEG-003)
- Autonomous Operations (per ADR-ES-017 §11 + APROD-AUTO-NEG-004)
- Autonomous Value Stream (per ADR-ES-017 §11 + APROD-AUTO-NEG-005)
- Autonomous Workflow (per ADR-ES-017 §13)
- Autonomous Enterprise (per ADR-ES-017 §13 + APROD-AUTO-NEG-015)
- AI Product (per ADR-ES-017 §9 + APROD-AUTO-NEG-006)
- Automated Product (per ADR-ES-017 §10 + APROD-AUTO-NEG-008)

## Realization Pattern

Per ADR-ES-017 §4 + CR-ES-017 §5:

```
Product Objective
   |
   v
Product Context
   |
   v
Sense / Assess
   |
   v
Decision
   |
   v
Action Selection
   |
   v
Product Execution
   |
   v
Observe Outcome
   |
   v
Adapt
   <loop>
```

## Six Fences

Per ADR-ES-017 §4, autonomous progression is bounded by:

```
Objective -> Authority -> Policy -> Constraints -> Governance -> Escalation
```

## Materiality

Per ADR-ES-017 §5 + CR-ES-017 §8, material autonomous progression requires substantive evidence in one or more of:

- independent product decisions
- independent selection of permitted actions
- autonomous configuration
- autonomous coordination
- autonomous fulfillment progression
- contextual adaptation
- autonomous exception handling
- autonomous progression toward product objectives

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
