# Agentic Enterprise

Per CR-ES-010 §2 + ADR-ES-010 §1 + §3.

## Definition

> An Agentic Enterprise is an Enterprise in which material aspects of
> enterprise value realisation, operational coordination, decision-making,
> or execution are performed through agentic behavior within defined
> intent, authority, policy, and governance boundaries.

## Semantic grounding

Per CR-ES-010 §2 + ADR-ES-010 §1 + §3: Agentic Enterprise specialises
**Enterprise** (not Agent, not Agentic Operations, not Agentic Value
Stream, not Agentic Workflow). The Agentic Enterprise describes an
enterprise-level operating condition in which agentic behavior is
materially embedded in enterprise value realisation and / or
operation.

The architectural position per ADR-ES-010 §4 + §17:

```
                          Enterprise
                              |
              +---------------+---------------+
              |                               |
       Agentic Enterprise          Autonomous Enterprise
              |                               |
              +---------------+---------------+
                              |
              enterprise-level orthogonal modes
```

## Specialization

Per ADR-ES-010 §1 + §3 + CR-ES-010 §2:

```yaml
specializes:
  - ES:CONCEPT:enterprise
```

## Characteristics

Per ADR-ES-010 §6:

- **Material agentic participation.** Agentic behavior materially
  influences enterprise value realisation, operational coordination,
  decision-making, execution, or adaptation (per AE-CON-002).
- **Enterprise-intent-anchored behavior.** Agentic enterprise behavior
  is anchored to defined enterprise intent, authority, policy, and
  governance boundaries (per AE-CON-004 through AE-CON-008).
- **Enterprise-outcome-oriented behavior.** Agentic Enterprise produces
  enterprise-level outcomes through defined value realisation,
  operational coordination, and execution mechanisms (per
  AE-CON-016).
- **Human governance compatible.** Human participation is permitted
  (human-in-the-loop, on-the-loop, over-the-loop). Governance bodies,
  policy owners, exception escalation, and intervention authority
  remain valid (per AE-CON-009).
- **Authority bound.** Agentic Enterprise operates within defined
  authority. Authority = unrestricted fails conformance (per
  AE-CON-018).

## Value Realisation Boundary

Per ADR-ES-010 §14 + CR-ES-010 §4 + AE-CON-004:

An Agentic Enterprise may realise value through Agentic Value Streams
(via the governed `enterprise-realizes-through` predicate). The
relationship does NOT imply:

- Agentic Enterprise = Enterprise containing Agentic Value Streams (per
  AE-NEG-015).
- Agentic Enterprise = Autonomous Enterprise (per ADR-ES-011 §11).

An enterprise may have value streams that are autonomous, agentic,
conventional, or any mixed combination, and still qualify as an Agentic
Enterprise if enterprise-level material agentic participation is
established (per AE-CON-013).

## Operational Boundary

Per ADR-ES-010 §15 + CR-ES-010 §4 + AE-CON-005:

An Agentic Enterprise may operate through Agentic Operations (via the
governed `enterprise-operates-through` predicate). The relationship
does NOT imply:

- Agentic Enterprise = Agentic Operations (per AE-NEG-011).
- Agentic Operations automatically establish Agentic Enterprise (per
  AE-NEG-014).

An enterprise may use Autonomous Operations, Agentic Operations,
conventional Operations, or human-led Operations, and still qualify as
an Agentic Enterprise if enterprise-level material agentic
participation is established (per AE-CON-014).

## Workflow Boundary

Per ADR-ES-010 §16 + CR-ES-010 §4:

An Agentic Enterprise may use Agentic Workflows as an execution
mechanism. The relationship does NOT imply:

- Agentic Enterprise = Enterprise containing Agentic Workflows (per
  AE-NEG-013).

## Governance Boundary

Per ADR-ES-010 §17 + AE-CON-007 + AE-CON-008:

An Agentic Enterprise operates within defined authority, governed by
policies, constraints, escalation, accountability, and oversight. The
governance boundary includes:

- Enterprise intent
- Enterprise objectives
- Authority scope
- Policy framework
- Constraint set
- Decision boundary
- Action boundary
- Escalation / intervention boundary

Unlimited authority is therefore explicitly incompatible with the
Agentic Enterprise semantic model (per AE-CON-018).

## Human Participation

Per ADR-ES-010 §10 + AE-CON-009:

An Agentic Enterprise may operate with:

- Human-in-the-loop
- Human-on-the-loop
- Human-over-the-loop
- Delegated decision authority
- Mandatory escalation
- Discretionary intervention
- Governance approval

Therefore:

```
Agentic Enterprise != Human-free Enterprise
```

Human governance is compatible with, and required by, agentic
operation.

## AI Boundary

Per ADR-ES-010 §11 + AE-CON-010 + AE-NEG-001 + AE-NEG-002:

