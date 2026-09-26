# System / Process Boundary

Per ADR-ES-027 section 6 + CR-ES-027 section 7 + Recon-ES-004.

## Boundary Statement

System contains Process as an activity sequence inside the System. Process is what happens. System is what contains it. System is NOT Process.

## Conformance

Reject:
- System is-a Process
- Process is-a System

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
