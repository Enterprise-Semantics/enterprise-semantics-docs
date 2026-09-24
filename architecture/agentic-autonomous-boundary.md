# Agentic vs Autonomous Boundary

Per CR-ES-004 §14 + ADR-ES-004 §9, the boundary between Agentic and Autonomous is foundational.

## Distinction

```text
Agentic            Autonomous
  :                   :
  v                   v
delegated intent   self-direction
action selection   self-management
contextual       agency : self-adaptation
bounded authority   reduced external intervention
goal-directed       sustained independent operation
```

## The boundary test

```text
Agentic         Autonomous
  :              :
  v              v
may operate with limited autonomy
  :
  v
MAY evolve toward Autonomous (separately governed)
```

## What is NOT implied

Per ADR-ES-004 §9 + AG-INV-003:

- **Agentic -> Autonomous**, NOT implied as semantic identity
- **Autonomy requires separate semantic grounding**, per ADR-ES-004 §9 + AG-INV-010, governed by prospective ADR-ES-007 (Autonomous Operations)

## What IS allowed

- Agentic may operate with limited autonomy, per ADR-ES-004 §9, but limited autonomy does NOT make an Agentic construct semantically equivalent to Autonomous
- Agentic may evolve toward Autonomous, the transition requires separate semantic governance

## Why this distinction matters

Per ADR-ES-004 §9, conflating Agentic with Autonomous creates ambiguity when modeling enterprise operating behavior. Agentic semantics establishes the bounded operation, Autonomous semantics establishes the self-sustaining operation. These are different things.

## Out of scope for CR-ES-004

Per CR-ES-004 §3 + §14:

- Autonomous Agent
- Autonomous Enterprise
- Autonomous Operations

These require separate semantic grounding (ADR-ES-007 family).

## Cross-references

- [Agent](../concepts/agent.md)
- [Agentic](../concepts/agentic.md)
- [Agentic vs Automation Boundary](./agentic-boundary.md)
- [Agentic Execution Pattern Boundary](./agentic-execution-boundary.md)

## Governance

- **Governing ADR:** ADR-ES-004 §9 + §14
- **Governing CR:** CR-ES-004 §14

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)