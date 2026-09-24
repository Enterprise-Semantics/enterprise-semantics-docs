# Agentic Capability

## Definition

Per ADR-ES-012 §1 + CR-ES-012 §2:

> An Agentic Capability is a Capability whose realization materially
> incorporates agentic behavior in achieving or enabling an intended
> Outcome within defined authority, policy, and contextual boundaries.

## Semantic purpose

The Agentic Capability semantic establishes a formal representation of
agentic realization at the capability boundary. Per ADR-ES-012 §2-§4:

- Agentic Capability is a Capability, not a replacement, not a parallel
  construct.
- Agentic Capability specialises Capability ; contextual specialization
  of the universal foundational type.
- Agentic Capability retains the mandatory Capability semantics
  established by ADR-ES-002.
- Capability universality is preserved ; not every Capability is
  Agentic.

## Capability inheritance

Per ADR-ES-012 §6, the Agentic Capability schema preserves the
mandatory Capability semantics established by ADR-ES-002:

- definition (enduring ability)
- outcome orientation
- realization through Workflow / Operations / Service / System
- support by Agent / Role / Resource
- governance and provenance

The implementation does NOT duplicate or redefine these properties
where inheritance/reference is supported by the repository schema
architecture.

## Specialization boundary

Per ADR-ES-012 §2 + §4:

```
Capability
   |
   +-- Conventional Capability
   +-- Agentic Capability
   +-- Other future contextual specializations
```

The model must preserve the universal nature of Capability. Agentic
Capability describes how a Capability is materially realized, not what
a Capability is.

## Materiality requirement

Per ADR-ES-012 §7, Agentic behavior must be material to capability
realization. AI, automation, Agent participation, or autonomy alone do
not qualify.

Examples of material agentic participation include:

- contextual decision-making
- dynamic action selection
- adaptive coordination
- delegated execution
- contextual exception handling
- agentic interaction with stakeholders
- agentic resource coordination
- adaptive fulfillment of the capability's intended outcome

The mere use of an Agent as a tool does not automatically qualify.

## Boundary

Per ADR-ES-012 §8, the architecture distinguishes:

```
CAPABILITY
"What enduring ability exists?"
        |
        v
AGENTIC CAPABILITY
"Is the ability materially realized agentically?"
        |
        v
REALIZATION
Agentic Workflow / Agentic Operations / Service / System / Human
        |
        v
OUTCOME
```

Capability remains upstream of specific execution mechanisms.

## Realization pattern

Per ADR-ES-012 §21, the canonical realization pattern is:

```
Capability Intent
        |
        v
Agentic Capability
        |
        v
Context
        |
        v
Interpretation
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
Outcome
        |
        v
Adaptation
```

Bounded by Authority, Policy, and Constraints.

## Orthogonality

Per ADR-ES-012 §13-§14, the semantic architecture permits:

```
Capability
   |
   +-- Agentic
   +-- Autonomous
   +-- Agentic + Autonomous
   +-- neither
```

Only Agentic Capability is established by ADR-ES-012. Autonomous
Capability is explicitly deferred per ADR-ES-012 §25.

## Conformance invariants

Per ADR-ES-012 §23, 18 conformance invariants (ACAP-CON-001..018)
govern the Agentic Capability boundary:

- ACAP-CON-001: Agentic Capability specializes Capability
- ACAP-CON-002: Agentic Capability retains the Capability definition
- ACAP-CON-003: Agentic behavior must be material to realization
- ACAP-CON-004: Agentic Capability remains outcome-oriented
- ACAP-CON-005: Agentic Capability may engage an Agent
- ACAP-CON-006: Agentic Capability may be realized through Agentic Workflow
- ACAP-CON-007: Agentic Capability may be supported by Agentic Operations
- ACAP-CON-008: Agentic Capability may enable Agentic Value Stream realization
- ACAP-CON-009: Agentic Capability does not require AI
- ACAP-CON-010: Automation does not establish Agentic Capability
- ACAP-CON-011: Agentic Capability does not imply autonomy
- ACAP-CON-012: Agentic Capability does not imply Agentic Enterprise
- ACAP-CON-013: Agent is not a subtype of Capability
- ACAP-CON-014: Agentic Workflow is not a subtype of Capability
- ACAP-CON-015: Agentic Operations is not a subtype of Capability
- ACAP-CON-016: Agentic Value Stream is not a subtype of Capability
- ACAP-CON-017: Agentic Capability operates within appropriate authority boundaries
- ACAP-CON-018: Agentic Capability requires provenance and semantic grounding

## Deferred concepts

Per ADR-ES-012 §25 + CR-ES-012 §30:

- Autonomous Capability (held for ADR-ES-013)
- AI Capability
- Agentic Capability Maturity
- Agentic Capability Levels
- Agentic Organization
- Autonomous Organization
- Agentic Culture
- Autonomous Culture
- Agentic Ecosystem
- Autonomous Ecosystem

Each requires an independent ADR/CR pair.
