# Claim–Evidence Mapping — TrustGraph

**Domain:** trustgraph.de  
**Repository:** trustgraph-evidence  
**Reference model:** Claim → Evidence → Source (CES)  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Purpose

This document operationalizes the CES reference model by defining
which **types of claims** may be supported by which **types of evidence**.

It enforces consistency between:
- `SCOPE.md` (included / excluded boundaries)
- `MODEL.md` (CES structure)
- `index.html` (public reference description)

No evaluation or sufficiency judgement is expressed.

---

## Claim categories (in scope)

The following claim categories are explicitly **in scope**:

- **Stewardship claims**  
  Statements about maintenance, responsibility, or authorship.

- **Temporal claims**  
  Statements about creation, update, or publication time.

- **Alignment claims**  
  Statements about reference or alignment to standards or specifications.

- **Structural claims**  
  Statements about how information, artifacts, or models are organized.

Claims outside these categories are out of scope.

---

## Evidence categories (in scope)

The following evidence categories are explicitly **in scope**:

- Signed statements or attestations  
- Registry or directory entries  
- Changelog and version records  
- Published standards or specifications  
- Cryptographic artifacts (hashes, signatures, timestamps)  
- Logs or transparency records

---

## Claim–evidence mapping

| Claim category       | Permitted evidence types                                  | Notes |
|----------------------|-----------------------------------------------------------|-------|
| Stewardship claim    | Signed statement, registry entry, changelog               | Evidence must be attributable |
| Temporal claim       | Changelog record, timestamp, log entry                    | Time-bound evidence required |
| Alignment claim      | Standard reference, specification citation                | Reference only, not certification |
| Structural claim     | Model document, mapping table, repository structure       | Internal evidence permitted |

---

## Explicit constraints

- A **claim must not** reference a source anchor directly.  
- Evidence **must mediate** between claim and source anchor.  
- Evidence **does not imply** endorsement or correctness.  
- Source anchors **define legitimacy**, not claim validity.

These constraints are mandatory and non-negotiable.

---

## Out-of-scope mappings

The following mappings are explicitly **excluded**:

- Claims supported solely by reputation or popularity metrics  
- Claims supported by numerical trust or authority scores  
- Claims supported by legal or certification status  
- Claims inferred without inspectable evidence

---

## Consistency rule

Any introduction of a new:
- claim category, or
- evidence category

requires **simultaneous updates** to:
- this file,
- `SCOPE.md`, and
- `CHANGELOG.md`.

---

## Disclaimer

This document defines allowed mappings only.  
It does not provide judgement, validation, or assurance.
