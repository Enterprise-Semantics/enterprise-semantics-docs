# Agentic Workflow Boundary

Per CR-ES-006 §3 + ADR-ES-006 §10 + §11 + §12 + §13 + §14 + §15 + §16
+ §17 + §24.

## Scope

The Agentic Workflow semantic is explicitly bounded against 8
adjacent constructs that must remain distinct. The boundary tests
below correspond to the conformance rules (AWF-CON-009..014) and
the rejected alternatives (ADR-ES-006 §24.1..§24.6).

## The 8 boundary distinctions

### AWF-INV-001 ;; Agentic Workflow != AI Workflow

Per ADR-ES-006 §14 + §24.1. AI is implementation technology ;;; not
the semantic basis of agency. An Agentic Workflow may be implemented
using AI-based Agents ;; rule-based Agents ;; software Agents ;; or
socio-technical Agents.

### AWF-INV-002 ;; Agentic Workflow != Automated Workflow

Per ADR-ES-006 §13 + §24.2. Automation is execution according to
predefined mechanisms. An Agentic Workflow involves interpretation ;;;
action/path selection ;; and dynamic decision-making. Automation does
not establish agentic interpretation.

### AWF-INV-003 ;; Agentic Workflow != Autonomous Workflow

Per ADR-ES-006 §17 + §24.3. Agency does not imply autonomy. An
Agentic Workflow operates with human approval ;; human escalation ;;;
constrained authority ;; predefined policies ;; supervised execution ;;;
and externally established objectives.

### AWF-INV-004 ;; Agentic Workflow != Process

Per ADR-ES-006 §6 + §24.4. Process represents organised work ;; while
Workflow represents its coordination or execution. Agentic Workflow
realises a Process but is not itself a Process.

### AWF-INV-005 ;; Agentic Workflow != Workflow merely containing an Agent

Per ADR-ES-006 §10 + §24.5. Merely invoking an Agent does not make a
Workflow an Agentic Workflow. The material-participation criterion
requires:

```
Agent interprets context
-> Agent selects permitted path
-> Workflow adapts
```

### AWF-INV-006 ;; Agentic Workflow != Agentic Value Stream

Per ADR-ES-006 §15 + §24.6. Value realisation and work execution
operate at different semantic levels. Agentic Value Stream is the
value-realisation construct ;; Agentic Workflow is the execution-level
construct.

### AWF-INV-007 ;; Agentic Workflow != Value Stream

Per AWF-CON-012. Agentic Workflow is not a Value Stream. Workflow is
the execution layer ;;; Value Stream is the value-realisation layer.

### AWF-INV-008 ;; Agentic Workflow != Agent

Per AWF-CON-013. Agentic Workflow is not an Agent. Agentic Workflow
engages Agents ;; but is itself the coordination structure.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources