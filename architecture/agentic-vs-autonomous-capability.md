# Agentic Capability vs Autonomous Capability

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013

## Semantic Distinction

| Dimension | Agentic Capability | Autonomous Capability |
|---|---|---|
| Primary characteristic | Agentic behavior | Independent progression |
| Core question | Does realization interpret/select/coordinate actions agentically? | Can realization progress without human intervention for every decision/action? |
| Intent | Delegated intent may guide realization | Objective guides independent progression |
| Decision | Contextual/action selection may be agentic | Decisions can execute independently |
| Authority | Required | Required |
| Policy | Required where applicable | Required |
| Adaptation | May be agentic | May occur independently |
| Human participation | Permitted | Permitted |
| AI | Not required | Not required |
| Automation | Not sufficient | Not sufficient |
| Autonomy | Not implied | Defining characteristic |
| Agent | May be engaged | Not required |
| Agentic Workflow | May be used | May be used |
| Agentic Operations | May support | May support |
| Autonomous Operations | May support | May support |
| Autonomous Value Stream | May enable | May enable |

## The 2x2 Matrix

At the capability boundary, the four-state matrix is:

| Agentic | Autonomous | Interpretation |
|---|---|---|
| No | No | Conventional capability realization |
| Yes | No | Agentic Capability |
| No | Yes | Autonomous Capability |
| Yes | Yes | Capability exhibiting both characteristics |

The fourth state (Agentic + Autonomous) is a compositional semantic characterization, not a new concept type.

## Orthogonality Rules

Per ADR-ES-013 §3.2 and ADR-ES-013 §7:

- Autonomous Capability does NOT imply Agentic Capability
- Agentic Capability does NOT imply Autonomous Capability

The two dimensions are independent. A capability may exhibit one, both, or neither characteristic without invalidating its identity as a Capability.

## Compositional State

A Capability exhibiting both Agentic and Autonomous characteristics is, semantically, a Capability with two orthogonal properties applied. It is NOT a new foundational concept. This compositional state is the natural consequence of treating Agentic and Autonomous as orthogonal dimensions rather than as a single dimension.

## See Also

- ADR-ES-013 §7
- ADR-ES-012 §14
- CR-ES-013 §8
- architecture/autonomous-capability-boundary.md
- architecture/capability-autonomous-realization-boundary.md
- concepts/agentic-capability.md
- concepts/autonomous-capability.md
