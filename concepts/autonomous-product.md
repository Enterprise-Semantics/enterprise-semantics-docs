# Autonomous Product

Per ADR-ES-017 §1 + §2 + §3 + §7 + §20 and CR-ES-017 §2 + §6 + §17.

## Definition

An Autonomous Product is a Product whose realization, interaction, configuration, fulfillment, or adaptation is capable of progressing through defined decisions, actions, coordination, and adaptation within specified product objectives, authority, policies, constraints, and governance boundaries without requiring human intervention for every product decision or action.

## Specialization

Autonomous Product specializes Product. It does NOT redefine Product. The Product concept remains the universal foundational type at the Product boundary per ADR-ES-002.

## Four-State Product Model

Per ADR-ES-017 §3, Agentic and Autonomous are independent semantic dimensions:

| Agentic | Autonomous | Semantic characterization |
|---|---|---|
| No | No | Conventional Product |
| Yes | No | Agentic Product (v1.5.0) |
| No | Yes | Autonomous Product (v1.6.0, this ADR) |
| Yes | Yes | Agentic and Autonomous Product (combined semantic characterization, NOT a new foundational type) |

## Autonomous Materiality

Per ADR-ES-017 §5 + CR-ES-017 §8, material autonomous progression through material product decisions/actions required. The following do NOT independently establish Autonomous Product:

- software
- APIs
- automation
- AI
- an Agent
- machine learning
- event-driven execution

## Six Fences

Per ADR-ES-017 §4, autonomous progression is bounded by:

1. Product Objective
2. Authority
3. Policy
4. Constraints
5. Governance
6. Escalation

Autonomy means bounded independent progression, NOT unrestricted operation.

## Boundaries

Per ADR-ES-017 §8 + §11 + §13 and CR-ES-017 §6 + §7 + §9:

- Autonomous Product is NOT Agentic Product (APROD-AUTO-NEG-001)
- Autonomous Product is NOT Autonomous Service (APROD-AUTO-NEG-002)
- Autonomous Product is NOT Autonomous Capability (APROD-AUTO-NEG-003)
- Autonomous Product is NOT Autonomous Operations (APROD-AUTO-NEG-004)
- Autonomous Product is NOT Autonomous Value Stream (APROD-AUTO-NEG-005)
- Autonomous Product is NOT Autonomous Workflow (APROD-AUTO-NEG-016)
- Autonomous Product is NOT Autonomous Enterprise (APROD-AUTO-NEG-015)
- Autonomous Product is NOT AI Product (APROD-AUTO-NEG-006)
- Autonomous Product is NOT Automated Product (APROD-AUTO-NEG-008)

## Architectural Position

Per ADR-ES-017 §3 + §22 implicit, Autonomous Product belongs at the Product realization boundary, distinct from Capability, Service, Workflow, Operations, Value Stream, and Enterprise boundaries.

```
Capability
   |-- Agentic Capability
   |-- Autonomous Capability
Product
   |-- Agentic Product (v1.5.0)
   |-- Autonomous Product (v1.6.0)
Service
   |-- Agentic Service
   |-- Autonomous Service
Offering
   |-- Agentic Offering (v1.7.0, gated)
   |-- [Autonomous Offering -- future]
Value Stream
   |-- Agentic Value Stream
   |-- Autonomous Value Stream
Enterprise
   |-- Agentic Enterprise
   |-- Autonomous Enterprise
```

## AI / Automation Independence

Per ADR-ES-017 §9 + §10 and CR-ES-017 §10:

- AI is NOT required (APROD-AUTO-CON-015, APROD-AUTO-NEG-006)
- Automation is NOT sufficient (APROD-AUTO-CON-016, APROD-AUTO-NEG-008)
- AI-enabled Product is NOT automatically Autonomous Product (APROD-AUTO-NEG-007)
- Automated Product is NOT automatically Autonomous Product (APROD-AUTO-NEG-008)

## Human Participation

Per ADR-ES-017 §6, Autonomous Product remains compatible with human participation:

- human-in-the-loop
- human-on-the-loop
- human-over-the-loop
- approval gates
- exception intervention
- escalation
- supervisory governance

Autonomous Product does NOT mean human-free, unattended, uncontrolled, governance-free, unlimited, irreversible.

## Agentic / Autonomous Orthogonality

Per ADR-ES-017 §2 + §3 + §8 and CR-ES-017 §7, Autonomous Product does NOT imply Agentic Product. The two dimensions are independent semantic dimensions.

## Deferred Concepts

Per ADR-ES-017 §14 and CR-ES-017 §2, the following are NOT established by this ADR:

- Autonomous Offering
- Product autonomy maturity
- Autonomy levels
- Autonomous Portfolio
- Autonomous Agent
- Autonomous Product Agent
- Autonomous Ecosystem

## Provenance

- ADR-ES-003 (Value Stream Semantic Grounding)
- ADR-ES-004 (Agentic Semantic Grounding)
- ADR-ES-007 (Agentic Operations)
- ADR-ES-008 (Autonomous Operations)
- ADR-ES-009 (Autonomous Value Stream)
- ADR-ES-011 (Autonomous Enterprise)
- ADR-ES-014 (Agentic Service)
- ADR-ES-015 (Autonomous Service)
- ADR-ES-016 (Agentic Product)
- ADR-ES-017 (Autonomous Product decision)
- CR-ES-017 (implementation)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
