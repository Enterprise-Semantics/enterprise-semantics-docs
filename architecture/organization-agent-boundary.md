# Organization / Agent Boundary

Per ADR-ES-022 section 6 + CR-ES-022 section 11.

## Boundary Statement

Organization coordinates Actors, which may include Agents. An Organization may contain Agents, but an Organization is not an Agent.

## Conformance

Reject:
- Organization is-a Agent
- Agent is-a Organization

unless separately authorized by a governed relationship.

## Author

Emmanuel A. Otchere (cardinal author rule, 2026-09-24)
