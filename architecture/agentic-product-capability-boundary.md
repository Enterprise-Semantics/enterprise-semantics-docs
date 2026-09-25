# Agentic Product / Agentic Capability Boundary

Per ADR-ES-016 §10 and CR-ES-016 §14.

## Distinction

Capability represents an enduring ability. Product represents an offered realization of value.

```
Capability
   |
   v
may enable
   |
   v
Product
   |
   v
Agentic Product

Agentic Capability
   |
   v
may enable
   |
   v
Agentic Product
```

## Boundary Preservation

Per ADR-ES-016 §10 + APROD-CON-015 + APROD-NEG-002:

- An Agentic Capability does NOT automatically make every Product it enables agentic
- Agentic materiality must be demonstrated at the Product boundary
- Agentic Product is NOT Agentic Capability

## Validator Constraint

The validator must prevent:

- Agentic Capability is-a Agentic Product (APROD-NEG-002)
- Agentic Product is-a Agentic Capability (APROD-NEG-002)

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
