# System / Service Boundary

Per ADR-ES-027 section 6 + CR-ES-027 section 7 + Recon-ES-004.

## Boundary Statement

System implements Service. Service is delivery-oriented. System is structural-behavioral. System is NOT Service.

## Conformance

Reject:
- System is-a Service
- Service is-a System

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