AI is neither necessary nor sufficient for Agentic Enterprise:

- AI-enabled Enterprise != Agentic Enterprise (AE-NEG-001).
- Agentic Enterprise does not require AI (AE-CON-010).

AI may be an implementation mechanism for agentic behavior, but it is
not the semantic definition of agentic.

## Automation Boundary

Per ADR-ES-010 §12 + AE-CON-011 + AE-NEG-004 + AE-NEG-008:

Automation may support agentic enterprise behavior, but:

- Automation != Agentic behavior.
- Automation alone does not establish Agentic Enterprise (AE-NEG-008).
- Automation may coexist with Agentic Enterprise.

A fully automated enterprise mechanism may execute predefined behavior
without interpreting delegated intent or selecting actions
contextually. The presence of automation does not establish agentic
participation.

## Authority Boundary

Per ADR-ES-010 §1 + §17 + AE-CON-007 + AE-CON-018:

Agentic Enterprise operates within defined authority. Authority is
bounded. An Agentic Enterprise instance with:

```
authority = unrestricted
```

fails conformance. Unlimited authority is explicitly incompatible with
the Agentic Enterprise semantic model.

## Qualification

Per ADR-ES-010 §9 + ADR-ES-010 §8:

An enterprise instance qualifies as Agentic Enterprise only where there
is evidence of:

1. Enterprise-level intent or objectives.
2. Material agentic participation.
3. Defined authority boundaries.
4. Defined policy or governance boundaries.
5. Material impact on enterprise value realisation, operations,
   decisions, coordination, or execution.
6. Defined outcomes.
7. Adaptation or contextual response where claimed.
8. Human intervention / escalation boundaries where applicable.
9. Traceable realisation through enterprise architecture.

The model does NOT require every enterprise activity to be agentic
(per AE-CON-013 + AE-CON-014). Material agentic participation is the
qualification criterion.

## Conformance Invariants

Per ADR-ES-010 §19 + CR-ES-010 §15:

Positive invariants:

```
AE-CON-001  Agentic Enterprise specialises Enterprise
AE-CON-002  Agentic Enterprise requires material agentic participation
AE-CON-003  Agentic Enterprise is enterprise-boundary semantics
AE-CON-004  Agentic Enterprise may realise value through Agentic Value Streams
AE-CON-005  Agentic Enterprise may operate through Agentic Operations
AE-CON-006  Agentic Enterprise may use Agentic Workflows
AE-CON-007  Agentic Enterprise operates within defined authority
AE-CON-008  Agentic Enterprise operates within policy and governance boundaries
AE-CON-009  Human participation does not invalidate Agentic Enterprise
AE-CON-010  AI is not required
AE-CON-011  Automation is not sufficient
AE-CON-012  Agentic Enterprise does not imply Autonomous Enterprise
AE-CON-013  Agentic Enterprise does not require every Value Stream to be agentic
AE-CON-014  Agentic Enterprise does not require every operation to be agentic
AE-CON-015  Agentic Enterprise does not equal an enterprise containing Agents
AE-CON-016  Agentic Enterprise must remain outcome-oriented
AE-CON-017  Agentic Enterprise requires defined governance boundaries
AE-CON-018  Agentic Enterprise requires provenance and semantic grounding
```

Negative invariants (per CR-ES-010 §16):

```
AE-NEG-001  Agentic Enterprise is-a AI Enterprise
AE-NEG-002  Agentic Enterprise requires AI
AE-NEG-003  Agentic Enterprise is-a Autonomous Enterprise
AE-NEG-004  Agentic Enterprise requires Autonomous Operations
AE-NEG-005  Agentic Enterprise requires every Value Stream to be Agentic
AE-NEG-006  Agentic Enterprise requires every Process to be Agentic
AE-NEG-007  Agentic Enterprise is established merely by possessing an Agent
AE-NEG-008  Agentic Enterprise is established merely by using automation
AE-NEG-009  Agentic Enterprise requires elimination of humans
AE-NEG-010  Agentic Enterprise implies unlimited authority
AE-NEG-011  Agentic Enterprise is-a Agentic Operations
AE-NEG-012  Agentic Enterprise is-a Agentic Value Stream
AE-NEG-013  Agentic Enterprise is-a Agentic Workflow
AE-NEG-014  Agentic Operations automatically makes the Enterprise Agentic
AE-NEG-015  Agentic Value Stream automatically makes the Enterprise Agentic
AE-NEG-016  Agentic Enterprise implies Autonomous Enterprise
```

## Cardinal rules verified

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-24).
- D-004: zero en-dash, zero em-dash, zero U+2E3B. The file is authored
  with commas and colons per the project punctuation rule.
- Vendor-specific embargo: zero references to material from embargoed
  sources.
