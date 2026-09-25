# Agentic Offering / Agentic Value Stream Boundary

Per ADR-ES-018 §12 and CR-ES-018 §10.

## Distinction

Agentic Value Stream describes agentic behavior at the end-to-end value-realization boundary. Agentic Offering describes agentic behavior at the offering boundary.

```
Agentic Value Stream
   |
   v
value realization journey
   |
   v
may involve
   |
   v
Agentic Offering
```

## Boundary Preservation

Per ADR-ES-018 §12 + AOFF-NEG-006:

- Agentic Offering is NOT Agentic Value Stream
- Agentic Value Stream is NOT Agentic Offering
- An Agentic Offering may participate in a conventional Value Stream, Agentic Value Stream, or Autonomous Value Stream

## Validator Constraint

The validator must prevent:
- Agentic Offering is-a Agentic Value Stream (AOFF-NEG-006)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
