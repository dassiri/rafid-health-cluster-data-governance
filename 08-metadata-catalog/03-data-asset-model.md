# Data Asset Model

**Document ID:** RHC-DG-P8-003  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (model method); Data Owner **A** for assets in the domain  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Locked hierarchy and Year-1 asset types; API and Data Product deferred.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Physical data model; API catalog; data-product marketplace

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **data asset hierarchy** and **Year-1 catalog asset types** `[A][B]`.

The model is **not** expanded in this phase. It is not a technical schema and not an NDMO-mandated asset taxonomy `[NDMO verification required]`.

---

## 2. Hierarchy (locked)

```text
Data Domain
→ Data Asset
→ Data Structure / Object
→ Data Element
```

| Level | Meaning |
| --- | --- |
| **Data Domain** | One of the eight Phase 4 ownership domains. Exactly one Data Owner per domain. |
| **Data Asset** | The catalog-registered unit (Year-1 types below). Classification is **dataset-level** in Phase 5; a Dataset asset carries the Rafid tier. Other Year-1 types inherit or link that governance context; they are not a new classification scheme. |
| **Data Structure / Object** | Table, file structure, or equivalent object **inside** an asset, when known. Not required to explode every column on day one. |
| **Data Element** | A field. Phase 7 CDEs are data elements with dedicated quality governance; not every element is a CDE. |

Do **not** catalog at domain level only. Do **not** require column-level cataloging for Year-1 publish.

---

## 3. Year-1 asset types (locked) `[A][B]`

| Asset type | Year-1 catalog |
| --- | --- |
| **Dataset** | Yes — primary operational unit aligned to Phase 6 registration |
| **Table** | Yes — when a governed table is the useful discovery unit |
| **Report** | Yes — governed output, not a shadow spreadsheet of record |
| **Dashboard** | Yes — governed analytic surface |
| **Master Data Entity** | Yes — Person, Provider, reference entity **as a catalog type**; Phase 10 matching is not designed |

**Deferred — not first-class Year-1 types**

| Type | Status |
| --- | --- |
| **API** | Deferred |
| **Data Product** | Deferred |

Do not add further first-class types in this phase.

---

## 4. Illustrative walk-down `[A]`

Fictional only — not a live inventory.

```text
Domain: Patient / Person Master Data
  Asset (Dataset): Patient demographic dataset [A]
    Structure: Registration table (conceptual)
      Element: National ID (also Phase 7 CDE-001)
```

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved hierarchy and Year-1 types | Sections 2–3 |
| `[C]` | Data Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Official NDMO asset-type mandates | Not claimed |
