# Agentic Value Stream Relationships

Per CR-ES-005 §7 + ADR-ES-005 §7 ;; the 3 governed Agentic Value Stream
predicates.

## Predicate table

| Subject | Predicate | Object | Provenance |
|---|---|---|---|
| agentic-value-stream | specializes | value-stream | CR-ES-005 §5 + §7 + ADR-ES-005 §2 + §7 |
| agentic-value-stream | engages | agent | CR-ES-005 §7 + ADR-ES-005 §7 + §14 |
| agentic-value-stream | agent-realizes | value-stage | ADR-ES-005 §6 + §7 + CR-ES-005 §6 |

## Predicate details

### ES:REL:specializes

**Subject:** ES:CONCEPT:agentic-value-stream
**Object:** ES:CONCEPT:value-stream
**Inverse:** generalised-by

An Agentic Value Stream specialises a Value Stream when the agentic
participation is a governed specialisation of the parent Value
Stream semantics. Per CR-ES-005 §5 + §7 + ADR-ES-005 §2 + §7. The
specialised construct retains the parent's mandatory properties (per
CR-ES-005 §8 inheritance requirements).

### ES:REL:engages

**Subject:** ES:CONCEPT:agentic-value-stream
**Object:** ES:CONCEPT:agent
**Inverse:** engaged-by

An Agentic Value Stream engages an Agent when agentic participation
materially contributes to value realization. Per CR-ES-005 §7 +
ADR-ES-005 §7 + §14. The engaged Agent inherits its semantic
properties from CR-ES-004 (interprets Intent ;; acts-within Authority ;;
selects Action ;; coordinates Action ;; produces Outcome ;; adapts-to
Context).

### ES:REL:agent-realizes

**Subject:** ES:CONCEPT:agentic-value-stream
**Object:** ES:CONCEPT:value-stage
**Inverse:** stage-agent-realised-by

A Value Stage within an Agentic Value Stream is realised agentically
when the stage's value transition involves agentic participation.
Per ADR-ES-005 §6 + §7. The namespaced predicate name
(agent-realizes ;; not realizes) disambiguates from the inherited
Value Stream realisation relationship (CR-ES-005 §7) and avoids
cross-CR subject-type collision.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23)
- D-004 dash rule
- SDO-neutral sourcing (ISO/IEC, ITU-T, ETSI, NIST)
- No vendor-specific material from embargoed sources