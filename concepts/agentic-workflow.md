# Agentic Workflow

Per CR-ES-006 §4 + §5 + ADR-ES-006 §2 + §3.

## Definition

> An Agentic Workflow is a Workflow in which one or more
> work-coordination or execution decisions are materially performed
> through agentic behavior, enabling contextual interpretation,
> dynamic action selection, coordination, adaptation, or escalation
> within defined authority.

## Semantic purpose

Per CR-ES-006 §4 + ADR-ES-006 §3 ;; Agentic Workflow fills the
**execution-level semantic gap** between Process and Activity/Task.
The semantic surface is:

```
Value Stream -> Value Stage -> Process -> Workflow -> Activity/Task
```

with Agentic Workflow as a specialisation at the Workflow layer.

## Workflow inheritance

Per CR-ES-006 §5 + ADR-ES-006 §5 ;; the canonical relationship is:

```
Agentic Workflow -|-> Workflow
```

Agentic Workflow inherits the Workflow semantics ;;; it does not
redefine Workflow.

## Process boundary

Per ADR-ES-006 §6 + CR-ES-006 §9 ;; Process and Workflow remain
distinct:

```
Process -> realized-through -> Workflow (or Agentic Workflow)
```

Agentic Workflow may realise or support a Process ;;; but Agentic
Workflow is NOT a Process.

## Activity boundary

Per ADR-ES-006 §7 + CR-ES-006 §10 ;; Agentic Workflow coordinates
Activities:

```
Agentic Workflow -> coordinates -> Activity
```

## Task boundary

Per ADR-ES-006 §7 + CR-ES-006 §10 ;; Agentic Workflow also
coordinates Tasks:

```
Agentic Workflow -> coordinates -> Task
```

## Agent participation

Per ADR-ES-006 §8 + CR-ES-006 §11 ;; Agentic Workflow engages one or
more Agents:

```
Agentic Workflow -> engages -> Agent
```

The material-participation criterion (per ADR-ES-006 §10) requires:

```
Agent interprets context
-> Agent selects permitted path
-> Workflow adapts
```

## Intent

Per ADR-ES-006 §4.1 + CR-ES-006 §12 ;; Agentic Workflow has an
associated workflow intent:

```
Agentic Workflow -> interprets -> Intent
```

## Authority

Per ADR-ES-006 §4.6 + §11 + CR-ES-006 §13 ;; Agentic Workflow
operates within defined Authority:

```
Agentic Workflow -> operates-within -> Authority
```

## Dynamic decision boundary

Per ADR-ES-006 §4.3 + §19 + CR-ES-006 §14 ;; Agentic Workflow has
identifiable decision boundaries where agentic behavior selects the
next task, activity, execution path, service, resource, escalation
route, or recovery strategy.

## Adaptation

Per ADR-ES-006 §4.5 + §12 + CR-ES-006 §15 ;; Agentic Workflow permits
runtime adaptation within bounded scope:

```
Context Change -> Interpretation -> Evaluate Authority/Constraints
  -> Select New Path -> Continue / Escalate
```

Runtime adaptation is distinct from permanent modification of the
canonical workflow definition.

## Human intervention

Per ADR-ES-006 §4.7 + §19 + CR-ES-006 §16 ;; Agentic Workflow
permits human intervention:

- `human-in-loop`
- `human-on-loop`
- `human-over-loop`
- `mixed`

## Automation distinction

Per ADR-ES-006 §13 + §24.2 ;; Automation is execution according to
predefined mechanisms. Agentic Workflow is workflow execution or
coordination materially influenced by agentic interpretation and
action/path selection.

An Agentic Workflow can contain automated steps. Automation is not
itself evidence of agency.

## AI distinction

Per ADR-ES-006 §14 + §24.1 ;; Agentic Workflow is technology-neutral:

- AI != Agentic Workflow
- AI-enabled Workflow != necessarily Agentic Workflow

AI may be used to implement agentic interpretation or action
selection, but it is not part of the definition.

## Autonomy distinction

Per ADR-ES-006 §17 + §24.3 + CR-ES-006 §10 ;; Agentic Workflow does
not imply Autonomous Workflow:

- Human approval
- Human escalation
- Constrained authority
- Predefined policies
- Supervised execution
- Externally established objectives

Autonomy requires separate semantic grounding (future ADR-ES-010).

## Agentic Value Stream relationship

Per ADR-ES-006 §15 + CR-ES-006 §21 ;; Agentic Value Stream and
Agentic Workflow operate at different architectural levels:

```
Agentic Value Stream
  -> Value Stage
    -> Process
      -> Agentic Workflow
```

Agentic Value Stream != Agentic Workflow. An Agentic Value Stream
may contain or use multiple Agentic Workflows. An Agentic Workflow
may also support a conventional Value Stream where appropriate.

## Examples

Per CR-ES-006 §27 + ADR-ES-006 §21 ;; the foundational OTCHERE Inc
Order Fulfillment example demonstrates the architectural distinction.

See `examples/foundational/workflows/order-fulfillment-workflow.yaml`
(Workflow-only) and
`examples/foundational/workflows/order-fulfillment-agentic-workflow.yaml`
(Agentic Workflow with 9-step flow).

## Conformance requirements

Per ADR-ES-006 §23 ;; 14 conformance rules (AWF-CON-001..014):

- AWF-CON-001 ;; Agentic Workflow specialises Workflow
- AWF-CON-002 ;; Agentic Workflow retains the semantics of Workflow
- AWF-CON-003 ;; Agentic Workflow materially incorporates agentic
  behavior into coordination or execution
- AWF-CON-004 ;; Agentic Workflow operates within defined authority
- AWF-CON-005 ;; Agentic Workflow has an identifiable intent or
  execution objective
- AWF-CON-006 ;; Agentic Workflow may coordinate Activities and Tasks
- AWF-CON-007 ;; Agentic Workflow may engage Agents
- AWF-CON-008 ;; Human intervention is permitted
- AWF-CON-009 ;; Agentic Workflow does not require AI
- AWF-CON-010 ;; Agentic Workflow does not imply autonomy
- AWF-CON-011 ;; Agentic Workflow is not a Process
- AWF-CON-012 ;; Agentic Workflow is not a Value Stream
- AWF-CON-013 ;; Agentic Workflow is not an Agent
- AWF-CON-014 ;; Agentic Workflow preserves grounding and provenance

## Provenance

Per CR-ES-006 + ADR-ES-006. Cardinal author Emmanuel A. Otchere.