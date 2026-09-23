# Agentic Workflow Relationships

Per CR-ES-006 §5 + ADR-ES-006 §18 ;; the 7 canonical Agentic Workflow
predicates.

## Predicate table

| Subject | Predicate | Object | Provenance |
|---|---|---|---|
| ES:CONCEPT:agentic-workflow | specializes | ES:CONCEPT:workflow | CR-ES-006 §5 + ADR-ES-006 §2 + §18 |
| ES:CONCEPT:agentic-workflow | engages | ES:CONCEPT:agent | ADR-ES-006 §18 + CR-ES-006 §11 |
| ES:CONCEPT:agentic-workflow | interprets | ES:CONCEPT:intent | ADR-ES-006 §18 + CR-ES-006 §12 |
| ES:CONCEPT:agentic-workflow | operates-within | ES:CONCEPT:authority | ADR-ES-006 §18 + CR-ES-006 §5 + §13 |
| ES:CONCEPT:agentic-workflow | coordinates | external:concept:activity | ADR-ES-006 §18 + CR-ES-006 §10 |
| ES:CONCEPT:agentic-workflow | coordinates | external:concept:task | ADR-ES-006 §18 + CR-ES-006 §10 |
| ES:CONCEPT:agentic-workflow | produces | external:concept:outcome | ADR-ES-006 §18 + CR-ES-006 §21 |
| external:concept:process | process-realized-through | ES:CONCEPT:agentic-workflow | ADR-ES-006 §6 + CR-ES-006 §9 |

## Notes

- The `process-realized-through` predicate is namespaced to
  disambiguate from `value-stream-realized-through` and
  `capability-realized-through`.
- `Activity`, `Task`, `Outcome` are forward-references ;;; they are not
  yet canonicalised as Enterprise-Semantics concept records. Per
  CR-ES-006 §6 + §10 ;; they remain governed as external concepts.
- The Agent, Intent, Authority, and Agent semantics are inherited
  from CR-ES-004 + ADR-ES-004.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean
- No embargo refs