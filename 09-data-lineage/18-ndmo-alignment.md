# NDMO Alignment — Data Lineage

**Document ID:** RHC-DG-P9-018  
**Phase:** 9 — Data lineage  
**Status:** Implemented (alignment notes only)  
**Does not claim:** Implementation, evidence, scores, specification completion, or regulatory satisfaction

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

Phase 9 alignment is **limited**. This repository’s retrieved NDMO Standards v1.5 extract does **not** treat lineage as a named knowledge domain with copied control IDs.

**Do not invent NDMO control IDs.**  
**Do not claim NDMO compliance.**  
**Do not claim lineage satisfies any specific regulatory or NDMO requirement.**

---

## 2. Three-way distinction (mandatory)

| Bucket | What it includes in Phase 9 |
| --- | --- |
| **Verified NDMO-supported information** `[C]` | Data Catalog and Metadata is a knowledge-domain **name** (`MCM` as recorded in Phase 2); Data Quality, Data Classification, Data Sharing and Interoperability, and Reference and Master Data Management are knowledge-domain **names**; Trusted Data is a guiding principle **name**; DAMA DMBOK is a key reference **name**; NDMO describes an automated catalog as a national **concept** (not implemented here) |
| **Unverified NDMO information** `[NDMO verification required]` | **Specific lineage requirements**; whether lineage is mandated as a control/specification; official lineage artifacts; NPHIES or national claims-interchange lineage rules; whether technical lineage is required |
| **Rafid’s proposed design** `[A][B]` | Lifecycle; four types and Year-1 cut; Phase 8 hierarchy reuse; four granularity levels; two-step criticality; one E2E example; one business-lineage example; MVP |

**Do not mix the three buckets.**

---

## 3. General benefit vs confirmed requirement

Traceability for audit **as a governance practice** is `[B]`. Treating that as a **confirmed NDMO or sector specification** is `[NDMO verification required]` and is **not** claimed.

Specific lineage requirements remain:

**`[NDMO verification required]`**

---

## 4. What Phase 9 is not

- Not a completed NDMO domain implementation  
- Not automated catalog lineage  
- Not Phase 10 MDM  
- Not an annual assessment pack (Phase 14)

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5 — domain and principle **names** already used in this repo | Verified column |
| `[NDMO verification required]` | Specific lineage mandates; national interchange | Unverified column |
| `[A][B]` | Approved Phase 9 framework | Rafid column |
