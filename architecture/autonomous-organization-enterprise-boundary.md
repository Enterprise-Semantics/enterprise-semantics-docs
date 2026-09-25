# Autonomous Organization / Autonomous Enterprise Boundary

Per ADR-ES-021 section 10 + CR-ES-021 section 12.

## Boundary Statement

Autonomous Enterprise may contain autonomous organizations, but Autonomous Organization is not Autonomous Enterprise. Enterprise-level autonomous value realization is a separate semantic concern.

## Conformance

Reject:
- Autonomous Organization is-a Autonomous Enterprise
- Autonomous Enterprise is-a Autonomous Organization

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
