# Intent

## Definition

Per CR-ES-004 §7 + ADR-ES-004 §15:

> Intent is a communicated or established desired direction, purpose,
> or intended result that guides action.

## Distinctions

Per CR-ES-004 §7, Intent shall remain distinct from:

- **Goal**, Intent is broader, may include communicated direction without being a quantified target
- **Requirement**, Requirement is a necessary condition, Intent is a desired direction
- **Instruction**, Instruction is a prescribed action or procedure, Intent is a communicated desired direction
- **Policy**, Policy is a constraint or rule, Intent is a desired direction
- **Action**, Action is performed or initiated, Intent guides action

The exact semantic relationship among these concepts may be refined by subsequent governance.

## Relationships

- `Intent guides Action`, per CR-ES-004 §10, Action is directed toward the Intent's communicated desired direction or purpose

## Agent interpretation

Per ADR-ES-004 §7.1, an Agent interprets a delegated Intent. The interpretive obligation is established by the receipt of the Intent, per `Agent receives Intent` (CR-ES-004 §10).

## Governance

- **Source:** enterprise-semantics/concepts/intent.concept.yaml
- **Governing ADR:** ADR-ES-004 §15
- **Governing CR:** CR-ES-004 §7

## See also

- [Agent](./agent.md), Intent is received and interpreted by an Agent
- [Action](./action.md), Intent guides Action
- [Authority](./authority.md), Intent is interpreted within bounded authority

## Authored by

Emmanuel A. Otchere (cardinal author rule, 2026-09-23)