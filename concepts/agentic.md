# Agentic

## Definition

Per CR-ES-004 §6 + ADR-ES-004 §4.1 + §6:

> Agentic is a mode of operation in which an Agent interprets a
> delegated objective or intent, determines or selects actions
> within defined authority, and acts or coordinates actions toward
> an intended outcome.

## Semantic type

**SemanticProperty** (not Entity subtype), per ADR-ES-004 §6, Agentic is a mode of operation, not a universal Entity subtype. This prevents the ontology from unnecessarily turning every agentic construct into a new top-level entity class.

## Distinctions

Per ADR-ES-004 §8-§10 + §14:

- **Agentic != AI** (AG-INV-001)
- **Agentic != Automation** (AG-INV-002)
- **Agentic != Autonomous** (AG-INV-003)
- **Agent != AI Agent** (AG-INV-004)

## 6 Characteristics

Per ADR-ES-004 §7.1-§7.6:

1. **Delegated Intent**, an objective, intent, goal, or desired outcome is delegated to the Agent
2. **Context Interpretation**, the Agent interprets relevant context rather than executing predefined sequences
3. **Action Selection**, the Agent can select, sequence, or coordinate actions
4. **Bounded Authority**, the Agent operates within explicit or implicit authority boundaries
5. **Outcome Orientation**, actions are directed toward an intended outcome
6. **Adaptation**, the Agent may alter its execution path in response to changing conditions

## Human participation does not invalidate Agentic semantics

Per ADR-ES-004 §16, human-in/on/over-the-loop patterns all represent agentic operating patterns.

## Architectural invariants

Per ADR-ES-004 §20, 10 invariants AG-INV-001..010:

- AG-INV-001, Agentic != AI
- AG-INV-002, Agentic != Automation
- AG-INV-003, Agentic != Autonomous
- AG-INV-004, Agent != AI Agent
- AG-INV-005, Agentic operation requires delegated intent or objective
- AG-INV-006, Agentic operation occurs within defined authority
- AG-INV-007, Agentic operation is outcome-oriented
- AG-INV-008, Human participation does not invalidate Agentic semantics
- AG-INV-009, Agentic Value Stream is a specialization of Value Stream, not a replacement for Value Stream (held for ADR-ES-005)
- AG-INV-010, Autonomy requires separate semantic grounding (ADR-ES-007)

## Governance

- **Source:** enterprise-semantics/concepts/agentic.concept.yaml
- **Governing ADR:** ADR-ES-004 §4.1 + §6
- **Governing CR:** CR-ES-004 §6

## See also

- [Agent](./agent.md)
- [Agentic vs Autonomous Boundary](../architecture/agentic-autonomous-boundary.md)
- [Agentic Execution Pattern Boundary](../architecture/agentic-execution-boundary.md)
- [Agentic vs Automation Boundary](../architecture/agentic-boundary.md)

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)