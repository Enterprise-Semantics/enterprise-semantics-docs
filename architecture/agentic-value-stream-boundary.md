# Agentic Value Stream Boundary

## Scope

Per CR-ES-005 §3 + ADR-ES-005 §11 + §12 + §13 + §14 + §10 ;; the
Agentic Value Stream semantic is explicitly bounded against 6
adjacent constructs that must NOT be canonicalised as synonyms or
equivalences.

## 6 boundary distinctions

| # | Construct | Boundary | Source |
|---|-----------|----------|--------|
| 1 | AI Value Stream | NOT canonicalised | ADR-ES-005 §11 + AG-INV-001 + AG-INV-004 |
| 2 | Automated Value Stream | NOT canonicalised | ADR-ES-005 §12 + AG-INV-002 |
| 3 | Autonomous Value Stream | NOT canonicalised | ADR-ES-005 §13 + AG-INV-003 |
| 4 | Agentic Workflow | NOT canonicalised | ADR-ES-005 §14 + AG-INV-007 + CR-ES-005 §3 |
| 5 | Agentic Operations | NOT canonicalised | ADR-ES-005 §14 + AG-INV-007 + CR-ES-005 §3 |
| 6 | Process / Workflow | NOT redefined | ADR-ES-005 §10 + CAP-INV-001 |

## Boundary assertions

### AI != Agentic Value Stream

Per ADR-ES-005 §11:

- AI may implement an Agent
- An Agent may use AI
- An Agent may alternatively be implemented through software ;; a
  socio-technical mechanism ;; or another entity capable of satisfying
  the Agent semantics.

Therefore:

- AI != Agent
- AI != Agentic
- Agentic Value Stream != AI Value Stream

AI-based agents are an implementation possibility ;; NOT a semantic
requirement.

### Automation != Agentic

Per ADR-ES-005 §12:

- Automation executes predefined rules ;; trigger -> predefined rule
  -> predefined action.
- Agentic behavior involves delegated intent ;; context ;; action
  selection ;; execution ;; outcome ;; contextual adaptation.

Automation may participate in an Agentic Value Stream without itself
being agentic.

### Agentic Value Stream != Autonomous Value Stream

Per ADR-ES-005 §13:

An Agentic Value Stream may operate with:

- human approval
- human escalation
- constrained agent authority
- policy-controlled decisions
- fixed organizational boundaries
- externally established objectives

Autonomy is a separate semantic dimension. A future Autonomous Value
Stream ADR may establish additional criteria for self-governance ;;
self-directed adaptation ;; or reduced external intervention. Such
semantics are explicitly outside CR-ES-005.

### Agentic Value Stream != Agentic Workflow

Per ADR-ES-005 §14 + CR-ES-005 §3:

Agentic Workflow is held for ADR-ES-006. Per CR-ES-005 §14 ;; the
following semantics are sufficient for CR-ES-005:

```
Agentic Value Stream
        |
        v
engages
        |
        v
Agent
```

More specialized execution relationships should be introduced only
when their corresponding concepts become canonical.

### Agentic Value Stream != Agentic Operations

Per ADR-ES-005 §14 + CR-ES-005 §3:

Agentic Operations is held for ADR-ES-007. The Agentic Value Stream
CR does not establish Agentic Operations.

### Agentic Value Stream != Process / Activity / Task / Workflow

Per ADR-ES-005 §10 + CAP-INV-001:

The execution boundary remains intact:

```
VALUE REALIZATION
-----------------------------
Agentic Value Stream
        |
        v
Value Stage
-----------------------------
WORK ORGANIZATION
        |
        v
Process
        |
        v
Activity
        |
        v
Task
-----------------------------
EXECUTION / COORDINATION
        |
        v
Workflow / Task Flow
-----------------------------
IMPLEMENTATION
        |
        v
Service / System / Resource / Technology
```

Agentic behavior may influence any appropriate execution layer ;; but
this does NOT make those layers semantically equivalent.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources