# Enterprise Agentic / Autonomous Matrix

Per CR-ES-011 §19 + ADR-ES-011 §5 + §11.

## Scope

This document presents the four-state matrix that distinguishes the
Agentic Enterprise and Autonomous Enterprise classifications. The
matrix preserves the orthogonality invariant AE-AUTO-CON-013.

## The four-state matrix

Per ADR-ES-010 §13 + ADR-ES-011 §5 + §11:

| State | Agentic? | Autonomous? | Interpretation
|------  |---------  |------------  | --------------------------------------------
| 1     | No        | No           | Conventional / mixed enterprise
| 2     | Yes       | No           | Agentic Enterprise
| 3     | No        | Yes          | Autonomous Enterprise
| 4     | Yes       | Yes          | Agentic + Autonomous Enterprise

State 4 is a valid combination of semantic characteristics; it does
NOT result in creation of a new canonical concept. The two
specialisations are independent semantic dimensions.

## Authority and governance

All four states preserve:

- Authority: required, bounded
- Governance: required (policies, constraints, escalation,
  intervention)
- Human participation: permitted (human-in-the-loop, on-the-loop,
  over-the-loop)

The dimensions that differ across the four states are:

- Agentic behaviour (states 2 and 4)
- Independent progression (states 3 and 4)

## Architectural consequence

Per ADR-ES-011 §11:

The valid architectural position for an enterprise instance is:

```
Enterprise
   |
   +-- (optional) Agentic Enterprise specialisation
   |
   +-- (optional) Autonomous Enterprise specialisation
```

Each specialisation is independent. Both may be present on the same
enterprise instance.

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B.
- Vendor-specific embargo: zero references.
