# enterprise-semantics-docs

> Enterprise-Semantics human-readable documentation: conceptual guides, implementation guides, tutorials, glossary, lifecycle.

Documentation in this repository is generated where possible from the structured semantic source in [`enterprise-semantics`](https://github.com/Enterprise-Semantics/enterprise-semantics). Hand-authored content covers explanations, walk-throughs, and conceptual framing that cannot be generated.

## Status

**First + second + third + fourth + fifth content tranches (v0.1.0 Value Stream + v0.2.0 Agentic + v0.3.0 Agentic Value Stream + v0.5.0 Agentic Workflow + v0.6.0 Agentic Operations).** Value Stream documentation landed via VS-D1a on 2026-09-23 (6 files: concepts/value-stream.md, concepts/value-stage.md, architecture/value-stream-boundary.md, architecture/value-stream-process-boundary.md, architecture/value-realization-boundary.md, relationships/value-stream-relationships.md). Agentic documentation landed via VS-D1a (9 files: concepts/agent.md, concepts/agentic.md, concepts/intent.md, concepts/authority.md, concepts/action.md, architecture/agentic-boundary.md, architecture/agentic-autonomous-boundary.md, architecture/agentic-execution-boundary.md, relationships/agentic-relationships.md). Agentic Value Stream documentation landed via VS-D1a (5 files: concepts/agentic-value-stream.md, architecture/agentic-value-stream-boundary.md, architecture/value-stream-agentic-boundary.md, architecture/agentic-value-realization.md, relationships/agentic-value-stream-relationships.md).

## What lives here

- `docs/foundational/`, 12 Foundational Principles (style guide: spec tone, no narration).
- `docs/conceptual/`, conceptual guides (Capability, Value Stream, Agentic, Autonomous, Operations, Closed Loop, ...).
- `docs/implementation/`, how to consume enterprise-semantics from WSF, OpenDEA, custom systems.
- `docs/tutorials/`, step-by-step examples.
- `docs/glossary/`, generated from the semantic source; reviewed manually.
- `docs/lifecycle/`, lifecycle model documentation.

## Relationship to other repositories

| Repository | Relationship |
|------------|--------------|
| [`enterprise-semantics`](https://github.com/Enterprise-Semantics/enterprise-semantics) | Source of truth (this repository derives from it). |
| [`enterprise-semantics-examples`](https://github.com/Enterprise-Semantics/enterprise-semantics-examples) | Parallel: examples illustrate what documents describe. |

## License

Apache License 2.0. See [LICENSE](https://github.com/Enterprise-Semantics/enterprise-semantics-docs/blob/main/LICENSE).