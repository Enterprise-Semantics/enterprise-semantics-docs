# Agentic vs Autonomous Culture Orthogonality

Per ADR-ES-024 section 5 + ADR-ES-022 section 5.

## Orthogonality Principle

Agentic and Autonomous are independent semantic dimensions at the Culture boundary.

```
  Culture
       |
  +----+----+
  |         |
Agentic   Autonomous
Culture    Culture
  |         |
  +----+----+
       |
  Agentic + Autonomous
  Culture
```

## Four-State Model

| Agentic | Autonomous | Characterization |
|---|---|---|
| No | No | Conventional Culture |
| Yes | No | Agentic Culture |
| No | Yes | Autonomous Culture |
| Yes | Yes | Agentic + Autonomous Culture |

This does NOT establish four separate inheritance branches.

## Conformance

Reject:
- Autonomous Culture requires Agentic Culture
- Agentic Culture requires Autonomous Culture

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
