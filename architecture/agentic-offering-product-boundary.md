# Agentic Offering / Agentic Product Boundary

Per ADR-ES-018 §3 and CR-ES-018 §8.

## Distinction

An Offering may comprise or include multiple Products. An Agentic Offering may contain Agentic Products without itself being an Agentic Product.

```
Offering
   |
   v
may comprise / include
   |
   v
Product
   |
   v
Agentic Product

Offering
   |
   v
Agentic Offering
```

## Boundary Preservation

Per ADR-ES-018 §3 + AOFF-NEG-002 + AOFF-NEG-014:

- Agentic Offering is NOT Agentic Product
- Agentic Product does NOT automatically make the whole Offering agentic
- An Offering can be agentic because of how the overall proposition is configured, composed, interacted with, fulfilled, or adapted, even where its constituent Products are not individually agentic

## Validator Constraint

The validator must prevent:
- Agentic Offering is-a Agentic Product (AOFF-NEG-002)
- Agentic Product is-a Agentic Offering (unless an explicitly modeled separate specialization establishes this)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
