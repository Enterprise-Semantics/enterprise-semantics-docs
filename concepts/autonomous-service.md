# Autonomous Service

**Concept:** `ES:CONCEPT:autonomous-service`
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015
**Target release:** v1.4.0
**Status:** Candidate
**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)

## Definition

An Autonomous Service is a Service whose delivery or interaction is capable of progressing through decisions, actions, coordination, and adaptation within defined service objectives, authority, policies, constraints, and governance boundaries without requiring human intervention for every service decision or action.

The Service concept remains the universal foundational type per ADR-ES-002 ; Autonomous Service is a contextual specialization, not a replacement or narrowing.

## Properties

- **service_objective**: defines the service result toward which autonomous progression is directed
- **autonomy_scope**: defines where autonomy applies
- **service_context**: defines conditions relevant to service realization
- **decision_scope**: defines decisions permitted to progress independently
- **action_scope**: defines independently executable actions
- **coordination_scope**: defines independently coordinated service activity
- **authority_context**: defines permitted authority
- **policy_context**: defines applicable policy
- **constraint_context**: defines limiting conditions
- **governance_context**: defines governance boundaries
- **adaptation_scope**: defines where autonomous adaptation is permitted
- **intervention_model**: defines human intervention semantics
- **escalation_boundary**: defines when control transfers
- **observation_scope**: defines what the service observes
- **realization_mode**: characterizes conventional, automated, agentic, autonomous, or combined realization

## Autonomy Materiality Rule

A Service qualifies as Autonomous Service only when autonomous progression is material to service realization.

The following do NOT independently establish autonomy:
- uses AI
- uses automation
- uses an Agent
- uses an autonomous system
- runs without direct human supervision
- uses machine learning
- uses predefined decision rules

Material evidence required in one or more of: decision execution, action execution, coordination, adaptation, exception handling, service progression toward objective.

## Canonical Realization Pattern

```
Service Objective
       |
       v
Service Context
       |
       v
Sense / Assess
       |
       v
Interpret
       |
       v
Decision
       |
       v
Action Selection
       |
       v
Service Execution
       |
       v
Observe Service Outcome
       |
       v
Adapt
   (loop)
```

Bounded by: Authority, Policy, Constraints, Governance, Service Contract, Escalation.

## Boundaries

Autonomous Service is distinct from:

- Agentic Service (orthogonal dimension at service boundary)
- Agent (the bearer, not the service)
- Capability (the enduring ability, not the service)
- Autonomous Capability (capability-level autonomy, not service-level)
- Workflow (the execution mechanism, not the service)
- Agentic Workflow (the agentic execution mechanism, not the service)
- Operations (the operations boundary, not the service)
- Autonomous Operations (the autonomous operations boundary, not the service)
- Value Stream (end-to-end value realization, not the service)
- Autonomous Value Stream (may use multiple Autonomous Services, but Autonomous Service does NOT imply Autonomous Value Stream)
- Enterprise (enterprise-level autonomy, not service-level)
- Autonomous Enterprise (does NOT establish from a single Autonomous Service)
- AI Service (AI is a technological mechanism, not a semantic kind)
- Automated Service (Automation is an execution mechanism, not autonomy)

## Agentic / Autonomous Orthogonality

At the service boundary, the four-state matrix is:

| Agentic | Autonomous | Interpretation |
|---|---|---|
| No | No | Conventional Service |
| Yes | No | Agentic Service (ADR-ES-014, v1.3.0) |
| No | Yes | Autonomous Service (ADR-ES-015, v1.4.0) |
| Yes | Yes | Combined characterization (NOT a new subtype) |

Autonomous Service requires a separate decision from Agentic Service.

## Invariants

Per CR-ES-015 §10 + §11:

- Autonomous Service specializes Service
- Autonomous Service retains Service semantics
- Autonomous Service has material autonomous realization
- Autonomous Service has defined service objective, autonomy scope, decision scope, action scope
- Autonomous Service operates within authority (Authority + Policy + Constraints + Governance)
- Autonomous Service may adapt within defined scope
- Autonomous Service supports escalation
- Human intervention remains permitted
- AI is NOT required
- Automation is NOT sufficient
- Autonomous Service may use Agentic Workflow
- Autonomous Service may be supported by Autonomous Operations
- Autonomous Service may participate in Autonomous Value Stream realization
- Autonomous Service remains distinct from Agentic Service, Agent, Autonomous Capability, Autonomous Operations, Autonomous Value Stream, Autonomous Enterprise
- Autonomous Service retains provenance and grounding

## See Also

- ADR-ES-015 (Autonomous Service Semantic Grounding)
- CR-ES-015 (Implement Autonomous Service)
- ADR-ES-014 (Agentic Service Semantic Grounding) , the orthogonal specialization
- ADR-ES-002 (Enterprise Semantic Model) , the universal Service concept
