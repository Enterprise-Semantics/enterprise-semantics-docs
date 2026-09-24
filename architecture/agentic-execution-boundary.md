# Agentic Execution Pattern Boundary

Per CR-ES-004 §11 + ADR-ES-004 §11, the boundary between Agentic execution and conventional Workflow execution.

## Two patterns

**Conventional Workflow execution:**

```text
Workflow
  :
  v
conventional execution (predefined steps)
```

**Agentic execution:**

```text
Workflow
  :
  v
MAY be realized agentically (CR-ES-004 establishes boundary, not AgenticWorkflow canonical concept)
  :
  v
agentic participation in:
  - planning
  - interpretation
  - sequencing
  - decision selection
  - execution
  - adaptation
  - coordination
```

## Boundary tests

Per ADR-ES-004 §11:

- **Workflow may be realized agentically**, but AgenticWorkflow is NOT a canonical semantic concept in CR-ES-004
- **Agentic Workflow is established by ADR-ES-006**, CR-ES-004 only establishes the preparatory boundary
- **Agentic Workflow boundary is documented, no canonical specialization yet**, per CR-ES-004 §3 + §15

## Operations boundary (parallel)

Per CR-ES-004 §16 + ADR-ES-004 §12:

```text
Operations
  :
  v
may be performed agentically
  :
  v
Agentic Operations is NOT canonical in CR-ES-004, boundary established for ADR-ES-007
```

## Value Stream boundary (preliminary)

```text
Value Stream
  :
  v
uses / involves --> Agent
  :
  v
Agentic Value Stream is NOT canonical in CR-ES-004, boundary established for ADR-ES-005
```

## What is established by CR-ES-004

- The 3 boundaries (Workflow, Operations, Value Stream) are documented as potential Agentic modes
- No canonical specialization is established
- The semantic extension points are reserved for ADR-ES-005 (Agentic Value Stream), ADR-ES-006 (Agentic Workflow), ADR-ES-007 (Agentic Operations)

## Cross-references

- [Agent](../concepts/agent.md)
- [Agentic](../concepts/agentic.md)
- [Value Stream](./value-stream-process-boundary.md), parallel boundary documentation
- [Value Realization](./value-realization-boundary.md), parallel boundary documentation

## Governance

- **Governing ADR:** ADR-ES-004 §11 + §12 + §13
- **Governing CR:** CR-ES-004 §15 + §16 + §17

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)