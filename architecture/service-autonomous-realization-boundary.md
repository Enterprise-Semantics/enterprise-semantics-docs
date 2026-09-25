# Service vs Autonomous Service Realization Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Service (Universal)

The Service concept is the universal foundational type established by ADR-ES-002.

Service is:

- a means through which a capability or value is made available
- involves provider, consumer, service interaction, service delivery
- related to capability, outcome, value, service context

Service does not specify how the service is realized. A Service may be realized through conventional rules, AI, automation, agentic behavior, autonomous progression, or any other mechanism.

## Autonomous Service (Specialization)

Autonomous Service is a contextual specialization of Service established by ADR-ES-015:

> An Autonomous Service is a Service whose delivery or interaction is capable of progressing through decisions, actions, coordination, and adaptation within defined service objectives, authority, policies, constraints, and governance boundaries without requiring human intervention for every service decision or action.

Autonomous Service adds:

- defined service objectives
- defined decision and action scopes
- defined authority, policy, constraint, governance, service contract contexts
- adaptation within defined scope
- bounded independence

## Realization Boundary

The boundary is:

- **Service** describes what a service delivers (a means through which value is made available)
- **Autonomous Service** describes how that service is realized (bounded independence)

Autonomous Service does NOT change the meaning of Service. It qualifies the realization of the service.

## Invariants

- Service remains foundational ; Autonomous Service does NOT redefine Service
- Autonomy describes how the service can be realized, not what makes something a service
- Autonomous Service is a contextual specialization, not a replacement
- The Service -> Provider / Consumer / Service Interaction / Service Delivery / Capability / Outcome / Value / Service Context semantic anchors are preserved

## See Also

- ADR-ES-015 §3
- ADR-ES-002
- concepts/service.md (in the canonicalization pipeline)
- concepts/autonomous-service.md
- architecture/autonomous-service-boundary.md
