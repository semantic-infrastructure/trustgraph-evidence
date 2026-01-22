# Changelog — TrustGraph Evidence Layer

**Domain:** trustgraph.de  
**Repository:** trustgraph-evidence  
**Versioning scheme:** semantic (vX.Y)  

---

## v1.0 — 2026-01-19

### Added
- Initial public reference page (`index.html`) with structured JSON-LD markup  
- Evidence repository baseline:
  - `README.md` (purpose, scope overview, discipline)
  - `SCOPE.md` (included/excluded boundaries)
  - `SOURCES.md` (primary and context sources)
  - `MODEL.md` (Claim → Evidence → Source reference model)
  - `MAPS/claim-evidence-mapping.md` (operational mapping rules)

### Scope
- Defined TrustGraph as a non-evaluative, source-led reference
- Explicit exclusion of scoring, certification, and endorsement logic

### Sources
- Anchored terminology and model concepts to stable W3C, IETF, NIST, and C2PA references

### Constraints
- Enforced claim → evidence → source mediation
- Prohibited direct claim-to-source inference

---

## Versioning policy

- Minor versions (`v1.1`, `v1.2`, …) document:
  - scope clarifications,
  - additional source anchors,
  - refined mappings.
- Major versions (`v2.0`, …) indicate:
  - structural model changes,
  - scope redefinition.

All changes are additive or explicitly deprecated; no silent removals.

---

2026-01-22 — Metadata
- Added explicit `license` field to JSON-LD Dataset object to satisfy schema validation requirements (non-functional change).

---

## Disclaimer

This changelog documents structural and editorial changes only.  
It does not express validation, endorsement, or compliance guarantees.
