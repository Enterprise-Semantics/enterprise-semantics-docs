# Agentic vs Autonomous Operations

Per CR-ES-008 §10 + ADR-ES-008 §10 + §26.

## Scope

Agentic Operations and Autonomous Operations are distinct semantic
concepts operating at different semantic dimensions. They are
orthogonal ;; not nested ;; not equivalent.

## The architectural distinction

Per ADR-ES-008 §10 + CR-ES-008 §11 ;; a multi-dimension comparison:

| Dimension | Agentic Operations | Autonomous Operations |
|---|---|---|
| Core semantic | Mode of operation | Independent execution characteristic |
| Key question | How is operational behavior performed? | How independently can it operate? |
| Delegated intent | Required | Normally required |
| Authority | Required | Required |
| Context interpretation | Characteristic | Required for contextual autonomy |
| Action selection | Characteristic | Required where decisions are autonomous |
| Human participation | Fully compatible | Fully compatible |
| Human intervention | May be frequent | Not required for every operational action |
| AI | Not required | Not required |
| Automation | Not required | Not required |
| Autonomy | Not implied | Defining characteristic |
| Escalation | Supported | Required for boundary conditions |
| Operational scope | Operations | Operations |

## Boundary tests

### Test 1 ;; Agentic Operations != Autonomous Operations

```
Agentic Operations -[is-a]-> Autonomous Operations ;; INVALID
Autonomous Operations -[is-a]-> Agentic Operations ;; INVALID
```

The concepts are orthogonal per ADR-ES-008 §9 + §26 + CR-ES-008 §10.

### Test 2 ;; Agentic Operations may exhibit Autonomous behavior

```
Agentic Operations -[may exhibit]-> Autonomous behavior ;; VALID
```

Per ADR-ES-008 §9 + CR-ES-008 §10, Agentic Operations may exhibit
autonomous behavior ;; but this does not establish a specialisation
relationship.

### Test 3 ;; Autonomous Operations uses Agentic Operations

```
Autonomous Operations -[uses]-> Workflow ;; VALID
Autonomous Operations -[uses]-> Agentic Workflow ;; VALID
Autonomous Operations -[engages]-> Agent ;; VALID
```

Per ADR-ES-008 §12 + §17 + CR-ES-008 §11, Autonomous Operations
may use workflows (conventional or Agentic) and engage Agents, but
does not specialise any of them.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources