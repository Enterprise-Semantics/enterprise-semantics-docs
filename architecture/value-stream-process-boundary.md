# Value Stream vs Process Boundary

This document expands the critical architectural boundary between Value
Stream and Process.

Per CR-ES-003 §8 + §16 + §17 + ADR-ES-003 §8.

## The Critical Boundary

A Value Stream is NOT a Process hierarchy.

A Value Stream may contain or be realized through multiple Processes,
and a single Process may contribute to multiple Value Streams.

## Conceptual Model

The hierarchy is:

    Value Stream
        ;;
        v
    Value Stage
        ;;
        v
    (realized through)
        ;;
        v
    Process
        ;;
        v
    Activity
        ;;
        v
    Task
        ;;
        v
    Workflow / Task Flow

NOT:

    Value Stream = Process Group

NOT:

    Value Stream = Process

## Workflow Boundary

Per CR-ES-003 §17, Workflow shall remain an execution concept.

A Workflow may coordinate:

- processes
- activities
- tasks
- decisions
- system interactions
- human actions
- automated actions

A Value Stream represents the larger value progression within which such
execution occurs.

Therefore:

    Value Stream
        ;;
        +-- realized through --> Process
                                     ;;
                                     +-- coordinated by --> Workflow

Workflow shall not be treated as the semantic representation of a Value
Stream.

## What Value Stream Is Not

Per CR-ES-003 §8:

- A Value Stream does NOT reduce to a single Process
- A Value Stream does NOT decompose structurally into Process Stages
- A Value Stream does NOT require linear execution ;;; branching,
  convergence, optional and repeated stages are permitted
- A Value Stream does NOT define its own Workflow

## What Process Is Not

- A Process does NOT define stakeholder value
- A Process does NOT determine the stakeholder
- A Process does NOT prescribe the value realization boundary
- A Process does NOT constitute an end-to-end value journey

## The Central Distinction

Value Stream answers "what value is realized and through what progression?"
while Process answers "how is work organized and executed?"

These are distinct questions ;;; conflating them collapses value
progression into execution detail and breaks the architectural
separation of concerns that makes Value Stream a stable semantic lens.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule (no en-dash, no em-dash)
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources (cardinal embargo
  2026-09-22)

## See also

- `value-stream-boundary.md` ;;; broader boundary analysis
- `value-realization-boundary.md` ;;; value realization vs execution
