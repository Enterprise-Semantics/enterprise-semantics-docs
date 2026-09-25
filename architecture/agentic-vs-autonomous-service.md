# Agentic Service vs Autonomous Service

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-015
**Implemented by:** CR-ES-015

## Semantic Distinction

| Dimension | Agentic Service | Autonomous Service |
|---|---|---|
| Primary characteristic | Agentic behavior | Independent progression |
| Core question | Does service realization behave agentically? | Can service realization progress without human intervention for every decision/action? |
| Intent | May interpret delegated intent | Pursues defined service objective |
| Decision | May dynamically select actions | Decisions may execute independently |
| Authority | Required where applicable | Required |
| Policy | Applicable | Applicable |
| Adaptation | May be agentic | May occur independently |
| Human participation | Permitted | Permitted |
| AI | Not required | Not required |
| Automation | Not sufficient | Not sufficient |
| Agent | May be used | Not required |
| Agentic Workflow | May be used | May be used |
| Autonomous Operations | May support | May support |
| Agentic Value Stream | May participate | May participate |
| Autonomous Value Stream | May participate | May participate |

## Service 2x2 Matrix (now structurally complete)

Per ADR-ES-015 §7 + ADR-ES-014 §11:

| Agentic | Autonomous | Interpretation |
|---|---|---|
| No | No | Conventional Service |
| Yes | No | Agentic Service (ADR-ES-014, v1.3.0) |
| No | Yes | Autonomous Service (ADR-ES-015, v1.4.0) |
| Yes | Yes | Combined characterization (NOT a new subtype) |

The fourth state is a combined characterization, NOT another foundational subtype.

## Orthogonality Rules

Per ADR-ES-015 §7:

- Autonomous Service does NOT imply Agentic Service
- Agentic Service does NOT imply Autonomous Service

The two dimensions are independent. A service may exhibit one, both, or neither characteristic without invalidating its identity as a Service.

## Compositional State

A Service exhibiting both Agentic and Autonomous characteristics is, semantically, a Service with two orthogonal properties applied. It is NOT a new foundational concept. This compositional state is the natural consequence of treating Agentic and Autonomous as orthogonal dimensions rather than as a single dimension.

## See Also

- ADR-ES-015 §7, §8
- ADR-ES-014 §11
- CR-ES-015 §9
- architecture/autonomous-service-boundary.md
- architecture/service-autonomous-realization-boundary.md
- concepts/agentic-service.md
- concepts/autonomous-service.md
