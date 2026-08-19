# Search and Discovery

**Document ID:** RHC-DG-P8-010  
**Version:** 1.0  
**Status:** Implemented (conceptual only)  
**Owner:** DMO `[B]` (discovery method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Discovery dimensions; sensitive-asset metadata vs data split.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Search engine, index design, UI, or cybersecurity architecture

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **how people find assets using governed metadata** `[A][B]`.

It is not a technical search architecture. It is not an access-control product. Open by Default remains a national principle **name** `[C]`; it does not put Restricted clinical **data** into the catalog.

---

## 2. Discovery dimensions (locked)

Users may find assets by:

- Business term
- Domain
- Owner
- Classification
- Quality / Certification status
- Asset type
- System
- Tags / Keywords

No additional Year-1 discovery dimension is added (for example “data product” — deferred).

---

## 3. Sensitive assets — metadata vs data (locked)

The catalog **may** expose governed metadata needed for discovery, such as:

- Asset name
- Owner
- Classification
- Business definition

The catalog **must not** expose the underlying **Restricted** or **Confidential** data.

| Allowed in catalog `[B]` | Not allowed in catalog |
| --- | --- |
| “Patient demographic dataset” as a name | Rows of National IDs, names, diagnoses |
| Rafid tier **Restricted** `[A][B]` | The Restricted file contents |
| Owner title | A data extract “for convenience” |

Access to the **data** remains the approved Phase 4 / Phase 5 process (in-policy Owner **A**; exception **DMC A**; sharing privacy review **PDPO A**). This file does not create cybersecurity architecture or NCA controls.

Rafid tiers are not NDMO national tiers `[NDMO verification required]`.

---

## 4. What this file does not do

- No ranking algorithm
- No technical index
- No “analyst bypass” of classification
- No claim that NDMO requires these eight dimensions `[NDMO verification required]`

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Eight dimensions; metadata-vs-data split | Sections 2–3 |
| `[C]` | Open by Default principle **name**; Catalog domain **name** | Constraints |
| `[NDMO verification required]` | Official discovery/catalog UX mandates | Not claimed |
