# Scope Matrix — TrustGraph

**Domain:** trustgraph.de  
**Repository:** trustgraph-evidence  
**Model:** Claim → Evidence → Source (CES)  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Purpose of this matrix

This scope matrix maps **conceptual elements** of TrustGraph to their
allowed roles within the CES model.

It serves as:
- a consistency check across files,
- a machine- and audit-readable scope reference,
- a guardrail against scope drift.

This matrix is classificatory only.

---

## Core concepts mapping

| Concept        | CES Layer        | Description                                                   | In scope |
|----------------|------------------|---------------------------------------------------------------|----------|
| Claim          | Claim            | Verifiable statement asserted about an entity or artifact     | Yes      |
| Evidence       | Evidence         | Artifact substantiating a claim                               | Yes      |
| Source anchor  | Source           | Canonical authority defining legitimacy                       | Yes      |
| Provenance     | Evidence         | Origin and custody information for artifacts                  | Yes      |
| Attribution    | Evidence         | Authorship or responsibility metadata                         | Yes      |
| Citation       | Evidence         | Reference linking to source material                          | Yes      |
| Integrity data | Evidence         | Hashes, timestamps, signatures                                | Yes      |

---

## Evidence category mapping

| Evidence category      | CES Layer | Examples                                                   | Notes |
|------------------------|-----------|------------------------------------------------------------|-------|
| Signed statement       | Evidence  | Signed declaration, attestation                             | Time-bound |
| Registry entry         | Evidence  | Official registry record                                    | External |
| Changelog              | Evidence  | Version history, update log                                 | Internal |
| Standard reference     | Evidence  | W3C, IETF, ISO specification                                | Cited, not copied |
| Cryptographic artifact | Evidence  | Hash, signature, timestamp                                  | Integrity only |
| Log / transparency log | Evidence  | Append-only log                                             | Optional |

---

## Explicit exclusions matrix

| Concept                     | Reason for exclusion                                   |
|-----------------------------|--------------------------------------------------------|
| Trust score                 | Introduces subjective evaluation                       |
| Authority ranking           | Conflicts with non-evaluative scope                    |
| Reputation metrics          | Sentiment-based, non-verifiable                        |
| Certification status        | Jurisdiction-specific, out of scope                    |
| Compliance judgement        | Legal interpretation not provided                      |

---

## Relationship constraints

- Claims **must not** directly reference source anchors.  
- Evidence **must** mediate between claim and source.  
- Source anchors **do not validate** claims; they provide legitimacy context only.

---

## Consistency rules

- Every concept listed here must appear consistently across:
  - `index.html`
  - `SCOPE.md`
  - `MODEL.md`
- Any new concept requires:
  - an update to this matrix, and
  - an entry in `CHANGELOG.md`.

---

## Disclaimer

This matrix documents internal scope discipline only.  
It does not express endorsement, validation, or sufficiency.
