# Agentic Operations Boundary

Per CR-ES-007 §3 + ADR-ES-007 §28 ;; Agentic Operations is bounded
against 7 adjacent constructs.

## Scope

The Agentic Operations semantic is explicitly bounded against
constructs that must remain distinct. The boundary tests below
correspond to the conformance rules (AOP-CON-011..014) and the
rejected alternatives (ADR-ES-007 §28.1..§28.7).

## The 7 boundary distinctions

### AOP-INV-001 ;; Agentic Operations != AI Operations

Per ADR-ES-007 §14 + §28.1. AI is implementation technology ;;; not
the semantic basis of agency. An Agentic Operations may use AI ;;;
non-AI implementations are equally valid.

### AOP-INV-002 ;; Agentic Operations != Automated Operations

Per ADR-ES-007 §13 + §28.2. Automation is execution according to
predefined mechanisms. An Agentic Operations involves operational
sensing ;; interpretation ;;; dynamic decision ;;; and runtime
adaptation. Automation does not establish agentic behavior.

### AOP-INV-003 ;; Agentic Operations != Agentic Workflow

Per ADR-ES-007 §7 + §28.3. Workflow represents work coordination ;;
while Operations represents an ongoing operating mode. An Agentic
Operations may use Agentic Workflows ;; but is not itself a Workflow.

### AOP-INV-004 ;; Agentic Operations != Agentic Value Stream

Per ADR-ES-007 §8 + §28.4. Value realisation and operational
execution are distinct semantic concerns. An Agentic Value Stream
depends on Agentic Operations ;; but is not reducible to them.

### AOP-INV-005 ;; Agentic Operations != Autonomous Operations

Per ADR-ES-007 §15 + §28.5 + AOP-CON-012. Agency does not imply
autonomy. An Agentic Operations may remain supervised ;; policy-
controlled ;; approval-driven ;; bounded by human authority ;; partially
adaptive ;; constrained to predefined operational domains.

### AOP-INV-006 ;; Agentic Operations != Operations containing an Agent

Per ADR-ES-007 §28.6. Mere Agent presence does not establish
material agentic operational behavior. The material-participation
criterion requires:

```
Operational Context -> Sense -> Interpret -> Decide -> Coordinate
    -> Act -> Observe Outcome -> Adapt
```

with agentic behavior materially participating in one or more
points in the loop.

### AOP-INV-007 ;; Agentic Operations != AI-managed Enterprise Operations

Per ADR-ES-007 §28.7. The semantic applies to operational behavior
;; not to a specific technology architecture. Agentic Operations is
technology-neutral ;; AI is one possible implementation among many.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources