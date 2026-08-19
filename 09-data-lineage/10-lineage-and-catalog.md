# Lineage and the Data Catalog

**Document ID:** RHC-DG-P9-010  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (catalog lineage method); Data Owner **A** for domain content  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 8 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Supplies Phase 8 Lineage Metadata; no catalog product.

**Phase:** 9 — Data lineage  
**Does not decide:** Catalog UI; technical lineage graphs in a tool

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records how Phase 9 **fills** the Phase 8 **Lineage Metadata** category. It does **not** change the Phase 8 metadata model.

Phase 8 treated Lineage Metadata as **capability-dependent**. This phase is the capability: governed conceptual lineage for prioritized flows.

---

## 2. Conceptual lineage fields (Phase 8 — unchanged)

| Field | Use in Phase 9 |
| --- | --- |
| **Upstream source** | Source asset or system context |
| **Downstream consumers** | Target uses (report, interchange) — not access grants |
| **Transformation reference** | Conceptual transformation name/description — not ETL code |

These remain capability-dependent occupancy: do not invent fake lineage to look complete.

---

## 3. What the catalog may expose

At **asset level**, the catalog may expose:

```text
Source → Target → Consumer
```

That is **governed metadata** for discovery. It is **not** the underlying Restricted or Confidential **data** (Phase 8 search rule unchanged).

Detailed **technical** lineage remains out of scope (Year-1 technical lineage is conceptual only; no scanner).

---

## 4. Registration relationship

Publishing lineage metadata uses the Phase 9 operating workflow ([`12-registration-workflow.md`](12-registration-workflow.md)) **and** existing Phase 8 catalog/metadata governance (including the Metadata Registration Procedure by title/path). **No new Phase 6 procedure. No invented document ID.**

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Asset-level exposure; field mapping | Sections 2–3 |
| `[C]` | Data Catalog and Metadata domain **name** (`MCM` as recorded in Phase 2) | Context |
| `[NDMO verification required]` | Official NDMO catalog-lineage field list | Not claimed |
