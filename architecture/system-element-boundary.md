# System / Element Boundary

Per ADR-ES-027 section 6 + CR-ES-027 section 7 + Recon-ES-004.

## Boundary Statement

System contains Element. A System is an organized whole of interacting elements. Element is a constituent. System is NOT Element.

## Conformance

Reject:
- System is-a Element
- Element is-a System

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
