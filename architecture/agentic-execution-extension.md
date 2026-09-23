# Agentic Execution (Extended Profile)

Per CR-ES-006 §21 ;; the Agentic Execution Profile (ES:PROFILE:agentic-execution)
is extended to include Workflow + Agentic Workflow in its scope.

## Scope (post-CR-ES-006)

The Agentic Execution Profile now covers:

- Agent
- Agentic
- Intent
- Authority
- Action
- **Workflow** (added per CR-ES-006 §21)
- **Agentic Workflow** (added per CR-ES-006 §21)

## Profile characteristics

The Profile applies four governed characteristics to base concepts:

1. Goal-directed execution under bounded autonomy
2. AI-augmented decision-making (or its non-AI equivalent ;;; per
   technology neutrality)
3. Adaptive behavior
4. Human governance, not human execution

## Cardinal rules

- Profile is organisational only ;;; does not imply inheritance between
  members
- Author: Emmanuel A. Otchere
- D-004 clean
- No vendor-specific material from embargoed sources

## Architectural position

Per ADR-ES-006 §14 ;;; the Profile provides discoverability and
grouping for the agentic execution semantic surface. Workflow and
Agentic Workflow are added because they participate in agentic
execution ;;; per the architectural boundary:

```
Value Stream -> Value Stage -> Process -> Workflow -> Activity/Task
```

The Profile was originally Established by FND-ES-AG-003 + ADR-ES-AG-001
§3.3. The CR-ES-006 extension is additive ;;; the Profile retains its
Established status.