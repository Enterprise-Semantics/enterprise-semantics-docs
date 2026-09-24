# Autonomous Operations Relationships

Per CR-ES-008 §9 + ADR-ES-008 §17 ;; the 10 canonical Autonomous
Operations predicates.

## Predicate table

| Subject | Predicate | Object | Provenance |
|---|---|---|---|
| ES:CONCEPT:autonomous-operations | specializes | ES:CONCEPT:operations | CR-ES-008 §3 + §9.1 + ADR-ES-008 §1 + §17 |
| ES:CONCEPT:autonomous-operations | operates-within | ES:CONCEPT:authority | ADR-ES-008 §5 + §14 + §17 + CR-ES-008 §9.2 |
| ES:CONCEPT:autonomous-operations | governed-by | external:concept:policy | ADR-ES-008 §14 + §17 + CR-ES-008 §9.3 |
| ES:CONCEPT:autonomous-operations | pursues | external:concept:operational-objective | ADR-ES-008 §5 + §14 + §17 + CR-ES-008 §9.4 |
| ES:CONCEPT:autonomous-operations | responds-to | external:concept:operational-context | ADR-ES-008 §5 + §17 + CR-ES-008 §9.5 |
| ES:CONCEPT:autonomous-operations | produces | external:concept:operational-outcome | ADR-ES-008 §13 + §17 + CR-ES-008 §9.6 |
| ES:CONCEPT:autonomous-operations | adapts-to | external:concept:operational-context | ADR-ES-008 §5 + §7.7 + §17 + CR-ES-008 §9.5 |
| ES:CONCEPT:autonomous-operations | escalates-to | external:concept:human-authority | ADR-ES-008 §7.8 + §8 + §17 + CR-ES-008 §9.7 |
| ES:CONCEPT:autonomous-operations | uses | ES:CONCEPT:workflow | ADR-ES-008 §12 + §17 + CR-ES-008 §9.8 |
| ES:CONCEPT:autonomous-operations | uses | ES:CONCEPT:agentic-workflow | ADR-ES-008 §12 + §17 + CR-ES-008 §9.8 |

## Notes

- `Policy`, `Operational Objective`, `Operational Context`, 
  `Operational Outcome`, and `Human / Authority` are
  forward-references ;; not yet canonicalised as Enterprise-Semantics
  concept records. Per CR-ES-008 §5 ;; they remain governed as
  external concepts.
- The Authority semantics are inherited from CR-ES-004.
- The Workflow semantics are inherited from CR-ES-001.
- The Agentic Workflow semantics are inherited from CR-ES-006.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean
- No embargo refs