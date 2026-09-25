# Agentic Offering

Per ADR-ES-018 §1 + §2 + §3 + §10 + §14 and CR-ES-018 §3 + §7 + §21.

## Definition

An Agentic Offering is an Offering whose composition, interaction, configuration, fulfillment, or value realization materially incorporates agentic behavior in interpreting intent, selecting or coordinating actions, or adapting the offering toward an intended stakeholder outcome within defined authority, policy, and contextual boundaries.

## Specialization

Agentic Offering specializes Offering. It does NOT redefine Offering. The Offering concept remains the universal foundational concept at the Offering boundary. Per ADR-ES-018 §16 + CR-ES-018 §2, this record does NOT introduce a foundational Offering ontology.

## Foundational Dependency Gate

Per ADR-ES-018 §16 + CR-ES-018 §2, before canonical implementation, the repository must verify one of:
1. Offering already exists as a canonical Enterprise-Semantics concept ;; or
2. a separately authorized Offering semantic grounding ADR establishes it.

**Status as of 2026-09-25:** The parent Offering concept is NOT yet canonical in Enterprise-Semantics. Per user directive message 1552900782440058902 ("Proceed with 18"), this specialization is established with the dependency documented rather than blocked. ADR-ES-019 (Offering canonical grounding) remains the next-foundational tranche.

## Agentic Materiality

Agentic behavior must be material to the Offering. Per ADR-ES-018 §5 + §13 + CR-ES-018 §13, the following do NOT independently establish Agentic Offering:
- an AI component somewhere in the implementation
- automated billing
- automated ordering
- a chatbot used only as an interface
- an Agent participating in an unrelated internal process

## AI / Automation Independence

Per ADR-ES-018 §7 + §8 and CR-ES-018 §14:

- AI is NOT required (AOFF-CON-017, AOFF-NEG-007)
- Automation is NOT sufficient (AOFF-CON-018, AOFF-NEG-009)
- AI-enabled Offering is NOT automatically Agentic Offering (AOFF-NEG-008)
- Automated Offering is NOT automatically Agentic Offering (AOFF-NEG-009)

## Human Participation

Per ADR-ES-018 §9, Agentic Offering permits:
- assisted interaction
- approval
- exception handling
- human escalation
- human oversight
- human-controlled boundaries

Agentic does NOT mean human-free.

## Boundaries

Per ADR-ES-018 §3 + §4 + §13 + §15 and CR-ES-018 §8-§12:

- Agentic Offering is NOT Agent (AOFF-NEG-001)
- Agentic Offering is NOT Agentic Product (AOFF-NEG-002)
- Agentic Offering is NOT Agentic Service (AOFF-NEG-003)
- Agentic Offering is NOT Agentic Workflow (AOFF-NEG-004)
- Agentic Offering is NOT Agentic Operations (AOFF-NEG-005)
- Agentic Offering is NOT Agentic Value Stream (AOFF-NEG-006)
- Agentic Offering is NOT Agentic Enterprise (AOFF-NEG-013)
- Agentic Offering is NOT AI Offering (AOFF-NEG-007)
- Agentic Offering is NOT Automated Offering (AOFF-NEG-009)
- Agentic Offering is NOT autonomous offering (AOFF-NEG-011)
- Agentic Product does NOT automatically make whole Offering agentic (AOFF-NEG-014)
- Agentic Service does NOT automatically make whole Offering agentic (AOFF-NEG-015)

## Architectural Position

Per ADR-ES-018 §22, Agentic Offering belongs at the Offering boundary, distinct from Capability, Product, Service, Workflow, Operations, Value Stream, and Enterprise boundaries.

```
Capability
   |-- Agentic Capability
   |-- Autonomous Capability
Product
   |-- Agentic Product
   |-- Autonomous Product
Service
   |-- Agentic Service
   |-- Autonomous Service
Offering
   |-- Agentic Offering (v1.7.0)
   |-- [Autonomous Offering -- future]
Value Stream
   |-- Agentic Value Stream
   |-- Autonomous Value Stream
Enterprise
   |-- Agentic Enterprise
   |-- Autonomous Enterprise
```

## Agentic / Autonomous Orthogonality

Per ADR-ES-018 §6 and CR-ES-018 §14, Agentic Offering does NOT establish Autonomous Offering. The 2x2 matrix at the Offering boundary permits:
- Conventional Offering
- Agentic Offering (this ADR, v1.7.0)
- Autonomous Offering (deferred per ADR-ES-018 §14)
- Agentic + Autonomous Offering (future combination, NOT a new subtype)

## Deferred Concepts

Per ADR-ES-018 §14, the following are NOT established by this ADR:
- Autonomous Offering
- Autonomous Portfolio
- Autonomous Agent
- Autonomous Product Agent
- Autonomous Ecosystem
- Autonomous Enterprise beyond ADR-ES-011

## Provenance

- ADR-ES-004 (Agentic Semantic Grounding)
- ADR-ES-005 (Agentic Value Stream)
- ADR-ES-006 (Agentic Workflow)
- ADR-ES-007 (Agentic Operations)
- ADR-ES-012 (Agentic Capability)
- ADR-ES-014 (Agentic Service)
- ADR-ES-016 (Agentic Product)
- ADR-ES-017 (Autonomous Product)
- ADR-ES-018 (Agentic Offering decision)
- CR-ES-018 (implementation)
- USER-DIRECTIVE-1552900782440058902 (dependency override)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
