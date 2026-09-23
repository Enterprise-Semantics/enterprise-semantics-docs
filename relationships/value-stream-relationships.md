# Value Stream Relationships

This document explains the canonical Value Stream and Value Stage
relationship vocabulary.

Per CR-ES-003 §9 + §10 + ADR-ES-003 §20.

## Relationship Table

The full 13-predicate relationship table per CR-ES-003 §9:

| Subject | Predicate | Object | Inverse | Provenance |
|---|---|---|---|---|
| Value Stream | realizes | Stakeholder Value | realized-by | CR-ES-003 §10.1 |
| Value Stream | contains | Value Stage | belongs-to | CR-ES-003 §10.2 |
| Value Stream | enabled-by | Capability | enables | CR-ES-003 §10.3 |
| Value Stream | realized-through | Process | realizes | CR-ES-003 §10.4 |
| Value Stream | produces | Outcome | produced-by | CR-ES-003 §10.5 |
| Value Stream | uses | Service | used-by | CR-ES-003 §10.6 |
| Value Stream | involves | Organization | involved-in | CR-ES-003 §10.7 |
| Value Stream | uses-resource | Resource | used-by-resource | CR-ES-003 §9 table |
| Value Stage | precedes | Value Stage | follows | CR-ES-003 §10.8 |
| Value Stage | stage-realized-through | Process | stage-realizes | CR-ES-003 §10.9 |
| Value Stage | requires | Capability | required-by | CR-ES-003 §10.10 |
| Value Stage | stage-produces | Outcome | stage-produced-by | CR-ES-003 §10.11 |
| Value Stage | contributes-to | Stakeholder Value | receives-contribution-from | CR-ES-003 §9 table |

## Per-Predicate Definitions

### Value Stream ;;; realizes ;;; Stakeholder Value (primary relationship)

A Value Stream realizes Stakeholder Value when progression through the
Value Stream results in the intended stakeholder value being achieved
or made available.

### Value Stream ;;; contains ;;; Value Stage

A Value Stream contains a Value Stage when that stage forms part of the
defined progression of value realization.

### Value Stream ;;; enabled-by ;;; Capability

A Value Stream is enabled by a Capability when that Capability provides
an ability required for one or more stages of the Value Stream to be
realized.

### Value Stream ;;; realized-through ;;; Process

A Value Stream is realized through a Process when Process execution
contributes to the realization of one or more stages of the Value
Stream. This relationship must NOT imply Value Stream = Process.

### Value Stream ;;; produces ;;; Outcome

A Value Stream produces an Outcome when progression through the Value
Stream results in the specified outcome.

### Value Stream ;;; uses ;;; Service

A Value Stream uses a Service when the Service provides functionality,
interaction, or value-enabling means required by the Value Stream.

### Value Stream ;;; involves ;;; Organization

A Value Stream involves an Organization when the Organization
participates in, enables, or contributes to one or more stages of the
Value Stream.

### Value Stream ;;; uses-resource ;;; Resource

A Value Stream uses a Resource when the Resource provides means
required by the Value Stream.

### Value Stage ;;; precedes ;;; Value Stage

A Value Stage precedes another Value Stage when it occurs earlier in
the defined progression of value realization.

### Value Stage ;;; stage-realized-through ;;; Process

A Value Stage is realized through a Process when execution of the
Process contributes to the transition represented by the Value Stage.

### Value Stage ;;; requires ;;; Capability

A Value Stage requires a Capability when the Capability provides an
ability necessary for the stage to be realized.

### Value Stage ;;; stage-produces ;;; Outcome

A Value Stage produces an Outcome when completion of the stage results
in the specified outcome.

### Value Stage ;;; contributes-to ;;; Stakeholder Value

A Value Stage contributes to Stakeholder Value when the stage outcome
contributes to the overall stakeholder value realized by the parent
Value Stream.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule (no en-dash, no em-dash)
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources (cardinal embargo
  2026-09-22)

## See also

- `concepts/value-stream.md` ;;; the Value Stream concept
- `concepts/value-stage.md` ;;; the Value Stage concept
