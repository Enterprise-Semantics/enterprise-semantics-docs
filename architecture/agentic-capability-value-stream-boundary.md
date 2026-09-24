# Agentic Capability / Agentic Value Stream Boundary

## Architectural purpose

This document captures the boundary between Agentic Capability and
Agentic Value Stream. Per ADR-ES-012 §12 + CR-ES-012 §13.

## Core distinction

```
Capability = ability
Value Stream = value realization
```

These two are distinct semantic kinds. The boundary test is:

An Agentic Capability may enable an Agentic Value Stream.

This does NOT imply:

Agentic Capability = Agentic Value Stream

## Relationship

Per ADR-ES-012 §12:

```
Agentic Capability
        |
        v
enables
        |
        v
Agentic Value Stream
```

The relationship is governed, not coincidental. The Capability enables
the Value Stream ; the Value Stream realises the value. The semantic
distinction remains:

- Capability -> ability
- Value Stream -> value realization

## Boundary assertions

Per ADR-ES-012 §12 + ACAP-CON-008 + ACAP-CON-016:

- Agentic Value Stream is NOT a subtype of Agentic Capability
- An Agentic Capability does not require an Agentic Value Stream
- An Agentic Value Stream may be supported by one or more Agentic
  Capabilities

## Conformance invariants

- ACAP-CON-008: Agentic Capability may enable Agentic Value Stream realization
- ACAP-CON-016: Agentic Value Stream is not a subtype of Capability
