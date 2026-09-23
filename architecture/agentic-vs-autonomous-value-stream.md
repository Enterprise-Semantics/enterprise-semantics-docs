# Agentic vs Autonomous Value Stream

Per CR-ES-009 §10 + ADR-ES-009 §3 + §8 + §23.

## Scope

Agentic Value Stream and Autonomous Value Stream are distinct
semantic concepts operating at different semantic dimensions. They
are orthogonal ;; not nested ;; not equivalent.

## The architectural distinction

Per ADR-ES-009 §10 + CR-ES-009 §10 ;; a multi-dimension comparison:

| Dimension | Agentic Value Stream | Autonomous Value Stream |
|---|---|---|
| Core characteristic | Agentic behavior | Independent value realization |
| Key question | How does value realization behave? | How independently can value realization progress? |
| Agent required | Where agentic behavior is asserted | Not necessarily |
| Human intervention | Fully compatible | Not required for every value-realization action |
| AI | Not required | Not required |
| Automation | Not required | Not required |
| Autonomy | Not implied | Defining characteristic |
| Relationship to Operations | May use Agentic Operations | May use Autonomous Operations |

## Boundary tests

### Test 1 ;; Agentic Value Stream != Autonomous Value Stream

```
Agentic Value Stream -[is-a]-> Autonomous Value Stream ;; INVALID
Autonomous Value Stream -[is-a]-> Agentic Value Stream ;; INVALID
```

The concepts are orthogonal per ADR-ES-009 §3 + §8 + §23.

### Test 2 ;; Combinations are valid

```
Value Stream
   |-- Agentic Value Stream + Autonomous characteristic (both)
   |-- Agentic Value Stream only (e.g. Agentic + human approval)
   |-- Autonomous Value Stream only (e.g. Autonomous rule/control)
   |-- Neither (e.g. Human-led conventional)
```

Per ADR-ES-009 §8 ;; the semantic model SHALL not infer one
characteristic from the other.

### Test 3 ;; Autonomous Value Stream uses Agentic Operations

```
Autonomous Value Stream -[uses]-> Autonomous Operations ;; VALID
Autonomous Value Stream -[uses]-> Agentic Operations ;; VALID
```

Per ADR-ES-009 §12 + CR-ES-009 §12 ;; agentic behavior and
autonomy are independent semantic dimensions ;; both may coexist.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources