# Agentic Service

**Concept:** `ES:CONCEPT:agentic-service`
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014
**Target release:** v1.3.0
**Status:** Candidate
**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)

## Definition

An Agentic Service is a Service whose delivery or interaction materially incorporates agentic behavior in interpreting intent, selecting or coordinating actions, adapting service behavior, or executing service responses toward an intended outcome within defined authority, policy, and contextual boundaries.

The Service concept remains the universal foundational type per ADR-ES-002 ; Agentic Service is a contextual specialization, not a replacement or narrowing.

## Properties

- **service_intent**: the intended service outcome
- **agentic_scope**: where agentic behavior applies
- **service_context**: context in which service realization occurs
- **delegated_intent**: intent delegated by the consumer/stakeholder
- **authority_context**: permitted authority for service actions
- **decision_boundary**: scope of service-level decisions
- **action_selection_scope**: scope of agentic action selection
- **coordination_scope**: coordination that may occur within the service
- **adaptation_scope**: where adaptation is permitted
- **intervention_model**: human intervention semantics (in-the-loop, on-the-loop, over-the-loop)
- **escalation_boundary**: when control must transfer to a human or another service
- **policy_context**: applicable policies
- **constraint_context**: limiting conditions
- **realization_mode**: realization characteristics

## Agentic Materiality

Agentic behavior must be material to service realization. Per ADR-ES-014 §4 + CR-ES-014 §8:

A Service shall NOT become Agentic merely because it:

- invokes an Agent
- uses AI
- uses automation
- exposes an API
- contains an AI model
- supports conversational interaction
- is implemented by an autonomous system

Examples of material agentic behavior include:

1. interpreting delegated service intent
2. interpreting contextual service conditions
3. dynamically selecting service actions
4. dynamically coordinating service actions
5. adapting service behavior
6. interpreting service exceptions
7. deciding within bounded service authority
8. escalating when authority or policy boundaries are reached

## Canonical Realization Pattern

```
Service Intent
      |
      v
Agentic Service
      |
      v
Service Context
      |
      v
Interpretation
      |
      v
Decision / Action Selection
      |
      v
Service Execution
      |
      v
Service Outcome
      |
      v
Contextual Adaptation
   (loop)
```

Bounded by: Authority, Policy, Constraints, Service Contract, Governance, Escalation.

## Boundaries

Agentic Service is distinct from:

- Agent (the bearer, not the service)
- Capability (the enduring ability, not the service)
- Agentic Capability (orthogonal at capability boundary)
- Workflow (the execution mechanism, not the service)
- Agentic Workflow (the agentic execution mechanism, not the service)
- Operations (the operations boundary, not the service)
- Agentic Operations (the agentic operations boundary, not the service)
- Value Stream (end-to-end value realization, not the service)
- Agentic Value Stream (may use multiple Agentic Services, but Agentic Service does NOT imply Agentic Value Stream)
- Autonomous Service (orthogonal at service boundary, deferred per ADR-ES-014 §19)
- AI Service (AI is a technological mechanism, not a semantic kind)
- Automated Service (Automation is an execution mechanism, not agentic behavior)

## Agentic / Autonomous Orthogonality

At the service boundary, the four-state matrix is:

| Agentic | Autonomous | Interpretation |
|---|---|---|
| No | No | Conventional Service |
| Yes | No | Agentic Service |
| No | Yes | Future Autonomous Service |
| Yes | Yes | Future combined characterization |

Autonomous Service requires a separate ADR per ADR-ES-014 §19.

## Invariants

Per CR-ES-014 §10 + §11:

- Agentic Service specializes Service
- Agentic Service retains Service semantics
- Agentic Service has material agentic realization
- Agentic Service may interpret delegated intent
- Agentic Service may interpret contextual conditions
- Agentic Service may dynamically select actions
- Agentic Service may coordinate actions
- Agentic Service may adapt service behavior
- Agentic Service operates within defined authority
- Agentic Service may be governed by policy
- Agentic Service may engage an Agent
- Agentic Service may use Agentic Workflow
- Human participation is permitted (in-the-loop, on-the-loop, over-the-loop)
- AI is NOT required
- Automation is NOT sufficient
- Agentic Service remains distinct from Agentic Capability
- Agentic Service remains distinct from Agentic Operations
- Agentic Service remains distinct from Agentic Value Stream
- Agentic Service retains provenance and grounding

## See Also

- ADR-ES-014 (Agentic Service Semantic Grounding)
- CR-ES-014 (Implement Agentic Service)
- ADR-ES-012 (Agentic Capability Semantic Grounding)
- ADR-ES-002 (Enterprise Semantic Model)
- concepts/service.md
