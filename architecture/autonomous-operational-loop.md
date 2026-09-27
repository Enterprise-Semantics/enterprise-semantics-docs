# Autonomous Operational Loop

Per CR-ES-008 §15 + ADR-ES-008 §5 + §15.

## Scope

The autonomous operational control loop is the canonical semantic loop
that governs how Autonomous Operations independently senses, 
interprets, decides, coordinates, executes, observes, 
and adapts within explicit objectives, authority, and policy
boundaries.

## The 11-step loop with boundary

Per ADR-ES-008 §5:

```
Objective / Intent
        |
        v
Authority
        |
        v
Policies / Constraints
        |
        v
Operational Context
        |
        v
Sense
        |
        v
Interpret
        |
        v
Decide
        |
        v
Coordinate
        |
        v
Execute
        |
        v
Observe Outcome
        |
        v
Adapt
        |
        +-----------------> Operational Context
```

The loop iterates continuously ;; bounded by intent, authority, 
and policy boundaries.

## Bounded autonomous operating mode

Per ADR-ES-008 §14 + §26 ;; autonomy remains bounded:

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
Constraint
   |
   v
Autonomous Decision
   |
   v
Authorized Action
   |
   v
Outcome
```

## Material participation criterion

Per ADR-ES-008 §7 + §23 ;; autonomous behaviour must materially
participate in operational decision and action. Mere presence of an
Agent ;; an AI system, or an Automation does not satisfy the
autonomy criterion (per AOP-AUTO-CON-002 + AOP-AUTO-CON-003).

## Cardinal rules

- Author: Emmanuel A. Otchere
- D-004 clean ;; 0 forbidden glyphs
- No vendor-specific material from embargoed sources