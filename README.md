# TrustGraph — Evidence Layer

**Domain:** trustgraph.de  
**Repository:** trustgraph-evidence  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Purpose

This repository provides the evidence layer for **TrustGraph**, an independent reference documenting how claims, evidence, and source anchors can be structured into traceable relationships for machine-consumable systems.

The repository exists to make terminology, scope boundaries, reference models, and source mappings **explicit, inspectable, and versioned**.

---

## What this repository is

- A **definitions and boundaries repository**, not an implementation  
- A **source-led reference**, grounded in primary standards  
- A **mapping layer** between conceptual claims and verifiable evidence  
- A **versioned artifact** suitable for audit, review, and machine consumption  

---

## What this repository is not

- Not a verification or certification service  
- Not a trust, authority, or reputation scoring system  
- Not legal, compliance, or policy advice  
- Not a product comparison or recommendation  

---

## Scope overview

The scope of TrustGraph is limited to **traceability of justification**, not evaluation of quality or intent.

Covered concepts include:

- Claims and assertions  
- Evidence artifacts  
- Provenance and attribution  
- Integrity primitives (timestamps, hashes, signatures)  
- Claim → evidence → source relationships  

Explicit exclusions are documented in `SCOPE.md`.

---

## Repository structure

- `README.md`  
  Purpose, scope overview, and repository discipline  

- `SCOPE.md`  
  Included and excluded boundaries, terminology notes  

- `SOURCES.md`  
  Primary source anchors and citation discipline  

- `MODEL.md`  
  The reference model used by TrustGraph (single model, max. three layers)  

- `MAPS/`  
  Mapping artifacts (e.g. term taxonomies, claim–evidence relationships)  

- `CHANGELOG.md`  
  Version history and documented changes  

---

## Editorial and source discipline

- Every definitional statement must be traceable to at least one primary source  
- Primary sources are stable standards or protocol documents  
- Contextual sources may be referenced but never replace anchor sources  
- No source text is reproduced if restricted by license  

---

## Versioning policy

- Semantic versioning is used (`v1.0`, `v1.1`, …)  
- Any change to scope, definitions, or the reference model requires:  
  - an update to the affected file(s)  
  - a corresponding entry in `CHANGELOG.md`  

Deprecated concepts are documented; they are not silently removed.

---

## Relationship to the website

The public site at **https://trustgraph.de/** provides a human-readable overview.

This repository is the **authoritative evidence layer**:

- definitions originate here  
- source lists are maintained here  
- models and mappings are versioned here  

---

## Contact

**Editorial inquiries:**  
research@rightsofrobots.com  

---

## Disclaimer

This repository documents terminology, scope boundaries, and evidence structures only.  
It does not provide legal advice, certification, compliance guarantees, or endorsements.
