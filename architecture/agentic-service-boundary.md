# Agentic Service Boundary

**Concept:** `ES:CONCEPT:agentic-service`
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014
**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)

## Semantic Boundary

Agentic Service operates at the **service boundary**. The service boundary answers the question:

> How is value or capability made available to a consumer or stakeholder through interaction or delivery?

The service boundary is distinct from:

- the **capability boundary** (what an Entity is able to achieve)
- the **agent boundary** (who is acting)
- the **workflow boundary** (how work is coordinated/executed)
- the **operations boundary** (how ongoing operational activity progresses)
- the **value stream boundary** (end-to-end value realization)

A single Agentic Service operates at the service boundary only. It does not, by itself, establish Agentic Capability, Agentic Workflow, Agentic Operations, Agentic Value Stream, or Autonomous Service.

## Agentic Materiality Boundary

Per ADR-ES-014 §4 + CR-ES-014 §8:

A Service shall NOT become Agentic merely because it:

- invokes an Agent
- uses AI
- uses automation
- exposes an API
- contains an AI model
- supports conversational interaction
- is implemented by an autonomous system

Agentic behavior must be material to service realization.

## Boundary With Agent

The distinction is:

- **Agent** = Entity capable of interpreting delegated intent, selecting/coordinating actions, and acting within authority.
- **Agentic Service** = Service whose realization materially incorporates agentic behavior.

An Agent may participate in an Agentic Service without being the Service itself.

Therefore: Agent != Agentic Service per ASVC-NEG-001.

## Boundary With Agentic Capability

The distinction is:

- **Agentic Capability** = enduring ability to achieve or enable an Outcome through material agentic realization.
- **Agentic Service** = means through which a capability or service outcome is made available through material agentic realization.

A capability may be delivered through an Agentic Service. An Agentic Service may expose or enable capabilities that are not themselves Agentic Capabilities.

Therefore: Agentic Capability != Agentic Service per ASVC-NEG-002.

## Boundary With Agentic Workflow

The distinction is:

- **Agentic Workflow** = agentic coordination/execution of work.
- **Agentic Service** = agentic realization of a service interaction or delivery.

An Agentic Service may use one or more Agentic Workflows. The workflow is an execution mechanism ; the service is the service-level offering/delivery construct.

Therefore: Agentic Service != Agentic Workflow per ASVC-NEG-003.

## Boundary With Agentic Operations

The distinction is:

- **Agentic Operations** = agentic operating mode for ongoing operational activity.
- **Agentic Service** = service realization through agentic behavior.

An Agentic Service may operate within Agentic Operations. Agentic Operations do NOT make every Service Agentic.

Therefore: Agentic Service != Agentic Operations per ASVC-NEG-004.

## Boundary With Agentic Value Stream

The distinction is:

- **Agentic Value Stream** = end-to-end stakeholder value realization materially involving agentic behavior.
- **Agentic Service** = service-level delivery or interaction materially involving agentic behavior.

An Agentic Value Stream may use multiple Agentic Services. An Agentic Service does NOT imply an Agentic Value Stream.

Therefore: Agentic Service != Agentic Value Stream per ASVC-NEG-005.

## Boundary With Autonomous Service

Per ADR-ES-014 §11 + ASVC-NEG-006:

- Agentic Service does NOT imply Autonomous Service.
- Autonomous Service is orthogonal at the service boundary.

The two dimensions remain independent. Autonomous Service requires a separate ADR per ADR-ES-014 §19.

## AI Boundary

Per ADR-ES-014 §12 + ASVC-CON-014 + ASVC-NEG-007 + ASVC-NEG-008:

- AI may be used to implement an Agentic Service.
- AI-enabled Service is NOT Agentic Service.
- Agentic Service does NOT require AI.

## Automation Boundary

Per ADR-ES-014 §13 + ASVC-CON-015 + ASVC-NEG-009:

- Automation may participate in an Agentic Service.
- Automated Service is NOT Agentic Service.
- Agentic Service does NOT require Automation.

## Human Participation

Per ADR-ES-014 §14:

Human participation does NOT invalidate Agentic Service. An Agentic Service may use:

- human-in-the-loop
- human-on-the-loop
- human-over-the-loop
- human escalation
- approval gates
- exception handling

## See Also

- ADR-ES-014 §6-§14
- CR-ES-014 §8, §9, §11
- architecture/agentic-vs-autonomous-service.md
- architecture/service-authority-escalation-boundary.md
- concepts/agentic-service.md
