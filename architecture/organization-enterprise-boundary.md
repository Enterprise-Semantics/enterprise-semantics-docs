# Organization / Enterprise Boundary

Per ADR-ES-022 section 5 + CR-ES-022 section 11.

## Boundary Statement

Enterprise comprises Organizations. An Organization is part of an Enterprise, but an Organization is not an Enterprise.

## Conformance

Reject:
- Organization is-a Enterprise
- Enterprise is-a Organization

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
