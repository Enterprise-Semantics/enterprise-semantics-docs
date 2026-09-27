# Autonomous System ; Concept

> **Status:** Established in ES-028. 9-of-9 boundary dimension matrix complete.
> **Semantic Version:** 2.4.0
> **Authority:** Enterprise-Semantics
> **Depends on:** WSF-ADR-SYSTEM-001 (provisional, per LOCKED-PICKS v9), ES-ADR-027, ES-022

## Definition

An Autonomous System is a System capable of independently progressing through decisions, actions, coordination, and adaptation toward defined objectives within specified authority, policies, constraints, and governance boundaries, without requiring human intervention for every system decision or action.

Per ES-ADR-028 section 2.

## Semantic Rationale

A conventional System establishes elements, relationships, behavior, purpose, boundary, and context. An Autonomous System additionally establishes objective, decision independence, action independence, coordination independence, adaptation, bounded authority, policy, constraint, governance, and intervention boundary.

## Specialization Chain

WSF System
    |
    +-- Agentic System (ES-025)
    |
    +-- Autonomous System (ES-028)

## Agentic/Autonomous Independence

Autonomous System and Agentic System remain independent semantic dimensions:

```
                  Autonomous
                No          Yes
              +- ----------+----------+
Agentic  No   | System    | Autonomous|
              |           | System    |
              +-----------+----------+
        Yes   | Agentic   | Agentic + |
              | System    | Autonomous|
              +-----------+----------+
```

No state may be inferred from the presence of another.

## AI/Automation Boundary

- Autonomous System does NOT require AI.
- Automation != Autonomy.
- AI != Autonomy.
- AI + Automation != necessarily Autonomous System.

## Materiality Test

A System is NOT classified as Autonomous merely because it executes automatically, contains an AI model, contains an Agent, performs scheduled actions, exposes APIs, uses machine learning, follows predefined rules, or performs unattended execution. Autonomy requires material evidence of independent progression through decisions, actions, coordination, or adaptation.

## Boundary With Related Concepts

- Autonomous System != Autonomous Operations
- Autonomous System != Agent
- Autonomous System != Agentic System
- Autonomous System can coexist with Agentic System

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
