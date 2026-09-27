# Agentic System / Agentic Service Boundary

Per ADR-ES-025 section 11 + CR-ES-025 section 9.

## Boundary Statement

Agentic System implements Agentic Service. Service is the delivery-oriented unit ; System is the structural-behavioral whole that may implement services. Agentic System is NOT Agentic Service.

## Conformance

Reject:
- Agentic System is-a Agentic Service
- Agentic Service is-a Agentic System

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
