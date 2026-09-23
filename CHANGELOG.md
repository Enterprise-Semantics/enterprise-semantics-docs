## [0.3.0] ; 2026-09-23 ; CR-ES-004 VS-D1a Agentic documentation

### Added (5 concept docs + 3 architecture docs + 1 relationships doc)

- concepts/agent.md ;;; Agent entity per CR-ES-004 §5
- concepts/agentic.md ;;; Agentic semantic property per CR-ES-004 §6
- concepts/intent.md ;;; Intent concept per CR-ES-004 §7
- concepts/authority.md ;;; Authority concept per CR-ES-004 §8
- concepts/action.md ;;; Action concept per CR-ES-004 §9
- architecture/agentic-boundary.md ;;; Agentic vs Automation boundary per CR-ES-004 §12 + ADR-ES-004 §8
- architecture/agentic-autonomous-boundary.md ;;; Agentic vs Autonomous boundary per CR-ES-004 §14 + ADR-ES-004 §9
- architecture/agentic-execution-boundary.md ;;; Agentic Workflow + Operations + Value Stream boundaries per CR-ES-004 §15-§17
- relationships/agentic-relationships.md ;;; 11 Agentic predicates table per CR-ES-004 §10

### Cardinal rules

- Author: Emmanuel A. Otchere on all 9 files
- D-004 clean ;;; 0 forbidden glyphs on all 9 files
- No vendor-specific material from embargoed sources

# Changelog

All notable changes to this repository are documented in this file. Dates use
the committer's local time.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) semantics.
This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned

- VS-D2 ;;; tests + visuals across enterprise-semantics-test-probe + enterprise-semantics-visuals (CR-ES-003 §29-§31, §28).
- Generated Markdown views for additional concepts (Capability was a Phase 4.8 deliverable ;;; Value Stream is the next).
- Foundational principles documents (12 total per README).

## [0.1.0] ; 2026-09-23 ; VS-D1a Value Stream documentation

### Added

- `concepts/value-stream.md` ;;; Value Stream concept documentation per CR-ES-003 §27. Canonical definition, 8 semantic characteristics, identity rules, 8 relationships, cardinal rules.
- `concepts/value-stage.md` ;;; Value Stage concept documentation per CR-ES-003 §27. Canonical definition, 8 semantic characteristics, identity rules, 6 relationships, cardinal rules.
- `architecture/value-stream-boundary.md` ;;; semantic boundary analysis per CR-ES-003 §27 + ADR-ES-003 §7. 12-row boundary table + 11 architectural invariants + 6 rejected alternatives.
- `architecture/value-stream-process-boundary.md` ;;; critical Value Stream vs Process boundary per CR-ES-003 §27 + §8 + §16 + §17. Conceptual hierarchy, Workflow boundary, central distinction.
- `architecture/value-realization-boundary.md` ;;; Value Realization vs Execution layering per CR-ES-003 §27 + §14 + ADR-ES-003 §12 + §20. Three-layer architecture (Value Realization / Execution / Implementation) + schema implications + architectural result diagram.
- `relationships/value-stream-relationships.md` ;;; full 13-predicate vocabulary per CR-ES-003 §27 + §9 + §10. Subject/predicate/object/inverse/provenance table + per-predicate definitions.

### Scope

This release implements VS-D1a of CR-ES-003 ;;; the human-readable documentation for Value Stream + Value Stage across concepts + architecture + relationships. No concept YAML mutation, no schema mutation, no validation rule addition. The 6 documentation files are companion views of the canonical concept records (already on enterprise-semantics main after VS-A PR #2) and the 13 governed predicates (already on enterprise-semantics main after VS-B PR #5).

### Governance

- ADR-ES-003 (Proposed, governance slot 0005) ;;; ratifies the foundational Value Stream decision ;;; §7, §12, §20 are the documentation anchors.
- CR-ES-003 (Proposed, governance slot 0011) ;;; carries §27 documentation requirements + §7-§20 source material.
- FND-ES-AG-008 (Established 2026-09-22) ;;; establishes the WSF grounding classification referenced throughout.

### Cardinal rules applied

- Author: Emmanuel A. Otchere (cardinal author rule, 2026-09-23) ;;; present in all 6 new files.
- No en-dash (U+2013) or em-dash (U+2014) in any new file (D-004 dash rule). Section dividers use `;;;` boundary lines per existing convention.
- No vendor-specific material from embargoed sources in any new file (cardinal embargo, 2026-09-22).
- ES is sourced from SDO-neutral standardisation only (ISO/IEC, ITU-T, ETSI, NIST).

### Held non-actions

- No tests or PlantUML visuals (held for VS-D2).
- No examples (held for VS-D1b).
- No ADR-ES-003 promotion to Accepted (gated on CR-ES-003 implementation completion).
- No release tag (per v3.1.4 user directive).

## [0.0.1] ; 2026-09-02 ; Skeleton

### Added

- README.md (purpose, ownership, status, relationship to other repos).
- CODEOWNERS (sole owner: @emmanuel-a-otchere).
- CHANGELOG.md (this file).
- .gitignore (credential, AI-model, and workspace-noise patterns).
- LICENSE (Apache-2.0).