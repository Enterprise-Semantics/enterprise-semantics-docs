# Agentic Enterprise Boundary

Per CR-ES-010 §10 + ADR-ES-010 §1 + §3 + §8.

## Scope

The Agentic Enterprise semantic is explicitly bounded against adjacent
constructs. The boundary tests below correspond to the conformance
rules (AE-CON-001 through AE-CON-022) and the rejected alternatives
(ADR-ES-010 §20).

## The boundary diagram

```
Enterprise Boundary
+-------------------------------------------+
|                                           |
|              Agentic Enterprise           |
|                                           |
|   Value Realization     Operations        |
|          |                  |             |
|   Agentic Value       Agentic Operations  |
|     Streams                |             |
|          |            Agentic Workflows   |
|          +--------------+                |
|                         |                |
|                    Agents / Humans /     |
|                    Systems / Services    |
|                                           |
+-------------------------------------------+
```

The diagram represents semantic participation and realisation, not
mandatory containment. An Agentic Enterprise may realise value through
mixes of agentic, autonomous, conventional, or hybrid value streams.

## Boundary distinctions

### AE-CON-001 ; Agentic Enterprise specialises Enterprise

Per ADR-ES-010 §1 + §3 + CR-ES-010 §2. Agentic Enterprise is a direct
specialisation of Enterprise. The specialisation establishes
enterprise-level operating condition, not a new universal kind.

### AE-CON-013 ; Agentic Enterprise != Enterprise containing Agentic Value Streams

Per ADR-ES-010 §14 + CR-ES-010 §22 + AE-NEG-015. The presence of
agentic value realisation in a value stream does NOT establish agentic
participation at the enterprise boundary. Enterprise-level evidence is
required.

### AE-CON-014 ; Agentic Enterprise != Enterprise containing Agentic Operations

Per ADR-ES-010 §15 + CR-ES-010 §22 + AE-NEG-014. The presence of
agentic operational behavior does NOT establish agentic participation
at the enterprise boundary. Enterprise-level evidence is required.

### AE-CON-015 ; Agentic Enterprise != Enterprise containing Agents

Per ADR-ES-010 §1 + AE-NEG-007. Merely possessing or deploying Agents
does NOT establish an Agentic Enterprise. The agentic behavior must
materially influence enterprise-level value realisation, operations,
decisions, coordination, execution, or adaptation.

### AE-NEG-016 ; Agentic Enterprise != Autonomous Enterprise

Per ADR-ES-010 §11 + ADR-ES-011 §11 + CR-ES-011 §5. Agentic Enterprise
and Autonomous Enterprise are orthogonal semantic dimensions, not
hierarchies. An enterprise may satisfy either, both, or neither.

### AE-CON-009 ; Agentic Enterprise != Human-free Enterprise

Per ADR-ES-010 §10 + §17 + AE-NEG-009. Human governance is compatible
with, and required by, Agentic Enterprise. The semantic boundary is
independence from per-decision human intervention, not independence
from human governance.

### AE-CON-010 + AE-NEG-001 ; Agentic Enterprise != AI Enterprise

Per ADR-ES-010 §11. AI is neither necessary nor sufficient for Agentic
Enterprise. AI may be an implementation mechanism for agentic behavior,
but the semantic definition of agentic is independent of AI.

### AE-CON-011 + AE-NEG-008 ; Agentic Enterprise != Automated Enterprise

Per ADR-ES-010 §12 + AE-NEG-008. Automation may coexist with Agentic
Enterprise, but automation alone does not establish agentic
participation. A deterministic automated mechanism executes predefined
behavior without interpreting delegated intent or selecting actions
contextually.

### AE-CON-018 ; Agentic Enterprise has bounded authority

Per ADR-ES-010 §1 + §17 + AE-NEG-010. An Agentic Enterprise instance
with `authority = unrestricted` fails conformance. Unlimited authority
is incompatible with the Agentic Enterprise semantic model.

### AE-NEG-013 ; Agentic Enterprise != Agentic Workflow

Per ADR-ES-010 §16 + AE-NEG-013. The presence of Agentic Workflows
does NOT establish agentic participation at the enterprise boundary.
A single Agentic Workflow is an execution mechanism, not an
enterprise-level operating condition.

## Boundary tests

The following boundary questions preserve the Agentic Enterprise
semantic:

1. Does agentic behavior materially influence enterprise-level value
   realisation, operations, decisions, coordination, execution, or
   adaptation?
2. Is the enterprise-level operating condition distinct from the
   presence of agentic subsystems?
3. Does the enterprise retain defined authority boundaries?
4. Does the enterprise retain defined policy and governance boundaries?
5. Is human participation compatible with the operating condition?

If question 1 is answered affirmatively with evidence at the
enterprise boundary, the Agentic Enterprise concept applies.

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B.
- Vendor-specific embargo: zero references to material from embargoed
  sources.
