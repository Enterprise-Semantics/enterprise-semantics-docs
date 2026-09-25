# Autonomous Offering

Per ADR-ES-019 section 1 + section 2 + section 3 + section 14 + section 21 and CR-ES-019 section 3 + section 7 + section 21.

## Definition

An Autonomous Offering is an Offering whose composition, interaction, configuration, fulfillment, or value realization is capable of progressing through defined decisions, actions, coordination, and adaptation within specified offering objectives, authority, policies, constraints, and governance boundaries without requiring human intervention for every offering decision or action.

## Specialization

Autonomous Offering specializes Offering. It does NOT redefine Offering. The Offering concept remains the universal foundational concept at the Offering boundary. Per ADR-ES-019 section 2 + CR-ES-019 section 2, this record does NOT introduce a foundational Offering ontology.

## Foundational Dependency Gate

Per ADR-ES-019 section 2 + CR-ES-019 section 2, before canonical implementation, the repository must establish:

Offering exists as a canonical semantic concept

**Status as of 2026-09-25:** The parent Offering concept is NOT yet canonical in Enterprise-Semantics. Per user directive messages 1552900782440058902 ("Proceed with 18") + 1552912455527571546 ("save, read, understand, implement"), this specialization is established with the dependency documented rather than blocked. The next-foundational tranche is ADR-ES-019 (Offering canonical grounding), which remains unresolved at acceptance.

## Autonomous Materiality

Autonomous behavior must be material to the Offering. Per ADR-ES-019 section 6 + section 13 + CR-ES-019 section 8 + section 13, the following do NOT independently establish Autonomous Offering:
- an AI component somewhere in the implementation
- automated billing
- automated ordering
- a chatbot used only as an interface
- an Agent participating in an unrelated internal process
- recommendation systems
- event-driven execution

## AI / Automation Independence

Per ADR-ES-019 section 14 + section 15 and CR-ES-019 section 14:

- AI is NOT required (AOFF-AUTO-CON-018, AOFF-AUTO-NEG-006)
- Automation is NOT sufficient (AOFF-AUTO-CON-019, AOFF-AUTO-NEG-008)
- AI-enabled Offering is NOT automatically Autonomous Offering (AOFF-AUTO-NEG-007)
- Automated Offering is NOT automatically Autonomous Offering (AOFF-AUTO-NEG-008)

## Human Participation

Per ADR-ES-019 section 7, Autonomous Offering permits:
- approval gates
- human-in-the-loop
- human-on-the-loop
- human-over-the-loop
- exception intervention
- escalation
- supervisory governance

Autonomous does NOT mean human-free.

## Boundaries

Per ADR-ES-019 section 9 + section 10 + section 11 + section 12 + section 13 + section 15 and CR-ES-019 section 9 - section 12:

- Autonomous Offering is NOT Agentic Offering (AOFF-AUTO-NEG-001)
- Autonomous Offering is NOT Autonomous Product (AOFF-AUTO-NEG-002)
- Autonomous Offering is NOT Autonomous Service (AOFF-AUTO-NEG-003)
- Autonomous Offering is NOT Autonomous Operations (AOFF-AUTO-NEG-004)
- Autonomous Offering is NOT Autonomous Value Stream (AOFF-AUTO-NEG-005)
- Autonomous Offering requires AI (AOFF-AUTO-NEG-006, rejected)
- AI automatically establishes Autonomous Offering (AOFF-AUTO-NEG-007, rejected)
- Automation automatically establishes Autonomous Offering (AOFF-AUTO-NEG-008, rejected)
- Agent presence automatically establishes Autonomous Offering (AOFF-AUTO-NEG-009, rejected)
- Autonomous Offering requires elimination of humans (AOFF-AUTO-NEG-010, rejected)
- Autonomous Offering has unlimited authority (AOFF-AUTO-NEG-011, rejected)
- Autonomous Offering requires every action to be autonomous (AOFF-AUTO-NEG-012, rejected)
- Autonomous Product automatically makes the whole Offering autonomous (AOFF-AUTO-NEG-013, rejected)
- Autonomous Service automatically makes the whole Offering autonomous (AOFF-AUTO-NEG-014, rejected)
- Autonomous Operations automatically makes the Offering autonomous (AOFF-AUTO-NEG-015, rejected)
- Autonomous Offering implies Autonomous Enterprise (AOFF-AUTO-NEG-016, rejected)

## Architectural Position

Per ADR-ES-019 section 21, Autonomous Offering belongs at the Offering boundary, distinct from Capability, Product, Service, Workflow, Operations, Value Stream, and Enterprise boundaries.

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
   |-- Agentic Offering
   |-- Autonomous Offering (v1.8.0)
Value Stream
   |-- Agentic Value Stream
   |-- Autonomous Value Stream
Enterprise
   |-- Agentic Enterprise
   |-- Autonomous Enterprise
```

## Autonomous / Agentic Orthogonality

Per ADR-ES-019 section 13 and CR-ES-019 section 12, Autonomous Offering does NOT imply Agentic Offering. The 2x2 matrix at the Offering boundary permits:
- Conventional Offering
- Agentic Offering (v1.7.0)
- Autonomous Offering (v1.8.0)
- Agentic + Autonomous Offering (compositional future state, NOT a new subtype)

## Deferred Concepts

Per ADR-ES-019 section 18, the following are NOT established by this ADR:
- Offering autonomy maturity
- autonomy levels
- Autonomous Portfolio
- Autonomous Ecosystem
- Autonomous Marketplace
- Autonomous Product Portfolio
- Autonomous Agent

## Provenance

- ADR-ES-004 (Agentic Semantic Grounding)
- ADR-ES-005 (Agentic Value Stream)
- ADR-ES-007 (Agentic Operations)
- ADR-ES-008 (Autonomous Operations)
- ADR-ES-009 (Autonomous Value Stream)
- ADR-ES-011 (Autonomous Enterprise)
- ADR-ES-015 (Autonomous Service)
- ADR-ES-017 (Autonomous Product)
- ADR-ES-018 (Agentic Offering)
- ADR-ES-019 (Autonomous Offering decision)
- CR-ES-019 (implementation)
- USER-DIRECTIVE-1552900782440058902 (dependency override)
- USER-DIRECTIVE-1552912455527571546 (paired tranche)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
