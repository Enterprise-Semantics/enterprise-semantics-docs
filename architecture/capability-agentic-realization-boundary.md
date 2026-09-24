# Capability / Agentic Capability Realization Boundary

## Architectural purpose

This document captures the architectural boundary between the universal
Capability concept (ADR-ES-002) and the Agentic Capability
specialization (ADR-ES-012). Per ADR-ES-012 §4 + §8.

## Primary distinction

Capability = enduring ability
Agentic Capability = enduring ability + material agentic realization

The distinction must remain explicit. Agentic Capability describes
how a Capability is materially realized, not what a Capability is.

## Boundary test

The primary question is:

Does the capability's realization materially incorporate agentic
behavior?

It is NOT:

- Does the enterprise possess an Agent?
- Does the capability use AI?
- Is the capability automated?
- Is the capability autonomous?

Per ADR-ES-012 §5, the answer to the primary question determines the
qualification ; the four negative questions are explicitly excluded
from the qualification test.

## Architectural diagram

```
CAPABILITY
"What enduring ability exists?"
        |
        v
AGENTIC CAPABILITY
"Is the ability materially realized agentically?"
        |
        v
REALIZATION
Agentic Workflow / Agentic Operations / Service / System / Human
        |
        v
OUTCOME
```

Per ADR-ES-012 §8.

## Materiality

Per ADR-ES-012 §7, Agentic behavior must be material to capability
realization. Examples of material agentic participation:

- contextual decision-making
- dynamic action selection
- adaptive coordination
- delegated execution
- contextual exception handling
- agentic interaction with stakeholders
- agentic resource coordination
- adaptive fulfillment of the capability's intended outcome

The mere use of an Agent as a tool does not automatically qualify.

## Conformance invariants

Per ADR-ES-012 §23:

- ACAP-CON-001: Agentic Capability specializes Capability
- ACAP-CON-002: Agentic Capability retains the Capability definition
- ACAP-CON-003: Agentic behavior must be material to realization
- ACAP-CON-009: Agentic Capability does not require AI
- ACAP-CON-010: Automation does not establish Agentic Capability
- ACAP-CON-011: Agentic Capability does not imply autonomy
