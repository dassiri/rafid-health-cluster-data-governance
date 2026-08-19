# Data Lifecycle and Metadata

**Document ID:** RHC-DG-P11-016  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for domain metadata content; DMO catalog method `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 8 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 8 hierarchy and seven categories reused; lifecycle fields added as occupancy, not new categories.

**Phase:** 11 — Data lifecycle  
**Does not decide:** New metadata categories or a new catalog product

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **reuses the Phase 8 hierarchy and categories**.

**Do not redesign Phase 8 metadata categories or hierarchy.**

Hierarchy (locked):

```text
Data Domain
→ Data Asset
→ Data Structure / Object
→ Data Element
```

Seven categories (locked): Business; Governance; Security / Classification; Technical (mandatory group with the first three); Quality; Operational; Lineage (capability-dependent).

---

## 2. Lifecycle metadata occupancy `[A][B]`

These fields may be recorded on the **asset** (primarily Dataset). They are **not** an eighth category.

| Field | Typical Phase 8 home | Intent |
| --- | --- | --- |
| **Lifecycle status** | Governance Metadata | Active / Archived / Disposed (or equivalent working status) |
| **Creation date** | Governance / Operational (governance-level) | When the asset/record was created or acquired |
| **Last review** | Governance Metadata | Last Owner/Steward lifecycle review |
| **Retention rule** | Governance Metadata | Retention Rule ID |
| **Archive status** | Governance Metadata | Whether archived; link to Archive Register |
| **Disposal eligibility** | Governance Metadata | Eligible / not eligible / on hold / period unverified |
| **Legal hold status** | Governance Metadata | Hold active or not |

Business Data Steward maintains this occupancy. Data Owner **A** for content approval (Phase 4 row 8).

Year-1 asset types unchanged (Dataset, Table, Report, Dashboard, Master Data Entity). API and Data Product remain deferred.

---

## 3. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Lifecycle fields as occupancy | Section 2 |
| `[C]` | Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Official NDMO lifecycle-metadata specs | Not claimed |
