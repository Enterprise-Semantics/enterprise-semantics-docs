# System

Per ADR-ES-027 section 1 + CR-ES-027 section 2.

## Canonical Definition

A System is an organized whole of interacting elements whose relationships and behavior enable the realization of one or more intended functions, purposes, or outcomes within a defined context and boundary.

## Foundational Status

System is a foundational concept within Enterprise-Semantics. It specializes Entity (not any existing concept).

## Canonical Relationships (per ADR-ES-027 section 5)

System specializes Entity. System contains Element. System has Boundary. System operates-within Context. System realizes Function, Purpose. System produces Outcome. System exhibits Behavior. System supports Capability. System implements Service. System participates-in Workflow. System engages Agent.

## Boundary Discipline (per ADR-ES-027 section 6 + Recon-ES-004)

System is NOT Entity, Organization, Enterprise, Service, Resource, Process, Workflow, Capability, IT system specifically.

## Properties (per ADR-ES-027 section 3 + CR-ES-027 section 3)

element_organization, behavioral_coherence, system_boundary, intended_functions, intended_purposes, intended_outcomes, contextual_operation, realization_mode.

## Architectural Significance

Per Recon-ES-004, System performs distinctive semantic work:
- Element organization
- Behavioral coherence
- Boundary
- Purpose orientation
- Contextual operation

System accommodates business, information, technical, socio-technical, operational, and distributed systems. System does NOT collapse into IT system.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
