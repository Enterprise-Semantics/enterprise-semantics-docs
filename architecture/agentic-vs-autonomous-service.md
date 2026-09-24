# Agentic Service vs Autonomous Service

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-014
**Implemented by:** CR-ES-014

## Semantic Distinction

| Dimension | Agentic Service | Autonomous Service |
|---|---|---|
| Primary characteristic | Agentic service delivery | Independent service progression |
| Core question | Does realization materially incorporate agentic behavior? | Can realization progress without human intervention for every decision/action? |
| Intent | Delegated service intent may guide realization | Service objective guides independent progression |
| Decision | Contextual/action selection may be agentic | Service decisions can execute independently |
| Authority | Required | Required |
| Policy | Required where applicable | Required |
| Adaptation | May be agentic | May occur independently |
| Human participation | Permitted | Permitted |
| AI | Not required | Not required |
| Automation | Not sufficient | Not sufficient |
| Autonomy | Not implied | Defining characteristic |

## Orthogonality at Service Boundary

Per ADR-ES-014 §11:

| Agentic | Autonomous | Interpretation |
|---|---|---|
| No | No | Conventional Service |
| Yes | No | Agentic Service (ADR-ES-014, this) |
| No | Yes | Future Autonomous Service (ADR-ES-015, deferred) |
| Yes | Yes | Future combined characterization |

Autonomous Service requires a separate ADR per ADR-ES-014 §19.

## Compositional State

A Service exhibiting both Agentic and Autonomous characteristics is, semantically, a Service with two orthogonal properties applied. It is NOT a new foundational concept.

## See Also

- ADR-ES-014 §11
- CR-ES-014 §9
- architecture/agentic-service-boundary.md
- architecture/service-authority-escalation-boundary.md
- concepts/agentic-service.md
