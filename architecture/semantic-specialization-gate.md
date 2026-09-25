# Semantic Specialization Gate

Per ADR-ES-022 section 4 + CR-ES-022 section 6.

## Specialization Gate

A specialization SHALL be established only where the dimension materially changes the semantics of the base concept.

## Materiality Test

Does Agentic behavior materially alter how the concept operates, realizes its purpose, coordinates activity, makes decisions, adapts, or produces outcomes?

Does Autonomous behavior materially alter how the concept progresses independently through decisions, actions, coordination, or adaptation?

If the answer is no, a specialization SHALL NOT be created merely for symmetry.

## Required Metadata

Per CR-ES-022 section 6, every new Agentic or Autonomous specialization SHALL identify:

- Base Concept
- Semantic Delta
- Materiality
- Authority Boundary
- Policy Boundary
- Constraint Boundary
- Outcome
- Applicable Relationships
- Dependency
- ADR
- CR

A specialization without a documented semantic delta SHALL fail validation.

## Dependency Gate

Per CR-ES-022 section 7 + ADR-ES-022 section 9: a candidate specialization SHALL fail validation when its base concept is not canonical. The validator SHALL prevent implicit base-concept creation.

## Mechanical Symmetry Prohibition

Per ADR-ES-022 section 13: Enterprise-Semantics SHALL NOT create a corresponding Autonomous concept solely because an Agentic concept exists. Likewise, the existence of an Autonomous concept SHALL NOT require an Agentic counterpart.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
