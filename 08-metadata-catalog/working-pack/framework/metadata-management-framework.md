# Metadata Management Framework (Working Pack)

**Document ID:** RHC-DG-P8-WP-001  
**Version:** 1.0  
**Status:** Implemented (working design only — not a live catalog)  
**Owner:** DMO `[B]` (method); domain **Data Owner** remains **A** for business meaning  
**Approver:** CDO `[B]`  
**Parent design:** Phase 8 — [`../../01-framework-overview.md`](../../01-framework-overview.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This working pack is the **applied Metadata Management layer** of Phase 8. It shows how Rafid would describe, register, approve, and publish metadata for synthetic healthcare assets.

It does **not** replace Phase 8. It does **not** create a second metadata framework. Locked design remains in:

| Topic | Locked file |
| --- | --- |
| Lifecycle and purpose | [`../../01-framework-overview.md`](../../01-framework-overview.md) |
| Seven metadata categories | [`../../02-metadata-categories.md`](../../02-metadata-categories.md) |
| Asset hierarchy | [`../../03-data-asset-model.md`](../../03-data-asset-model.md) |
| Minimum metadata occupancy | [`../../04-minimum-metadata-standard.md`](../../04-minimum-metadata-standard.md) |
| Glossary structure | [`../../05-business-glossary.md`](../../05-business-glossary.md) |
| Catalog concept | [`../../06-data-catalog-design.md`](../../06-data-catalog-design.md) |
| Registration workflow | [`../../07-asset-registration-workflow.md`](../../07-asset-registration-workflow.md) |
| Catalog MVP | [`../../14-catalog-mvp.md`](../../14-catalog-mvp.md) |
| Registration procedure | [`../../../06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`](../../../06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md) |

This pack adds **working records**: field occupancy, a 25-term glossary, an element-level inventory, a 13-step registration path, and completed sample catalog pages.

---

## 2. What metadata is (working definition) `[A][B]`

**Metadata** is governed information about a data asset: what it means, who owns it, how it is classified, where it comes from, and whether the description can be trusted.

Metadata is **not** the underlying patient, clinical, or claims data. Publishing metadata is **not** an access grant and **not** a data release.

```text
Data Domain
  → Data Asset
    → Data Structure / Object
      → Data Element
```

Year-1 catalog types remain Dataset, Table, Report, Dashboard, and Master Data Entity. This pack also records **Data Element** rows for CDEs and selected watch-items so the inventory can show the hierarchy. Element-level cataloging is **not** required to publish a Dataset ([`../../03-data-asset-model.md`](../../03-data-asset-model.md)).

---

## 3. Working-pack scope `[A]`

| In scope | Out of scope |
| --- | --- |
| Applied field model and occupancy | Catalog platform implementation |
| Business glossary (24 terms) | Official healthcare terminology standards |
| Synthetic metadata inventory | Live Rafid inventory |
| Catalog operating model and MVP checklist | Microsoft Purview / Collibra deployment |
| Asset registration path | Automated ingestion or scanning |
| Sample catalog pages | Real patient, provider, or claims data |

All identifiers are fabricated (`META-PAT-003`, `PAT-000001` as a format example only). No real personal data is used.

---

## 4. How this pack uses Phase 8 categories

Phase 8 defines **seven** categories. This pack groups them into **five working categories** for inventory columns. The mapping is in [`metadata-categories.md`](metadata-categories.md). It is a filing convenience. It does **not** retire Security / Classification or Lineage as Phase 8 categories.

---

## 5. Ownership pattern (unchanged)

```text
Domain → Data Owner (A) → Business Data Steward (R) → IT / Data Custodian (technical)
```

DMO owns the **method**. DMO does **not** become Data Owner of a business domain. Named Owner and Steward titles are the Phase 4 map ([`../../../04-ownership-stewardship/01-domain-ownership-detail.md`](../../../04-ownership-stewardship/01-domain-ownership-detail.md)).

---

## 6. Link to Data Quality (Phase 7)

```text
Metadata asset
      ↓
CDE identification (exactly 13 catalogue CDEs)
      ↓
Quality rules (Phase 7 design)
      ↓
Quality results / issues (when monitoring exists)
      ↓
Governance monitoring
```

This pack **does not** duplicate the CDE catalogue, quality rules, thresholds, or issue procedure. Quality metadata is **capability-dependent**. Fake scores are not invented.

---

## 7. NDMO / PDPL position

Data Catalog and Metadata is an NDMO knowledge-domain **name** (`MCM` as recorded in Phase 2) `[C]`. This pack is conceptually aligned with relevant data management governance considerations.

It is **not** NDMO compliant. It is **not** PDPL compliant. Official metadata fields and categories remain `[NDMO verification required]`.

---

## 8. What this file does not do

- Does not change Phase 8 locked design
- Does not add CDEs (catalogue remains **13**)
- Does not expand catalog MVP beyond the three approved domains
- Does not claim a tool deployment
