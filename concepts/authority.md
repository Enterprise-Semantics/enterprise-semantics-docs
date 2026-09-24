# Authority

## Definition

Per CR-ES-004 §8 + ADR-ES-004 §15:

> Authority is a defined scope of permitted action or decision
> assigned to an Entity within a specified context.

## 5 Boundary dimensions

Per CR-ES-004 §8, Authority may include:

- **action permissions**, what actions are permitted
- **decision boundaries**, what decisions are within scope
- **resource boundaries**, what resources may be used
- **escalation conditions**, when human approval or higher authority is required
- **constraints**, policies, regulations, or operational limits

## Required for agentic operation

Per ADR-ES-004 §7.4 + §15 + AG-INV-006, Agentic semantics without authority boundaries would be insufficiently defined for enterprise use.

## Relationships

- `Authority constrains Action`, per CR-ES-004 §10, Action is limited by the defined scope
- `Agent acts-within Authority`, per CR-ES-004 §10, Agent's actions are constrained by the Authority scope

## Distinctions

- **Authority != Permission**, per ADR-ES-004 §8, Authority is broader than Permission (includes decision boundaries, resource limits, escalation)
- **Authority != Role**, per ADR-ES-004 §5, Role identifies responsibility, Authority identifies scope of action
- **Authority != Capability**, per CR-ES-002, Capability is an enduring ability, Authority is a bounded scope

## Governance

- **Source:** enterprise-semantics/concepts/authority.concept.yaml
- **Governing ADR:** ADR-ES-004 §15
- **Governing CR:** CR-ES-004 §8

## See also

- [Agent](./agent.md), Agent acts-within Authority
- [Action](./action.md), Authority constrains Action

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)