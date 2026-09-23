# Agentic Operations Relationships

Per CR-ES-007 §8 + ADR-ES-007 §21 ;; the 9 canonical Agentic Operations
predicates.

## Predicate table

| Subject | Predicate | Object | Provenance |
|---|---|---|---|
| ES:CONCEPT:agentic-operations | specializes | ES:CONCEPT:operations | CR-ES-007 §3 + ADR-ES-007 §2 + §21 |
| ES:CONCEPT:agentic-operations | engages | ES:CONCEPT:agent | ADR-ES-007 §11 + §21 + CR-ES-007 §8.2 |
| ES:CONCEPT:agentic-operations | responds-to | external:concept:operational-context | ADR-ES-007 §21 + CR-ES-007 §8.3 |
| ES:CONCEPT:agentic-operations | operates-within | ES:CONCEPT:authority | ADR-ES-007 §21 + CR-ES-007 §8.4 |
| ES:CONCEPT:agentic-operations | governed-by | external:concept:policy | ADR-ES-007 §21 + CR-ES-007 §8.5 |
| ES:CONCEPT:agentic-operations | coordinates | external:concept:process | ADR-ES-007 §10 + §21 + CR-ES-007 §8.6 |
| ES:CONCEPT:agentic-operations | uses | ES:CONCEPT:agentic-workflow | ADR-ES-007 §9 + §21 + CR-ES-007 §8.7 |
| ES:CONCEPT:agentic-operations | produces | external:concept:operational-outcome | ADR-ES-007 §18 + §21 + CR-ES-007 §8.8 |
| ES:CONCEPT:agentic-operations | adapts-to | external:concept:operational-context | ADR-ES-007 §21 + CR-ES-007 §8.3 |

## Notes

- `Operational Context` ;; `Policy` ;; `Process` ;; and `Operational
  Outcome` are forward-references ;; not yet canonicalised as
  Enterprise-Semantics concept records. Per CR-ES-007 §27 ;; they
  remain governed as external concepts.
- The Agent semantics are inherited from CR-ES-004 + ADR-ES-004.
- The Authority semantics are inherited from CR-ES-004.
- The Agentic Workflow semantics are inherited from CR-ES-006.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean
- No embargo refs