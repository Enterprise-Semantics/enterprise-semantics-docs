# Process <> Workflow <> Agentic Workflow Boundary

Per CR-ES-006 §9 + §10 + ADR-ES-006 §6 + §7.

## Scope

The Process / Workflow / Agentic Workflow semantic boundary is
preserved as distinct layers.

## Process -|-> Workflow -|-> Agentic Workflow

```
Process
  -> realized-through
     -> Workflow
        -> specialized by
           -> Agentic Workflow
```

### Process layer

A Process represents the organised body of work through which a
Value Stage's outcome may be realised. Per CR-ES-003 ;; Process is
established as a distinct concept from Value Stage ;; Activity ;;;
Task ;; Workflow.

### Workflow layer

A Workflow is the coordination or execution mechanism through which a
Process is realised. Per ADR-ES-006 §5 + CR-ES-006 §5 ;; Workflow is
choreographic ;;; about how work executes ;; not what or why.

### Agentic Workflow layer

An Agentic Workflow is a Workflow that has agentic material
participation in coordination or execution. Per ADR-ES-006 §10 + §18.

## Boundary tests

### Test 1 ;; Process is NOT Agentic Workflow

```
Process -[is-a]-> Agentic Workflow ;;; INVALID
```

The Process remains the organised work. The Agentic Workflow is the
execution mechanism. They are different layers.

### Test 2 ;; Workflow is NOT Agentic Workflow

```
Workflow -[is-a]-> Agentic Workflow ;;; INVALID
```

Workflow is the general coordination mechanism. Agentic Workflow is
the agentic specialisation. A Workflow that contains an Agent without
material participation is NOT an Agentic Workflow.

### Test 3 ;; Agentic Workflow realises Process

```
Process -[realized-through]-> Agentic Workflow ;;; VALID
```

Agentic Workflow may realise or support a Process. This is permitted
because Agentic Workflow specialises Workflow.

### Test 4 ;; Agentic Workflow coordinates Activity

```
Agentic Workflow -[coordinates]-> Activity ;;; VALID
```

Per ADR-ES-006 §18 + CR-ES-006 §10 ;; Agentic Workflow coordinates
Activities. Activity coordination does not make Activity agentic
merely because an Agentic Workflow coordinates it.

### Test 5 ;; Agentic Workflow coordinates Task

```
Agentic Workflow -[coordinates]-> Task ;;; VALID
```

Per ADR-ES-006 §18 + CR-ES-006 §10 ;; Agentic Workflow also
coordinates Tasks.

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean
- No embargo refs