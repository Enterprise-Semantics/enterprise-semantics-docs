# Agentic vs Autonomous Organization Orthogonality

Per ADR-ES-021 section 3 + section 8 + CR-ES-021 section 7.

## Orthogonality Principle

Agentic and Autonomous are independent semantic dimensions. Neither subsumes the other.

```
  Organization
       |
  +----+----+
  |         |
Agentic   Autonomous
Organization   Organization
  |         |
  +----+----+
       |
  Agentic + Autonomous
  Organization
```

## Four-State Model

| Agentic | Autonomous | Characterization |
|---|---|---|
| No | No | Conventional Organization |
| Yes | No | Agentic Organization |
| No | Yes | Autonomous Organization |
| Yes | Yes | Agentic + Autonomous Organization |

This does not establish four separate inheritance branches. It represents two independent semantic dimensions.

## Conformance

Reject:
- Autonomous Organization requires Agentic Organization
- Agentic Organization requires Autonomous Organization

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
