# Agentic Enterprise Value / Operations Boundary

Per CR-ES-010 §12 + ADR-ES-010 §5 + §14 + §15.

## Scope

The Agentic Enterprise concept sits above the value-realisation and
operational boundaries. The boundary diagram below shows how Agentic
Enterprise participates in value realisation and operations without
collapsing into either.

## The boundary diagram

```
                     AGENTIC ENTERPRISE
                            |
              +-------------+-------------+
              |                           |
              v                           v
      VALUE REALIZATION             OPERATIONS
              |                           |
              v                           v
    Agentic Value Stream        Agentic Operations
              |                           |
              |                           v
              |                  Agentic Workflow
              |                           |
              +-------------+-------------+
                            v
                  Agent / Human / System /
                  Service
```

The diagram represents semantic participation and realisation, not
mandatory containment. Agentic Enterprise may participate in value
realisation and operations through mixes of agentic, autonomous,
conventional, or hybrid mechanisms.

## Value realisation boundary

Per ADR-ES-010 §14 + CR-ES-010 §4:

Agentic Enterprise may realise value through Agentic Value Streams via
the governed `enterprise-realizes-through` predicate. The relationship
does NOT imply:

- Agentic Enterprise = Enterprise containing Agentic Value Streams (per
  AE-NEG-015).
- Agentic Value Stream = Agentic Enterprise (per AE-NEG-012).

The Agentic Value Stream is the value-realisation boundary. The
Agentic Enterprise is the enterprise boundary. The two are related
through participation, not through identity.

## Operational boundary

Per ADR-ES-010 §15 + CR-ES-010 §4:

Agentic Enterprise may operate through Agentic Operations via the
governed `enterprise-operates-through` predicate. The relationship
does NOT imply:

- Agentic Enterprise = Agentic Operations (per AE-NEG-011).
- Agentic Operations automatically establish Agentic Enterprise (per
  AE-NEG-014).

Agentic Operations are an important realisation mechanism. Agentic
Enterprise is the enterprise-level operating condition. The two are
related through participation, not through identity.

## Realisation-mode matrix

Per ADR-ES-010 §19 + ADR-ES-011 §5:

A valid Agentic Enterprise may contain a mixture of realisation modes:

```
Mode                           Allowed in Agentic Enterprise?
-----------------------------  ------------------------------
Agentic Value Stream            yes (via enterprise-realizes-through)
Autonomous Value Stream         yes (parallel to Agentic Value Stream)
Conventional Value Stream       yes
Agentic Operations              yes (via enterprise-operates-through)
Autonomous Operations           yes (parallel to Agentic Operations)
Conventional Operations         yes
Human-led Operations            yes
Agentic Workflow                yes (as execution mechanism)
Autonomous Workflow             yes (deferred concept per ADR-ES-011 §27)
Conventional Workflow           yes
```

The mixed-mode model is architecturally valid. Agentic Enterprise does
NOT require all enterprise activity to be agentic (per AE-CON-013 +
AE-CON-014).

## Decision / Action independence

Per CR-ES-010 §16:

The schema distinguishes:

- decision_scope (decisions that may progress autonomously)
- action_scope (actions that may be executed autonomously)

This distinction is necessary because an enterprise may:

- Autonomously decide but require approval to execute.
- Execute predefined actions automatically but not autonomously decide.
- Autonomously decide and execute within a bounded domain.

Only the appropriate combination qualifies for the relevant autonomy /
agentic claim. The semantic distinction must be preserved in the
implementation.

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B.
- Vendor-specific embargo: zero references to material from embargoed
  sources.
