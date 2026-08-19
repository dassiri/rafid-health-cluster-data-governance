# Metadata Management Framework Overview

**Document ID:** RHC-DG-P8-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer / DMO `[B]` (methodology); domain **Data Owner** remains **A** for business meaning  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 8 conceptual metadata/catalog framework.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Tool, UI, automated lineage, or live register population

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved **metadata management lifecycle** for the fictional Rafid Health Cluster `[A]`.

It is governance operating design `[B]`. It is not a catalog product, not a search engine, and not an NDMO compliance pack.

Data Catalog and Metadata is an NDMO knowledge-domain **name** (`MCM` as recorded in Phase 2) `[C]`. Control-level catalog requirements remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Locked lifecycle

```text
Identify data asset
→ Register
→ Describe
→ Classify
→ Assign ownership
→ Validate
→ Publish
→ Maintain
→ Review
→ Retire
```

| Stage | Intent | Who (Phase 4 pattern — not redesigned) |
| --- | --- | --- |
| **Identify** | Recognize a data asset in operational use | Business Data Steward **R**; Custodian **C** |
| **Register** | Create the governed record | Steward **R**; DMO completeness check |
| **Describe** | Business definition and mandatory metadata | Steward **R**; Data Owner **A** for meaning |
| **Classify** | Link Rafid tier (Phase 5) | Owner **A**; Steward **R**; follows Classification Procedure — unlabeled is not Public |
| **Assign ownership** | Domain Owner and Steward on the record | Already assigned at domain level (Phase 4); recorded on the asset |
| **Validate** | Steward validation; Owner approval where required; DMO governance check | See [`07-asset-registration-workflow.md`](07-asset-registration-workflow.md) |
| **Publish** | Visible as governed metadata for discovery | DMO / Steward; not a data release |
| **Maintain** | Keep metadata current | Steward **R** |
| **Review** | Periodic confirmation of meaning, classification link, status | Steward **R**; Owner **A** for material change |
| **Retire** | Asset no longer in operational catalog use | Owner with DMO record-keeping ([`09-certification-trust-model.md`](09-certification-trust-model.md)) |

---

## 3. Registration consumes Phase 6 (not redesigned)

Registering metadata **shall** follow:

**Metadata Registration Procedure**

`06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`

Phase 6 process (unchanged): Identify dataset → Document business definition → Register metadata → Link classification → Maintain.

This Phase 8 lifecycle **wraps** that procedure. It does not replace it.

---

## 4. What metadata must support `[A][B]`

Governed metadata supports — it does not replace — these program capabilities:

| Capability | How metadata helps |
| --- | --- |
| **Data Governance** | Visible assets, owners, status, and evidence of registration |
| **Data Ownership** | Owner and Steward on every registered asset (Phase 4 titles) |
| **Data Classification** | Rafid tier on the asset record (Phase 5) |
| **Data Quality** | Links to quality status / CDEs when that capability exists (Phase 7; capability-dependent) |
| **Data Lineage** | Coarse source → transformation → target → consumer as metadata (detail = Phase 9) |
| **Data Discovery** | Search without exposing Restricted/Confidential **data** |
| **Data Sharing** | Context for the two Phase 4 sharing decisions (Owner business **A**; PDPO privacy **A**) — metadata is not the share approval |
| **Master Data Management** | Master Data Entity as a Year-1 asset type; no Phase 10 matching design |

---

## 5. What this framework is not

- Not Purview, Collibra, Atlan, Informatica, or any platform
- Not a UI or technical search architecture
- Not automated or column-level lineage
- Not a second Data Quality Framework
- Not NDMO certification

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 8 lifecycle and support list | Sections 2, 4 |
| `[C]` | Data Catalog and Metadata domain **name**; `MCM` as recorded in Phase 2 | Alignment name |
| `[NDMO verification required]` | Specification-level MCM fields and catalog mandates | Not invented |
