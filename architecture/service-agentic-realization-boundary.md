# Service vs Agentic Service Realization Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Service (Universal)

The Service concept is the universal foundational type established by ADR-ES-002.

Service is:

- a means through which a capability or value is made available
- involves provider, consumer, service interaction, service outcome
- related to capability realization

Service does not specify how the service is realized. A Service may be realized through conventional rules, AI, automation, agentic behavior, autonomous progression, or any other mechanism.

## Agentic Service (Specialization)

Agentic Service is a contextual specialization of Service established by ADR-ES-014:

> An Agentic Service is a Service whose delivery or interaction materially incorporates agentic behavior in interpreting intent, selecting or coordinating actions, adapting service behavior, or executing service responses toward an intended outcome within defined authority, policy, and contextual boundaries.

Agentic Service adds:

- material agentic behavior in service realization
- defined intent, context, authority, decision, action scopes
- adaptation within defined scope
- bounded independence within authority

## Realization Boundary

The boundary is:

- **Service** describes what a service delivers (a means through which value is made available)
- **Agentic Service** describes how that service is delivered (with material agentic behavior)

Agentic Service does NOT change the meaning of Service. It qualifies the realization of the service.

## Invariants

- Service remains foundational ; Agentic Service does NOT redefine Service
- Agentic behavior qualifies service realization, not service identity
- Agentic Service is a contextual specialization, not a replacement
- The Service -> Provider / Consumer / Service Interaction / Service Outcome semantic anchors are preserved

## See Also

- ADR-ES-014 §3
- ADR-ES-002
- concepts/service.md
- concepts/agentic-service.md
- architecture/agentic-service-boundary.md
