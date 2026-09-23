# Action

## Definition

Per CR-ES-004 §9 + ADR-ES-004 §14:

> Action is an intentional act performed or initiated by an Entity
> toward an intended result.

## Semantic unit for agentic action selection

Per ADR-ES-004 §17 ;;; Action is the semantic unit required to describe agentic action selection.

## Distinctions

Per CR-ES-004 §9 ;;; Action shall remain distinct from:

- **Process** ;;; Action is the semantic unit ;;; Process is the organized execution pattern
- **Activity** ;;; Action is intentional ;;; Activity is execution-level
- **Task** ;;; Action is broader than Task ;;; a Task is one form of Action
- **Workflow** ;;; Workflow is coordinated execution ;;; Action is the unit being coordinated

## Relationships

- `Intent guides Action` ;;; per CR-ES-004 §10 ;;; Action is directed toward the Intent's purpose
- `Authority constrains Action` ;;; per CR-ES-004 §10 ;;; Action is limited by the Authority scope
- `Agent selects Action` ;;; per CR-ES-004 §10 ;;; Agent chooses among possible actions
- `Agent coordinates Action` ;;; per CR-ES-004 §10 ;;; Agent sequences Actions
- `Action action-produces Outcome` ;;; per CR-ES-004 §10 ;;; Action results in the Outcome

## The 3 instruction-decision-action patterns

Per ADR-ES-004 §17 ;;; the agentic decision boundary distinguishes:

- **Instruction** ;;; prescribed action or procedure
- **Decision** ;;; selection among possible actions or responses
- **Agentic Decision** ;;; context-sensitive action selection performed by an Agent within delegated authority toward an intended outcome

The 3 patterns:

```text
Instruction      Intent           ; Agent + Context
  :                   :           :
  v                   v           v
Execution       Context           Decision / Action Selection
                                  :
                                  v
                                Execution
                                  :
                                  v
                                Outcome
```

The middle and right patterns are the agentic pattern ;;; left is conventional automation.

## Governance

- **Source:** enterprise-semantics/concepts/action.concept.yaml
- **Governing ADR:** ADR-ES-004 §14 + §17
- **Governing CR:** CR-ES-004 §9

## See also

- [Agent](./agent.md) ;;; Agent selects and coordinates Action
- [Intent](./intent.md) ;;; Intent guides Action
- [Authority](./authority.md) ;;; Authority constrains Action

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)