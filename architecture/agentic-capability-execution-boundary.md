# Agentic Capability / Agentic Workflow / Agent Boundary

## Architectural purpose

This document captures the boundary between Agentic Capability, Agentic
Workflow, and Agent. Per ADR-ES-012 §9-§11 + CR-ES-012 §10-§12.

## Core distinction

```
Agentic Capability = enduring ability (with material agentic realization)
Agentic Workflow = coordinated execution
Agent = acting Entity
```

These three are distinct semantic kinds, related via governed
predicates but not interchangeable.

## Boundary assertions

Per ADR-ES-012 §9-§11:

- Agent is NOT a subtype of Capability (ACAP-CON-013)
- Agentic Workflow is NOT a subtype of Capability (ACAP-CON-014)
- Agentic Operations is NOT a subtype of Capability (ACAP-CON-015)
- Agentic Value Stream is NOT a subtype of Capability (ACAP-CON-016)

The Agent is not the Capability. The Agent is an acting Entity ; the
Capability is an enduring ability.

## Relationships

Per ADR-ES-012 §6:

```
Agentic Capability
   |
   +-- engages -> Agent
   +-- realized-through -> Agentic Workflow
   +-- supported-by -> Agentic Operations
```

The Capability engages an Agent ; is realized through an Agentic
Workflow ; is supported by Agentic Operations. The relationships
inherit the Capability semantics established by ADR-ES-002 where
applicable. Agentic realization adds the behavioral dimension.

## Conformance invariants

Per ADR-ES-012 §23:

- ACAP-CON-005: Agentic Capability may engage an Agent
- ACAP-CON-006: Agentic Capability may be realized through Agentic Workflow
- ACAP-CON-007: Agentic Capability may be supported by Agentic Operations
- ACAP-CON-013: Agent is not a subtype of Capability
- ACAP-CON-014: Agentic Workflow is not a subtype of Capability
- ACAP-CON-015: Agentic Operations is not a subtype of Capability
