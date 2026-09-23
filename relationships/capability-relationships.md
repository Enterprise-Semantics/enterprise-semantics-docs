# Capability Relationships

This document describes the eight canonical relationships that anchor
Capability within the enterprise semantic model.

## Core Relationships

Per CR-ES-002 §4 + §5 and ADR-ES-002 §1.4:

| Subject | Predicate | Object |
|---------|-----------|--------|
| Entity | possesses | Capability |
| Capability | enables | Outcome |
| Capability | realized-through | Process |
| Capability | exercised-by | Role |
| Capability | supported-by | Resource |
| Capability | delivered-through | Service |
| Capability | implemented-by | System |
| Capability | contributes-to | Value |
| Capability | supports | Goal |

Each predicate is registered in `relationships/vocabulary.yaml` with
identity, definition, subject type, object type, inverse, lifecycle status,
and provenance.

## Cardinal rules

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-22)
- D-004 dash rule
- SDO-neutral sourcing
- No vendor-specific material from embargoed sources
