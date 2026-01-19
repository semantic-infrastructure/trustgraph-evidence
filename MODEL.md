# Reference Model — TrustGraph

**Model name:** Claim → Evidence → Source (CES)  
**Domain:** trustgraph.de  
**Repository:** trustgraph-evidence  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Model intent

The CES model provides a **minimal, non-evaluative structure** for representing how claims are justified by evidence and anchored in authoritative sources.

The model is designed for:
- machine-consumable traceability,
- audit and review contexts,
- provenance-aware knowledge representations.

It does **not** assess truth, quality, or sufficiency.

---

## Model structure

### Layer 1 — Claim

A **claim** is a verifiable statement asserted about an entity, dataset, system, or publication.

Examples:
- “This dataset is maintained by Organization X.”
- “This specification aligns with Standard Y.”
- “This page was last updated on Date Z.”

Properties:
- Claims are declarative.
- Claims are not self-validating.
- Every claim requires supporting evidence.

---

### Layer 2 — Evidence

**Evidence** is an artifact that substantiates a claim.

Typical evidence types:
- Signed statements or attestations
- Registry or directory entries
- Changelog records and version histories
- Published standards or specifications
- Cryptographic artifacts (hashes, signatures)
- Logs or transparency records

Properties:
- Evidence must be inspectable.
- Evidence may support multiple claims.
- Evidence may be time-bound.

---

### Layer 3 — Source anchor

A **source anchor** is the canonical authority that establishes legitimacy or definition.

Examples:
- Standards bodies (e.g. W3C, IETF)
- Official registries
- Recognized institutions or publishers

Properties:
- Source anchors define legitimacy, not endorsement.
- Source anchors are referenced, not replicated.
- A source anchor may host or define multiple evidence artifacts.

---

## Relationships

The CES model enforces the following directional relationships:

- **Claim → Evidence**  
  A claim is supported by one or more evidence artifacts.

- **Evidence → Source anchor**  
  Evidence derives legitimacy from a canonical source.

There is **no reverse inference** from source anchor directly to claim.

---

## Constraints

- No authority, trust, or reputation scoring is defined.
- No automated sufficiency thresholds are implied.
- No endorsement or certification is expressed.
- Relationships must be explicit and inspectable.

---

## Alignment with sources

The CES model is conceptually grounded in:
- provenance models (e.g. W3C PROV),
- verifiable artifact patterns (e.g. verifiable credentials),
- integrity and timestamping protocols (e.g. RFC 3161).

Specific source anchors and citations are maintained in `SOURCES.md`.

---

## Change discipline

- Any modification to this model requires:
  - an explicit update to this file, and
  - a corresponding entry in `CHANGELOG.md`.
- Deprecated model elements are documented and not removed without record.

---

## Disclaimer

This model is a classification and traceability aid only.  
It provides no legal, compliance, certification, or assurance guarantees.
