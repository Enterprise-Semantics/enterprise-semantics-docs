# Autonomous Operations Boundary

Per CR-ES-008 §3 + ADR-ES-008 §23 ;; Autonomous Operations is bounded
against 7 adjacent constructs.

## Scope

The Autonomous Operations semantic is explicitly bounded against
constructs that must remain distinct. The boundary tests below
correspond to the conformance rules (AOP-AUTO-CON-014..016) and the
rejected alternatives (ADR-ES-008 §23.1..§23.7).

## The 7 boundary distinctions

### AUTO-INV-001 ;; Autonomous Operations != AI Operations

Per ADR-ES-008 §19 + §23.1. AI is implementation technology ;;; not
the semantic basis of autonomy. An Autonomous Operations may use AI ;;;
non-AI implementations are equally valid.

### AUTO-INV-002 ;; Autonomous Operations != Agentic Operations

Per ADR-ES-008 §9 + §10 + §23.2. Agentic behavior describes a mode of
operation ;; while autonomy describes independent operational
execution. The two are orthogonal ;; not nested. An Autonomous
Operations may be agentic ;; or may be implemented via automation
;; systems ;; control systems ;;; or other mechanisms.

### AUTO-INV-003 ;; Autonomous Operations != Automation

Per ADR-ES-008 §11 + §23.3. Automation executes according to
predefined mechanisms ;; while Autonomous Operations independently
determine operational responses within defined boundaries. The
presence of Automation does not establish Autonomous Operations.

### AUTO-INV-004 ;; Autonomous Operations != Unattended Operations

Per ADR-ES-008 §23.4. Autonomy does not require complete absence of
humans. An Autonomous Operations may operate with human oversight
;; human escalation ;; human emergency override ;; and other human
governance.

### AUTO-INV-005 ;; Autonomous Operations != Human-free Operations

Per ADR-ES-008 §23.5. Human governance ;; intervention ;; and
escalation remain compatible with Autonomous Operations. The semantic
boundary is independence from per-action human intervention ;; not
independence from human governance.

### AUTO-INV-006 ;; Autonomous Operations != Unlimited Operations

Per ADR-ES-008 §14 + §23.6. Autonomy remains bounded by authority ;;;
policy ;;; and constraints. An Autonomous Operations does not have
unlimited authority merely because it can act without immediate
human intervention.

### AUTO-INV-007 ;; Autonomous Operations != Autonomous Agent as universal Entity subtype

Per ADR-ES-008 §6 + §23.7. Autonomy can apply to operations ;;;
workflows ;; systems ;; services ;; agents ;; vehicles ;; networks
;;; enterprises ;; ecosystems ;;; without prematurely defining every
autonomous thing as a new universal Entity ontology class.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources