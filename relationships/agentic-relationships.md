# Agentic Relationships

Per CR-ES-004 §10 + ADR-ES-004 §14 ;;; the 11 governed Agentic predicates.

## Predicate table

| Subject | Predicate | Object | Provenance |
|---|---|---|---|
| agent | interprets | intent | CR-ES-004 §10 + ADR-ES-004 §14 |
| agent | pursues | external:concept:goal | CR-ES-004 §10 + ADR-ES-004 §14 |
| agent | acts-within | authority | CR-ES-004 §10 + ADR-ES-004 §14 + §15 |
| agent | selects | action | CR-ES-004 §10 + ADR-ES-004 §14 + §17 |
| agent | coordinates | action | CR-ES-004 §10 + ADR-ES-004 §14 |
| agent | agent-produces | external:concept:outcome | CR-ES-004 §10 + ADR-ES-004 §14 |
| agent | adapts-to | external:concept:context | CR-ES-004 §10 + ADR-ES-004 §7.6 |
| agent | receives | intent | CR-ES-004 §10 + ADR-ES-004 §14 |
| intent | guides | action | CR-ES-004 §10 + ADR-ES-004 §14 |
| authority | constrains | action | CR-ES-004 §10 + ADR-ES-004 §14 + §15 |
| action | action-produces | external:concept:outcome | CR-ES-004 §10 + ADR-ES-004 §14 |

## Subject groupings

### Agent subject (8 predicates)

The Agent is the primary actor ;;; the 8 Agent predicates cover: interpretation (interprets, receives), pursuit (pursues), authority-bounded action (acts-within), action selection/coordination (selects, coordinates), outcome production (agent-produces), and adaptation (adapts-to).

### Intent subject (1 predicate)

`Intent guides Action` ;;; Intent informs Action without prescribing it.

### Authority subject (1 predicate)

`Authority constrains Action` ;;; Authority limits Action's allowed scope.

### Action subject (1 predicate)

`Action action-produces Outcome` ;;; Action results in the intended state.

## Namespacing notes

Two predicates are namespaced to disambiguate by subject_type:

- `produces` ;;; Value Stream subject (CR-ES-003 §10.5) vs `agent-produces` (Agent subject, CR-ES-004 §10) vs `action-produces` (Action subject, CR-ES-004 §10)
- Pattern follows `stage-realized-through` (Value Stage subject, VS-B) and `capability-realized-through` (Capability subject)

## Cross-references

- [Agent](../concepts/agent.md)
- [Agentic](../concepts/agentic.md)
- [Intent](../concepts/intent.md)
- [Authority](../concepts/authority.md)
- [Action](../concepts/action.md)
- [Value Stream Relationships](./value-stream-relationships.md) ;;; parallel predicate table for CR-ES-003

## Governance

- **Governing ADR:** ADR-ES-004 §14
- **Governing CR:** CR-ES-004 §10

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)