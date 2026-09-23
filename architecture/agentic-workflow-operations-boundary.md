# Agentic Workflow <> Agentic Operations Boundary

Per CR-ES-007 §10 + ADR-ES-007 §7 + §9.

## Scope

Agentic Workflow and Agentic Operations are distinct semantic
concepts operating at different layers. The boundary is preserved as
a key architectural invariant.

## The architectural distinction

Per ADR-ES-007 §23 + CR-ES-007 §10 ;; a multi-dimension comparison:

| Dimension | Agentic Workflow | Agentic Operations |
|---|---|---|
| Primary concern | Work coordination/execution | Ongoing operational behavior |
| Semantic scope | Workflow | Operational environment |
| Time horizon | Workflow execution | Continuous/ongoing operation |
| Context | Workflow context | Operational context |
| Decision focus | Work path/action | Operational response |
| Adaptation | Workflow execution | Operational behavior |
| Process relationship | Realizes/executes work | Coordinates operational processes |
| Agent relationship | Engages Agents | May coordinate multiple Agents |
| Workflow relationship | Is a Workflow specialisation | May use multiple Workflows |
| AI requirement | None | None |
| Autonomy implication | None | None |

## Boundary tests

### Test 1 ;; Agentic Operations != Agentic Workflow

```
Agentic Operations -[is-a]-> Agentic Workflow ;; INVALID
```

Agentic Operations uses Agentic Workflows ;;; but is not one. A
Workflow does not become an Operating Mode merely because it
contains an Agent.

### Test 2 ;; Agentic Operations uses Agentic Workflow

```
Agentic Operations -[uses]-> Agentic Workflow ;; VALID
```

The canonical relationship is Agentic Operations uses Agentic
Workflow ;; per ADR-ES-007 §9 + CR-ES-007 §8.7.

### Test 3 ;; Agentic Operations coordinates Processes

```
Agentic Operations -[coordinates]-> Process ;; VALID
```

Per ADR-ES-007 §10 + CR-ES-007 §8.6 ;; Agentic Operations may
coordinate one or more Processes.

### Test 4 ;; Agentic Operations engages multiple Agents

```
Agentic Operations -[engages]-> Agent A ;; VALID
Agentic Operations -[engages]-> Agent B ;; VALID
```

Per ADR-ES-007 §11 ;; Agentic Operations may engage multiple Agents.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources