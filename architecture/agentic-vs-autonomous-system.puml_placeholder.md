# Agentic vs Autonomous System ; Orthogonality Status

Per ADR-ES-025 section 8 + section 13 + ADR-ES-022 section 13.

## Orthogonality Principle

Agentic and Autonomous are independent semantic dimensions at the System boundary. Per ADR-ES-022 section 13 (mechanical symmetry prohibition), Autonomous System is intentionally NOT established alongside Agentic System. A separate semantic decision is required.

## Current State

| Agentic | Autonomous | System characterization |
|---|---|---|
| No | No | Conventional System |
| Yes | No | Agentic System (v2.3.0, Established) |
| No | Yes | Autonomous System candidate (DEFERRED) |
| Yes | Yes | Agentic + Autonomous System candidate (DEFERRED) |

The final two states remain characterization states only until Autonomous System is separately canonicalized.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
