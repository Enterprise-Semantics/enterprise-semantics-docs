# Autonomous Enterprise Operating Loop

Per CR-ES-011 §17 + ADR-ES-011 §8.

## Scope

The Autonomous Enterprise operating loop is the canonical pattern
that governs how an Autonomous Enterprise pursues material enterprise
decisions, coordination, execution, value realisation, and
adaptation under defined objectives, authority, policies,
constraints, and governance. The loop is bounded by human
intervention capabilities and escalation mechanisms.

## The canonical loop

```
Enterprise Objective
       |
       v
Enterprise Context
       |
       v
Sense
       |
       v
Interpret
       |
       v
Decide
       |
       v
Coordinate
       |
       v
Act
       |
       v
Observe Outcome
       |
       v
Adapt
       ^
       +----- loop back to Sense
```

The loop iterates continuously within defined boundaries.

## Bounded operation

The loop is explicitly bounded by:

```
Authority
   |
   v
Policy
   |
   v
Constraints
   |
   v
Governance
   |
   v
Autonomous Decision
   |
   v
Autonomous Action
   |
   v
Outcome
   |
   v
Escalation
```

Human intervention remains available at defined boundaries
(per AE-AUTO-CON-009). The defining distinction is that human
intervention is not required for every enterprise decision or
action (per ADR-ES-011 §9).

## Component semantics

Per ADR-ES-011 §8:

- **Sense.** Sense the enterprise context for relevant signals.
- **Interpret.** Interpret enterprise signals into actionable
  representations.
- **Decide.** Determine the next autonomous decision within
  decision scope and authority.
- **Coordinate.** Coordinate relevant resources, services,
  systems, and processes.
- **Act.** Initiate or execute the autonomous action within action
  scope.
- **Observe Outcome.** Record the outcome and contextual state.
- **Adapt.** Modify behaviour in response to the outcome and
  contextual state.

Each component may be implemented via agentic, autonomous,
automated, or human-led mechanisms. The semantic of the operating
loop is preserved across implementation modes.

## Operating modes

Per ADR-ES-011 §19 + AE-AUTO-CON-017:

A valid Autonomous Enterprise does not require all enterprise
behaviour to be autonomous. The model permits mixed-mode operation:

- Autonomous Value Streams
- Agentic Value Streams
- Conventional Value Streams
- Autonomous Operations
- Agentic Operations
- Conventional Operations
- Automated Workflows
- Agentic Workflows
- Human-led work

This mixed-mode model is important because autonomy can be scoped.

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B.
- Vendor-specific embargo: zero references.
