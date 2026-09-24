# Autonomous Capability Boundary

**Concept:** `ES:CONCEPT:autonomous-capability`
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013
**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)

## Semantic Boundary

Autonomous Capability operates at the **capability boundary**. The capability boundary answers the question:

> What is an Entity able to achieve or enable?

The capability boundary is distinct from:

- the **agent boundary** (who is acting)
- the **operations boundary** (how ongoing operational activity progresses)
- the **value stream boundary** (end-to-end value realization)
- the **enterprise boundary** (enterprise-level autonomous progression)

A single Autonomous Capability operates at the capability boundary only. It does not, by itself, establish Autonomous Operations, Autonomous Value Stream, or Autonomous Enterprise.

## Boundary With Agentic Capability

The semantic distinction is:

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

The two dimensions remain orthogonal. The four-state matrix at the capability boundary:

| Agentic | Autonomous | Interpretation |
|---|---|---|
| No | No | Conventional capability realization |
| Yes | No | Agentic Capability |
| No | Yes | Autonomous Capability |
| Yes | Yes | Capability exhibiting both characteristics |

The fourth state is a compositional semantic characterization, not a new concept.

## Boundary With Automation

Automation is an execution mechanism. Autonomous Capability is a semantic characteristic of capability realization.

Therefore:

- Automation may enable autonomy
- Automation is NOT autonomy
- A fully automated capability with no independent decision scope remains automated rather than autonomous

## Boundary With AI

AI is a technological mechanism or capability.

Therefore:

- AI may enable autonomous realization
- AI is NOT Autonomous Capability
- An AI-enabled capability is NOT automatically an Autonomous Capability
- Conversely, Autonomous Capability does NOT require AI

## Boundary With Autonomous Operations

Autonomous Capability and Autonomous Operations operate at different semantic levels.

- Autonomous Capability = what an Entity is able to achieve or enable
- Autonomous Operations = how ongoing operational activity can progress independently

Autonomous Operations may support realization of an Autonomous Capability. Autonomous Operations do NOT automatically make every supported Capability autonomous.

## Boundary With Autonomous Value Stream

- Autonomous Capability = enduring ability
- Autonomous Value Stream = autonomous end-to-end value realization

An Autonomous Capability may enable an Autonomous Value Stream, but the existence of an Autonomous Capability does NOT establish autonomy across the entire Value Stream.

## Boundary With Autonomous Enterprise

- Autonomous Capability = capability-level autonomy
- Autonomous Enterprise = enterprise-level autonomous progression

A single Autonomous Capability does NOT establish an Autonomous Enterprise. An Autonomous Enterprise may contain capabilities whose realization remains human-dependent.

## Bounded Autonomy

Autonomous Capability does NOT mean unrestricted independence. Autonomous realization operates within:

```
Objective
   |
   v
Authority
   |
   v
Policy
   |
   v
Constraints
   |
   v
Governance
   |
   v
Decision / Action
   |
   v
Outcome
   ^
   |
Adaptation (loop)
```

Authority = unrestricted must fail conformance per CR-ES-013 §17.

## Human Participation

A capability may be autonomous while retaining:

- human oversight
- escalation
- intervention
- approval for defined classes of decisions
- governance controls
- exception handling

Autonomy means that human intervention is not required for every capability decision or action.

## See Also

- ADR-ES-013 §3.1 to §3.5
- CR-ES-013 §8, §11, §17
- architecture/agentic-vs-autonomous-capability.md
- architecture/capability-autonomy-authority-boundary.md
- concepts/autonomous-capability.md
