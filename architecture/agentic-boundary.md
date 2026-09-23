# Agentic Boundary (vs Automation)

Per CR-ES-004 §12 + ADR-ES-004 §8 ;;; the boundary between Agentic operation and Automation is foundational.

## Two patterns

**Conventional automation:**

```text
Trigger
  v
Predefined Rule
  v
Predefined Action
```

**Agentic operation:**

```text
Delegated Intent
      v
   Context
      v
Interpretation
      v
Action Selection
      v
Execution
      v
Outcome
      ^ (contextual adaptation)
      |
   Context
```

## Boundary tests

Per ADR-ES-004 §8 + AG-INV-002:

- **Automation != Agentic** ;;; per ADR-ES-004 §8 ;;; conventional automated workflow may remain non-agentic
- **Agentic operation may use Automation** ;;; automation is a tool ;;; agentic operation may invoke it

## What is NOT Agentic

- Pure predefined-rule execution (Trigger -> Rule -> Action) ;;; no contextual interpretation
- Pure event-driven scripts ;;; no action selection
- Pure deterministic pipelines ;;; no outcome orientation (completion-oriented, not outcome-oriented)

## What IS Agentic

- Context-sensitive action selection ;;; Agent selects Action based on Context
- Outcome-oriented execution ;;; actions are directed toward an intended outcome, not mere completion
- Authority-bounded action ;;; Agent operates within explicit or implicit authority boundaries
- Adaptive execution ;;; Agent may alter execution path in response to changing conditions

## Cross-references

- [Agent](../concepts/agent.md)
- [Agentic](../concepts/agentic.md)
- [Agentic vs Autonomous Boundary](./agentic-autonomous-boundary.md)
- [Agentic Execution Pattern Boundary](./agentic-execution-boundary.md)
- [Agentic Relationships](../relationships/agentic-relationships.md)

## Governance

- **Governing ADR:** ADR-ES-004 §8
- **Governing CR:** CR-ES-004 §12

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)