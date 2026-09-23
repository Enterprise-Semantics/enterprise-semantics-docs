# Value Realization Boundary

This document explains the architectural boundary between value
realization (Value Stream) and execution (Process, Activity, Task,
Workflow, Service, System, Resource, Technology).

Per CR-ES-003 §14 + ADR-ES-003 §12 + §20.

## The Layered Architecture

The semantic source supports a strict layering:

    VALUE REALIZATION
    ==========================================
    Value Stream
         ;;
         v
    Value Stage
    ==========================================
    EXECUTION
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
    ==========================================
    IMPLEMENTATION
         ;;
         +-- Service
         +-- System
         +-- Resource
         +-- Technology

The Value Stream layer describes value progression. The Execution layer
describes how work is performed. The Implementation layer describes the
means by which execution is realized.

## Boundary Principles

1. **Value progression precedes execution.** A Value Stream is defined
   before its realizing Processes are identified.
2. **Stages are value-relevant, not execution units.** A Value Stage
   represents a meaningful value transition, not an Activity or Task.
3. **Execution belongs in the Process semantic.** Process input/output
   belongs to Process, not to Value Stage input_state/resulting_state.
4. **Implementation is downstream of execution.** Service, System,
   Resource, Technology are implementation concerns that realize the
   execution layer.

## Schema Implications

The implementation ensures that schemas do not accidentally collapse
these layers. Concretely:

- Value Stage input_state / resulting_state describe the value
  progression, NOT Process input / output.
- Value Stage does NOT contain Tasks as a direct semantic decomposition.
- Value Stream does NOT have a structural Task or Activity relationship.
- Value Stream does NOT have Workflow as a composition.

## Architectural Result

The resulting semantic architecture:

                    ENTERPRISE VALUE REALIZATION
                              ;;
                              v
                       +--------------+
                       | Value Stream |
                       +------+--------+
                              ;;
                    contains  ;;
                              v
                       +--------------+
                       | Value Stage  |
                       +------+--------+
                              ;;
              +---------------+--+--------------+
              |||              ||
              v v v            v v
         Capability     Process         Service
              |||              ||
              |||              v
              |||           Activity
              |||              ||
              |||              v
              |||            Task
              |||              ||
              |||              v
              |||          Workflow
              |||
              ++++--------------+
                              v
                          Outcome
                              ;;
                              v
                    Stakeholder Value

The model establishes value progression above execution. That
distinction is the principal architectural purpose of the Value
Realization Boundary.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule (no en-dash, no em-dash)
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources (cardinal embargo
  2026-09-22)

## See also

- `value-stream-boundary.md` ;;; semantic boundaries
- `value-stream-process-boundary.md` ;;; Value Stream vs Process
