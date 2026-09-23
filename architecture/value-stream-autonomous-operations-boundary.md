# Autonomous Value Stream <> Autonomous Operations Boundary

Per CR-ES-009 §14 + ADR-ES-009 §9 + §14.

## Scope

The Autonomous Value Stream may use Autonomous Operations ;; but the
two are distinct semantic concepts at different layers.

## The architectural distinction

Per ADR-ES-009 §9 + §14 + CR-ES-009 §14 ;; a multi-dimension
comparison:

| Dimension | Autonomous Value Stream | Autonomous Operations |
|---|---|---|
| Primary concern | Stakeholder value realization | Operational execution |
| Anchor | Stakeholder Value | Operational Outcome |
| Boundary | End-to-end Value Stream | Operating environment |
| Structure | Value Stages | Processes, workflows, operations |
| Autonomy applies to | Value realization | Operational behavior |
| Scope | End-to-end value journey | Operational domain |
| May use | Autonomous Operations | Value Streams |
| Stakeholder relationship | Fundamental | Indirect |
| Human participation | Compatible | Compatible |
| AI | Not required | Not required |

## Boundary tests

### Test 1 ;; Autonomous Value Stream != Autonomous Operations

```
Autonomous Value Stream -[is-a]-> Autonomous Operations ;; INVALID
Autonomous Operations -[is-a]-> Autonomous Value Stream ;; INVALID
```

The two are orthogonal ;; per ADR-ES-009 §9 + §14 + §22 + CR-ES-009 §14.

### Test 2 ;; Autonomous Value Stream uses Autonomous Operations

```
Autonomous Value Stream -[uses]-> Autonomous Operations ;; VALID
```

Per ADR-ES-009 §14 ;; the relationship is permitted ;; not
mandatory. A Value Stream may achieve autonomous value realization
through other autonomous mechanisms.

### Test 3 ;; Autonomous Operations supports multiple Value Streams

```
Autonomous Operations -[supports]-> Autonomous Value Stream A ;; VALID
Autonomous Operations -[supports]-> Autonomous Value Stream B ;; VALID
```

Per ADR-ES-009 §14 + §22 + CR-ES-009 §14 ;; an Autonomous Operations
capability may support multiple Value Streams.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources