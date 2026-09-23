# Value Stream <> Agentic Value Stream Boundary

## Scope

Per CR-ES-005 §8 + ADR-ES-005 §6 ;; the Agentic Value Stream semantic
preserves the Value Stream semantics established by CR-ES-003.

## Value Stream semantics (preserved)

Per CR-ES-005 §8 ;; the Agentic Value Stream schema preserves the
mandatory Value Stream semantics:

- stakeholder
- initiating_condition
- realization_boundary
- stages
- outcomes
- relationships
- grounding
- provenance
- version

The implementation does NOT duplicate or redefine these properties
where inheritance/reference is supported by the repository schema
architecture.

## Agentic Value Stream semantics (added)

Per CR-ES-005 §5 + ADR-ES-005 §8 ;; the Agentic Value Stream adds:

- agentic_scope
- delegated_intent
- authority_context
- decision_boundary
- intervention_model
- adaptation_scope
- realization_mode

## Inheritance principle

Per ADR-ES-005 §6 ;; agentic behavior may occur within one or more
existing Value Stages:

```
Value Stream
    |
    v
contains
    |
    v
Value Stage
    |
    v
may be realized agentically
```

A new Agentic Value Stage concept is NOT established by CR-ES-005.

This preserves the distinction between:

- what transition in value occurs ;; Value Stage
- how that transition is realized ;; Process and its execution
  mechanisms
- whether agentic behavior participates ;; Agentic realization

## Stage realisation modes

Per CR-ES-005 §11 + ADR-ES-005 §5 ;; agentic coverage is contextual
;; not binary at the entire-stream level.

A valid Agentic Value Stream may contain:

- Conventional execution
- Automated execution
- Human decision
- Agentic decision
- Agentic coordination
- Human intervention

For example:

```
Order-to-Cash
  Order Capture          Conventional
  Order Validation       Agentic
  Credit Decision        Human / Agentic
  Fulfillment Selection  Agentic
  Delivery               Automated / Conventional
  Exception Management   Agentic
  Settlement             Automated
```

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources