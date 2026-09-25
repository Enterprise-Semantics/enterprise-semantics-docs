# Agentic Organization

Per ADR-ES-020 section 1 + section 2 + section 3 + section 14 + section 20 and CR-ES-020 section 3 + section 7 + section 25.

## Definition

An Agentic Organization is an Organization in which material organizational activities, coordination, decision-making, or execution incorporate agentic behavior to interpret delegated intent, select or coordinate actions, adapt to context, or pursue organizational outcomes within defined authority, policy, and governance boundaries.

## Specialization

Agentic Organization specializes Organization. It does NOT redefine Organization. The Organization concept remains the universal foundational concept at the Organization boundary. Per ADR-ES-020 section 2 + CR-ES-020 section 2, this record does NOT introduce a foundational Organization ontology.

## Foundational Dependency Gate

Per ADR-ES-020 section 2 + CR-ES-020 section 2, before canonical implementation, the repository must establish:

Organization exists as a canonical semantic concept

**Status as of 2026-09-25:** The parent Organization concept is NOT yet canonical in Enterprise-Semantics. Per user directive messages 1552900782440058902 ("Proceed with 18") + 1552912455527571546 ("save, read, understand, implement"), this specialization is established with the dependency documented rather than blocked. The next-foundational tranche is ADR-ES-021 (Organization canonical grounding), which remains unresolved at acceptance.

## Material Agentic Behavior

Per ADR-ES-020 section 3 + CR-ES-020 section 8, agentic behavior must materially affect organizational:
- decision-making
- coordination
- execution
- adaptation
- delegation
- exception management
- organizational response

The mere presence of an Agent somewhere in the organization does NOT establish Agentic Organization.

## AI / Automation Independence

Per ADR-ES-020 section 9 + section 10 and CR-ES-020 section 14 + section 15:

- AI is NOT required (AORG-CON-018, AORG-NEG-006)
- Automation is NOT sufficient (AORG-CON-019, AORG-NEG-008)
- AI-enabled Organization is NOT automatically Agentic Organization (AORG-NEG-007)
- Automated Organization is NOT automatically Agentic Organization (AORG-NEG-008)

## Human Participation

Per ADR-ES-020 section 11, Agentic Organization permits:
- human decision-makers
- human supervisors
- human escalation
- human-in-the-loop
- human-on-the-loop
- human-over-the-loop
- delegated agent participation
- mixed human/agent coordination

Agentic Organization does NOT require replacing human organizational actors.

## Boundaries

Per ADR-ES-020 section 5 + section 6 + section 7 + section 14 + section 17 and CR-ES-020 section 9 - section 13:

- Agentic Organization is NOT an Agent (AORG-NEG-001)
- Agentic Organization is NOT Agentic Workflow (AORG-NEG-002)
- Agentic Organization is NOT Agentic Operations (AORG-NEG-003)
- Agentic Organization is NOT Agentic Enterprise (AORG-NEG-004)
- Agentic Organization is NOT Agentic Culture (AORG-NEG-005)
- Agentic Organization requires AI (AORG-NEG-006, rejected)
- AI-enabled Organization automatically becomes Agentic Organization (AORG-NEG-007, rejected)
- Automated Organization automatically becomes Agentic Organization (AORG-NEG-008, rejected)
- Organization containing an Agent automatically becomes Agentic Organization (AORG-NEG-009, rejected)
- Agentic Organization requires elimination of humans (AORG-NEG-010, rejected)
- Agentic Organization has unlimited authority (AORG-NEG-011, rejected)
- Agentic Organization has no governance boundary (AORG-NEG-012, rejected)
- Agentic Organization automatically becomes Autonomous Organization (AORG-NEG-013, rejected)
- Agentic Operations automatically makes the Organization agentic (AORG-NEG-014, rejected)
- Agentic Workflow automatically makes the Organization agentic (AORG-NEG-015, rejected)

## Architectural Position

Per ADR-ES-020 section 20, Agentic Organization introduces a new semantic branch at the Organization boundary, distinct from Capability, Product, Service, Offering, Workflow, Operations, Value Stream, and Enterprise.

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
   |-- Autonomous Offering
Organization
   |-- Agentic Organization (v1.9.0)
   |-- [Autonomous Organization -- future]
Value Stream
   |-- Agentic Value Stream
   |-- Autonomous Value Stream
Enterprise
   |-- Agentic Enterprise
   |-- Autonomous Enterprise
```

## Agentic / Autonomous Orthogonality

Per ADR-ES-020 section 8, Agentic Organization does NOT imply Autonomous Organization. Autonomous Organization is NOT established by this ADR.

## Deferred Concepts

Per ADR-ES-020 section 17, the following are NOT established by this ADR:
- Autonomous Organization
- Agentic Culture
- Autonomous Culture
- Agentic Ecosystem
- Autonomous Ecosystem
- Agentic Network
- Autonomous Network
- organizational autonomy maturity
- organizational agent hierarchy
- Agentic Management
- Autonomous Management

## Provenance

- ADR-ES-004 (Agentic Semantic Grounding)
- ADR-ES-007 (Agentic Operations)
- ADR-ES-010 (Agentic Enterprise)
- ADR-ES-011 (Autonomous Enterprise)
- ADR-ES-020 (Agentic Organization decision)
- CR-ES-020 (implementation)
- USER-DIRECTIVE-1552900782440058902 (dependency override)
- USER-DIRECTIVE-1552912455527571546 (paired tranche)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
