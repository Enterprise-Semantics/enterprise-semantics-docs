# Autonomous Service Boundary

**Concept:** `ES:CONCEPT:autonomous-service`
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015
**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)

## Semantic Boundary

Autonomous Service operates at the **service boundary**. The service boundary answers the question:

> How is value or capability made available to a consumer or stakeholder through interaction or delivery, with bounded independent progression?

The service boundary is distinct from:

- the **capability boundary** (what an Entity is able to achieve)
- the **agent boundary** (who is acting)
- the **workflow boundary** (how work is coordinated/executed)
- the **operations boundary** (how ongoing operational activity progresses)
- the **value stream boundary** (end-to-end value realization)
- the **enterprise boundary** (enterprise-level autonomous progression)

A single Autonomous Service operates at the service boundary only. It does not, by itself, establish Autonomous Capability, Autonomous Operations, Autonomous Value Stream, or Autonomous Enterprise.

## Autonomy Materiality Boundary

Per ADR-ES-015 §4 + CR-ES-015 §8:

A Service shall NOT become Autonomous merely because it:

- uses AI
- uses automation
- uses an Agent
- uses an autonomous system
- runs without direct human supervision
- uses machine learning
- uses predefined decision rules

Autonomous progression must be material to service realization.

## Boundary With Agentic Service

The distinction is:

| Dimension | Agentic Service | Autonomous Service |
|---|---|---|
| Primary characteristic | Agentic behavior | Independent progression |
| Core question | Does service realization behave agentically? | Can service realization progress without human intervention for every decision/action? |
| Intent | May interpret delegated intent | Pursues defined service objective |
| Decision | May dynamically select actions | Decisions may execute independently |
| Authority | Required where applicable | Required |
| Policy | Applicable | Applicable |
| Adaptation | May be agentic | May occur independently |
| Human participation | Permitted | Permitted |
| AI | Not required | Not required |
| Automation | Not sufficient | Not sufficient |
| Agent | May be used | Not required |
| Agentic Workflow | May be used | May be used |
| Autonomous Operations | May support | May support |
| Agentic Value Stream | May participate | May participate |
| Autonomous Value Stream | May participate | May participate |

Therefore: Agentic Service != Autonomous Service per ASVC-AUTO-NEG-001.

## Boundary With Autonomous Capability

- Autonomous Capability = capability-level autonomy
- Autonomous Service = service-level autonomy

Neither concept subsumes the other. Autonomous Service may deliver or expose an Autonomous Capability.

Therefore: Autonomous Service != Autonomous Capability per ASVC-AUTO-NEG-003.

## Boundary With Autonomous Operations

- Autonomous Service = independent progression of service delivery or interaction
- Autonomous Operations = independent progression of ongoing operational activity

Autonomous Operations may support an Autonomous Service. Autonomous Operations do NOT automatically make every Service autonomous.

Therefore: Autonomous Service != Autonomous Operations per ASVC-AUTO-NEG-004.

## Boundary With Autonomous Value Stream

- Autonomous Service = service-level autonomous realization
- Autonomous Value Stream = end-to-end autonomous value realization

An Autonomous Value Stream may use multiple Autonomous Services. An Autonomous Service does NOT establish autonomy across the entire Value Stream.

Therefore: Autonomous Service != Autonomous Value Stream per ASVC-AUTO-NEG-005.

## Boundary With Autonomous Enterprise

- Autonomous Service = service-level autonomy
- Autonomous Enterprise = enterprise-level autonomy

A single Autonomous Service does NOT establish Autonomous Enterprise.

Therefore: Autonomous Service != Autonomous Enterprise per ASVC-AUTO-NEG-006.

## AI Boundary

Per ADR-ES-015 §9 + ASVC-AUTO-CON-015 + ASVC-AUTO-NEG-007 + ASVC-AUTO-NEG-008:

- AI may be used to implement an Autonomous Service.
- AI-enabled Service is NOT Autonomous Service.
- Autonomous Service does NOT require AI.

## Automation Boundary

Per ADR-ES-015 §10 + ASVC-AUTO-CON-016 + ASVC-AUTO-NEG-009:

- Automation may participate in an Autonomous Service.
- Automated Service is NOT Autonomous Service.
- Autonomous Service does NOT require Automation.

## Human Participation

Per ADR-ES-015 §11 + ASVC-AUTO-CON-014:

Human participation does NOT invalidate Autonomous Service. An Autonomous Service may use:

- human-in-the-loop
- human-on-the-loop
- human-over-the-loop
- exception-based intervention
- approval for high-impact decisions
- escalation beyond authority
- governance intervention

## See Also

- ADR-ES-015 §6-§14
- CR-ES-015 §8, §9, §11
- architecture/agentic-vs-autonomous-service.md
- architecture/service-autonomy-authority-boundary.md
- concepts/autonomous-service.md
