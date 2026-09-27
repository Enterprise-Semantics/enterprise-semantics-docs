# Autonomous Enterprise Boundary

Per CR-ES-011 §18 + ADR-ES-011 §1 + §3.1 + §6.

## Scope

The Autonomous Enterprise semantic is explicitly bounded against
adjacent constructs. The boundary distinctions below correspond to
the conformance rules (AE-AUTO-CON-001 through AE-AUTO-CON-022)
and the rejected alternatives (ADR-ES-011 §26).

## The boundary diagram

```
Enterprise Boundary (semantic, not strict containment)
+-----------------------------------------------+
|                                               |
|             Autonomous Enterprise             |
|                                               |
|  Enterprise Boundary                          |
|     -> Autonomous Enterprise                  |
|  Value Boundary                               |
|     -> Autonomous Value Stream                |
|  Operational Boundary                         |
|     -> Autonomous Operations                  |
|  Execution Boundary                           |
|     -> Workflow / Agentic Workflow           |
|  Implementation Boundary                      |
|     -> Agent / Human / System / Service      |
|                                               |
+-----------------------------------------------+
```

The diagram explicitly states that these are **semantic
boundaries** rather than a strict containment hierarchy
(per CR-ES-011 §18).

## Boundary distinctions

Per ADR-ES-011 §26:

### Autonomous Enterprise != AI Enterprise
Per ADR-ES-011 §16 + AE-AUTO-NEG-005. AI is neither necessary nor
sufficient for Autonomous Enterprise.

### Autonomous Enterprise != Automated Enterprise
Per ADR-ES-011 §17 + AE-AUTO-NEG-006. Automation alone does not
establish Autonomous Enterprise.

### Autonomous Enterprise != Agentic Enterprise
Per ADR-ES-011 §11 + AE-AUTO-CON-013 + AE-AUTO-NEG-003 + AE-AUTO-NEG-009.
The two are orthogonal semantic dimensions, not a hierarchy.

### Autonomous Enterprise != Enterprise containing Autonomous Operations
Per AE-AUTO-NEG-007 + AE-AUTO-CON-015. Autonomous Operations alone
do not establish Autonomous Enterprise.

### Autonomous Enterprise != Enterprise containing Autonomous Value Streams
Per AE-AUTO-NEG-008 + AE-AUTO-CON-016. Autonomous Value Streams
alone do not establish Autonomous Enterprise.

### Autonomous Enterprise != Enterprise containing Agents
Per AE-AUTO-NEG-017 (parallel). Merely possessing Agents does
not establish Autonomous Enterprise.

### Autonomous Enterprise != Human-free Enterprise
Per AE-AUTO-NEG-012 + AE-AUTO-NEG-013 + AE-AUTO-CON-010. Human
participation is permitted and required for governance.

### Autonomous Enterprise != Unsupervised Enterprise
Per ADR-ES-011 §9. Human governance is required.

### Autonomous Enterprise != Unlimited authority
Per AE-AUTO-NEG-014 + AE-AUTO-CON-018. Authority is bounded.

### Autonomous Enterprise != Self-governing without objectives
Per ADR-ES-011 §10 + AE-AUTO-CON-004. Objectives are required.

### Autonomous Enterprise != Autonomous Workflow
Per AE-AUTO-NEG-015 + AE-AUTO-CON-020. Autonomous Workflow is
held as a future concept per CR-ES-011 §27.

### Autonomous Enterprise != Autonomous Agent
Per AE-AUTO-NEG-016 + AE-AUTO-CON-021. Autonomous Agent is held
as a future concept per CR-ES-011 §27.

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B.
- Vendor-specific embargo: zero references.
