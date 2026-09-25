# Autonomous Offering Boundary

Per ADR-ES-019 section 1 + section 2 + section 3 + section 14 + section 21 and CR-ES-019 section 3 + section 7 + section 21.

## Position

Autonomous Offering belongs at the Offering boundary. It is a contextual specialization of Offering, NOT a parallel construct.

## Boundaries

Autonomous Offering is distinct from:
- Agentic Offering (per ADR-ES-019 section 13 + AOFF-AUTO-NEG-001)
- Autonomous Product (per ADR-ES-019 section 9 + AOFF-AUTO-NEG-002)
- Autonomous Service (per ADR-ES-019 section 10 + AOFF-AUTO-NEG-003)
- Autonomous Operations (per CR-ES-019 section 12 + AOFF-AUTO-NEG-004)
- Autonomous Value Stream (per ADR-ES-019 section 11 + AOFF-AUTO-NEG-005)
- Autonomous Enterprise (per ADR-ES-019 section 12 + AOFF-AUTO-NEG-016)

## Realization Pattern

Per ADR-ES-019 section 5:

```
Offering Objective
   |
   v
Offering Context
   |
   v
Sense / Assess
   |
   v
Decision
   |
   v
Configuration / Composition
   |
   v
Action / Coordination
   |
   v
Fulfillment
   |
   v
Observe Outcome
   |
   v
Adapt
   <loop>
```

## Progression Boundaries

Per ADR-ES-019 section 5, autonomous progression operates within:
- Objective
- Authority
- Policy
- Constraints
- Governance
- Escalation

Autonomy therefore means bounded independent progression, not unrestricted operation.

## Materiality

Per ADR-ES-019 section 6 + section 13, material autonomous proving requires substantive evidence in one or more of:
- autonomous offering configuration
- autonomous proposition selection
- autonomous product/service composition
- autonomous fulfillment coordination
- autonomous response to contextual conditions
- autonomous exception handling
- autonomous adaptation
- autonomous progression toward an offering objective

## Foundational Dependency

Per ADR-ES-019 section 2, this ADR does NOT establish the complete semantic definition of Offering. The parent Offering concept remains to be canonicalized via ADR-ES-019 (next-foundational tranche).

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
