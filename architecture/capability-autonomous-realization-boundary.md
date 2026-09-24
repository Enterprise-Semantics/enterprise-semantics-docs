# Capability vs Autonomous Capability Realization Boundary

**Authored by:** Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
**Ratified by:** ADR-ES-013
**Implemented by:** CR-ES-013

## Capability (Universal)

The Capability concept is the universal foundational type established by ADR-ES-002:

> An enduring ability of an Entity to achieve or enable an Outcome.

Capability is:

- enduring (persistent across realizations)
- an ability (not an action)
- of an Entity (the bearer)
- to achieve or enable an Outcome (the semantic anchor)

Capability does not specify how the ability is realized. A Capability may be realized through human action, automation, agentic behavior, autonomous progression, or any other mechanism.

## Autonomous Capability (Specialization)

Autonomous Capability is a contextual specialization of Capability established by ADR-ES-013:

> An Autonomous Capability is a Capability whose realization is capable of progressing through decisions, actions, coordination, and adaptation within defined objectives, authority, policies, constraints, and governance boundaries without requiring human intervention for every capability decision or action.

Autonomous Capability adds:

- defined objectives
- defined decision and action scopes
- defined authority, policy, constraint, governance contexts
- adaptation within defined scope
- bounded independence

## Realization Boundary

The boundary is:

- **Capability** describes what an Entity can achieve (the ability itself)
- **Autonomous Capability** describes how that ability can be realized (bounded independence)

Autonomous Capability does NOT change the meaning of Capability. It qualifies the realization of the ability.

```
        Capability (universal)
              |
              | contextual specialization
              v
        Autonomous Capability
              |
              | bounded realization mode
              v
     autonomous-realization-mode
     (decision/action progression
      within authority/policy/
      constraints/governance)
```

## Invariants

- Capability remains foundational ; Autonomous Capability does NOT redefine Capability
- Autonomy describes how the capability can be realized, not what makes something a capability
- Autonomous Capability is a contextual specialization, not a replacement
- The Capability -> Outcome semantic anchor is preserved at both the universal and specialized levels

## See Also

- ADR-ES-013 §3.1
- ADR-ES-002 §4
- concepts/capability.md
- concepts/autonomous-capability.md
- architecture/autonomous-capability-boundary.md
