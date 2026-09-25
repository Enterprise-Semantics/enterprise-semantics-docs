# Agentic Product

Per ADR-ES-016 §1 + §2 + §3 + §7 + §20 and CR-ES-016 §3 + §8 + §30.

## Definition

An Agentic Product is a Product whose material realization, interaction, configuration, adaptation, or fulfillment incorporates agentic behavior in interpreting intent, selecting or coordinating actions, or adapting product behavior toward an intended outcome within defined authority, policy, and contextual boundaries.

## Specialization

Agentic Product specializes Product. It does NOT redefine Product. The Product concept remains the universal foundational type at the Product boundary per ADR-ES-002.

## Agentic Materiality

Agentic behavior must materially affect how the product realizes or interacts. Per ADR-ES-016 §6 + CR-ES-016 §5 + §27, the following do NOT independently establish Agentic Product:

- inclusion of an AI model
- use of machine learning
- use of an API
- automated execution
- conversational interaction
- recommendation functionality
- presence of an Agent somewhere in the implementation
- dynamic software behavior without delegated intent and bounded action selection

## Boundaries

Per ADR-ES-016 §5 + §17 + §18 and CR-ES-016 §13-§17:

- Agentic Product is NOT Agent (APROD-NEG-001)
- Agentic Product is NOT Agentic Capability (APROD-NEG-002)
- Agentic Product is NOT Agentic Service (APROD-NEG-003)
- Agentic Product is NOT Agentic Workflow (APROD-NEG-004)
- Agentic Product is NOT Agentic Operations (APROD-NEG-005)
- Agentic Product is NOT Agentic Value Stream (APROD-NEG-006)
- Agentic Product is NOT Autonomous Product (APROD-NEG-011)
- Agentic Product is NOT AI Product (APROD-NEG-007)
- Agentic Product is NOT Automated Product (APROD-NEG-009)

## Architectural Position

Per ADR-ES-016 §3 + §31, Agentic Product belongs at the Product realization boundary, distinct from Capability, Service, Workflow, Operations, Value Stream, and Enterprise boundaries.

```
Capability
   |-- Agentic Capability
   |-- Autonomous Capability
Product
   |-- Agentic Product
       |-- [Autonomous Product -- future]
Service
   |-- Agentic Service
   |-- Autonomous Service
Value Stream
   |-- Agentic Value Stream
   |-- Autonomous Value Stream
Enterprise
   |-- Agentic Enterprise
   |-- Autonomous Enterprise
```

## AI / Automation Independence

Per ADR-ES-016 §13 + §14 and CR-ES-016 §10 + §11:

- AI is NOT required (APROD-CON-017, APROD-NEG-007)
- Automation is NOT sufficient (APROD-CON-018, APROD-NEG-009)
- AI-enabled Product is NOT automatically Agentic Product (APROD-NEG-008)
- Automated Product is NOT automatically Agentic Product (APROD-NEG-009)

## Human Participation

Per ADR-ES-016 §15 and CR-ES-016 §12, Agentic Product permits:

- human-in-the-loop interaction
- human-on-the-loop oversight
- human-over-the-loop governance
- approval gates
- exception-based intervention
- escalation
- human-controlled boundaries

Agentic does NOT mean human-free.

## Agentic / Autonomous Orthogonality

Per ADR-ES-016 §12 and CR-ES-016 §9, Agentic Product does NOT imply Autonomous Product. The 2x2 matrix at the Product boundary permits:

- Conventional Product
- Agentic Product (this ADR)
- Autonomous Product (deferred per ADR-ES-016 §19)
- Agentic + Autonomous Product (future combination, NOT a new subtype)

## Deferred Concepts

Per ADR-ES-016 §19 and CR-ES-016 §2, the following are NOT established by this ADR:

- Autonomous Product
- AI Product
- Autonomous Product levels
- Product autonomy maturity
- Agentic Product maturity
- Autonomous Offering
- Agentic Offering
- Agentic Portfolio
- Autonomous Portfolio
- Product Agent
- Autonomous Agent
- Agentic Ecosystem
- Autonomous Ecosystem

## Provenance

- ADR-ES-003 (Value Stream Semantic Grounding)
- ADR-ES-004 (Agentic Semantic Grounding)
- ADR-ES-005 (Agentic Value Stream)
- ADR-ES-006 (Agentic Workflow)
- ADR-ES-007 (Agentic Operations)
- ADR-ES-012 (Agentic Capability)
- ADR-ES-014 (Agentic Service)
- ADR-ES-015 (Autonomous Service)
- ADR-ES-016 (Agentic Product decision)
- CR-ES-016 (implementation)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
