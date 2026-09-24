# Agentic Capability / Agentic Enterprise Boundary

## Architectural purpose

This document captures the boundary between Agentic Capability and
Agentic Enterprise. Per ADR-ES-012 §17 + CR-ES-012 §14.

## Core distinction

```
Agentic Capability = enduring ability with material agentic realization
Agentic Enterprise = Enterprise with material agentic value realization, operational coordination, decision-making, or execution
```

These two are distinct semantic kinds operating at different
boundaries (capability boundary vs enterprise boundary).

## Boundary assertions

Per ADR-ES-012 §17:

```
Agentic Enterprise
        |
        v
possesses
        |
        v
Agentic Capability
```

However:

Agentic Capability != Agentic Enterprise

A single Agentic Capability does not establish Agentic Enterprise.
Enterprise-level materiality remains a separate qualification
boundary.

## Architectural diagram

Per CR-ES-012 §32:

```
                     ENTERPRISE
                         |
                  Agentic Enterprise
                         |
                         v
                  Agentic Capability
                         |
        +----------------+----------------+
        |                |                |
        v                v                v
Agentic Value      Agentic Ops      Agentic Workflow
   Stream              |                |
        |              +-------+--------+
        |                      |
        +----------------------+
                               v
                            Agent
                               |
                               v
                            Outcome
```

## Conformance invariants

Per ADR-ES-012 §23:

- ACAP-CON-012: Agentic Capability does not imply Agentic Enterprise
