# Agentic Enterprise vs Autonomous Enterprise

Per CR-ES-010 §13 + ADR-ES-010 §11 + ADR-ES-011 §11 + §13.

## Scope

The Agentic Enterprise and Autonomous Enterprise concepts are
orthogonal semantic dimensions at the enterprise boundary. This
document preserves the distinction between them.

## The dimensional distinction

Per ADR-ES-010 §5 + §11 + ADR-ES-011 §5 + §11:

| Dimension      | Meaning
|---------------  | --------------------------------------------------------------
| Agentic         | How behavior is performed through interpretation, action
|                | selection, coordination, and adaptation.
| Autonomous      | The degree to which behavior can progress independently
|                | without human intervention for every decision / action.
| AI              | A technological or computational capability.
| Automation      | A mechanism for executing predefined behavior.

Therefore:

- Agentic != Autonomous
- Autonomous != Agentic
- Autonomous != AI
- Autonomous != Automation

This is a foundational invariant that must be preserved across all
subsequent ADRs and CRs.

## The orthogonality matrix

Per ADR-ES-010 §13 + ADR-ES-011 §5 + §11:

An enterprise may be in one of four states:

| Agentic? | Autonomous? | Interpretation
|---------  |------------  | ---------------------------------------------
| No        | No           | Conventional / mixed enterprise
| Yes       | No           | Agentic Enterprise
| No        | Yes          | Autonomous Enterprise
| Yes       | Yes          | Agentic + Autonomous Enterprise

The fourth state is a valid combination of semantic characteristics.
It does NOT result in creation of a new canonical concept. The two
specialisations are independent semantic dimensions that may coexist
on the same enterprise instance.

## Comparison

Per CR-ES-010 §13 + ADR-ES-010 §11 + ADR-ES-011 §11:

| Dimension                 | Agentic Enterprise           | Autonomous Enterprise
|--------------------------  | ---------------------------  | ---------------------------
| Primary semantic dimension| Agentic behavior              | Independent progression
| Core question              | How is behavior performed?   | Can behavior progress
|                            |                               | independently?
| Intent                     | Delegated / established intent| Defined enterprise objective
| Decision                   | Interpretation and action     | Independent decision
|                            | selection                     | progression
| Action                     | Agentic selection /           | Independent authorized
|                            | coordination                  | execution
| Human participation        | Permitted                     | Permitted
| AI requirement              | No                            | No
| Automation requirement      | No                            | No (automation alone is
|                            |                               | not sufficient)
| Authority                   | Required                      | Required (bounded)
| Governance                  | Required                      | Required
| Autonomy                    | Not implied                   | Explicit
| Relationship                | Independent dimension         | Independent dimension
| Cardinal rule               | Agentic Enterprise is NOT    | Autonomous Enterprise is NOT
|                            | Autonomous Enterprise        | Agentic Enterprise

## Invariants

Per ADR-ES-010 §13 + ADR-ES-011 §13:

```
AE-CON-012    Agentic Enterprise does not imply Autonomous Enterprise
AE-NEG-016    Agentic Enterprise implies Autonomous Enterprise (FALSE)
AE-AUTO-CON   Autonomous Enterprise does not imply Agentic Enterprise
              (parallel invariant from ADR-ES-011 §13)
```

Both invariants must be preserved in the implementation. Neither
dimension reduces to the other. They are orthogonal specialisations of
Enterprise per ADR-ES-011 §11.

## Architectural position

Per ADR-ES-010 §4 + ADR-ES-011 §11:

```
                          Enterprise
                              |
                +-------------+-------------+
                |                           |
                v                           v
        Agentic Enterprise       Autonomous Enterprise
                |                           |
                +-------------+-------------+
                              |
                enterprise-level orthogonal modes
```

The two concepts may coexist on the same enterprise instance. The
valid intersection is `Agentic + Autonomous Enterprise`, which is a
valid combination of semantic characteristics, not a new canonical
concept.

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B.
- Vendor-specific embargo: zero references to material from embargoed
  sources.
