# Value Stream Boundary

This document explains the semantic boundaries between Value Stream and
adjacent enterprise concepts.

Per CR-ES-003 §7 + ADR-ES-003 §7.

## Boundary Analysis

Value Stream is distinguished from the following adjacent concepts:

| Concept | Semantic meaning | Boundary |
|---|---|---|
| Capability | Enduring ability | Value Stream uses/enables capabilities, it is not itself an ability |
| Process | Organized execution/transformation | Processes realize activities within the Value Stream |
| Function | Area or purpose of activity | Functions may participate in multiple Value Streams |
| Service | Means of providing value or capability | Services may support one or more Value Stream stages |
| Product | Defined offering/proposition | Products may be the subject or output of Value Streams |
| Workflow | Coordinated execution flow | Workflow executes or coordinates work, Value Stream describes value progression |
| Activity | Unit of work | Activities contribute to stage realization |
| Outcome | Result achieved | Outcome represents a resulting state, Value Stream represents the journey toward it |
| Value | Worth/benefit realized | Value Stream provides the progression through which value is realized |
| Organization | Social/structural entity | Organizations participate in or enable Value Streams |
| System | Organized technical/socio-technical construct | Systems implement or support Value Stream execution |
| Agent | Entity capable of delegated action/decision | Agents may participate in execution without defining the Value Stream |

The central distinction is:

Value Stream describes the end-to-end progression of value, Process
describes execution within that progression.

## Architectural Invariants

Per ADR-ES-003 §32:

- VS-INV-001: Value Stream != Process
- VS-INV-002: Value Stream != Capability
- VS-INV-003: Value Stream != Workflow
- VS-INV-004: Value Stream != Service
- VS-INV-005: Value Stream != Organization
- VS-INV-006: Value Stream realizes Stakeholder Value
- VS-INV-007: Value Stream contains Value Stages
- VS-INV-008: Value Stage is not inherently a Process
- VS-INV-009: Value Stream identity is implementation-independent
- VS-INV-010: Agentic behavior is not required for Value Stream identity
- VS-INV-011: Autonomy is not required for Value Stream identity

## Rejected Alternatives

Per ADR-ES-003 §31:

- 31.1 Treat Value Stream as a Process, rejected because Process
  represents execution whereas Value Stream represents end-to-end value
  progression.
- 31.2 Treat Value Stream as a Process Group, rejected because
  Process Group is organizational/classification construct for processes.
- 31.3 Treat Value Stream as a Capability, rejected because
  Capability represents enduring ability rather than value progression.
- 31.4 Treat Value Stream as a Service, rejected because Service
  represents a means of providing value rather than the complete
  end-to-end journey.
- 31.5 Define Value Stream only through Value Stages, insufficient
  because Value Stream must also establish stakeholder, initiating
  condition, endpoint, value realization.
- 31.6 Make Agentic behavior foundational to Value Stream, rejected
  because traditional Value Streams must remain semantically valid
  independently of agentic or autonomous execution.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule (no en-dash, no em-dash)
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources (cardinal embargo
  2026-09-22)

## See also

- `value-stream-process-boundary.md`, the critical Value Stream vs
  Process boundary in detail
- `value-realization-boundary.md`, value realization architectural
  boundary
