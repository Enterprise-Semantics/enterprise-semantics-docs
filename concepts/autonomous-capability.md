# Autonomous Capability

**Concept:** `ES:CONCEPT:autonomous-capability`
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013
**Target release:** v1.2.0
**Status:** Candidate
**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)

## Definition

An Autonomous Capability is a Capability whose realization is capable of progressing through decisions, actions, coordination, and adaptation within defined objectives, authority, policies, constraints, and governance boundaries without requiring human intervention for every capability decision or action.

The Capability concept remains the universal foundational type per ADR-ES-002 ; Autonomous Capability is a contextual specialization, not a replacement or narrowing.

## Properties

- **objective**: what autonomous realization is intended to achieve
- **autonomy_scope**: where autonomy applies
- **realization_context**: context in which capability realization occurs
- **decision_scope**: decisions that may progress independently
- **action_scope**: actions that may progress independently
- **coordination_scope**: coordination that may occur independently
- **authority_context**: permitted authority
- **policy_context**: applicable policies
- **constraint_context**: limiting conditions
- **governance_context**: governance boundaries
- **adaptation_scope**: where adaptation is permitted
- **intervention_model**: human intervention semantics
- **escalation_boundary**: when control must transfer
- **observation_scope**: what realization observes
- **realization_mode**: conventional, automated, agentic, autonomous, or combined

## Realization Pattern

```
Capability Objective
       |
       v
Autonomous Capability
       |
       v
  Context
       |
       v
Interpret / Assess
       |
       v
 Decision
       |
       v
Action Selection
       |
       v
 Execution
       |
       v
Observe Outcome
       |
       v
   Adapt
    (loop)
```

Bounded by: Authority, Policy, Constraints, Governance, Escalation.

## Boundaries

Autonomous Capability is distinct from:

- Agentic Capability (orthogonal dimension at capability boundary, see ADR-ES-013 §7)
- Agent (the bearer, not the ability)
- Autonomous Operations (operational realization, not capability)
- Autonomous Value Stream (end-to-end value realization, not capability)
- Autonomous Enterprise (enterprise-level autonomy, not capability-level)
- AI Capability (AI is a technological mechanism, not a semantic kind)
- Automated Capability (automation is an execution mechanism, not autonomy)

## Invariants

Per CR-ES-013 §9 + §10:

- Autonomous Capability specializes Capability
- Autonomous Capability retains enduring-ability semantics
- Autonomous Capability is outcome-oriented
- Autonomous Capability has defined autonomy, decision, and action scope
- Autonomous Capability operates within defined authority
- Autonomous Capability is governed by policy and bounded by constraints
- Autonomous Capability may adapt within defined scope
- Autonomous Capability may retain human intervention
- Autonomous Capability supports escalation
- Autonomous Capability does NOT require AI
- Autonomous Capability does NOT require automation (Automation is NOT sufficient)
- Autonomous Capability may coexist with Agentic behavior (orthogonal dimensions)
- Autonomous Capability may support Autonomous Value Stream realization
- Autonomous Capability may be supported by Autonomous Operations
- Autonomous Capability retains provenance and grounding

## See Also

- ADR-ES-013 (Autonomous Capability Semantic Grounding)
- CR-ES-013 (Implement Autonomous Capability)
- ADR-ES-012 (Agentic Capability Semantic Grounding) , the orthogonal specialization
- ADR-ES-002 (Enterprise Semantic Model) , the universal Capability concept
- concepts/capability.md
- concepts/agentic-capability.md
