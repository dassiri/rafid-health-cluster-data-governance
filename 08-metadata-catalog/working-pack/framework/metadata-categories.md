# Metadata Categories (Working Grouping)

**Document ID:** RHC-DG-P8-WP-002  
**Version:** 1.0  
**Status:** Implemented (working design only)  
**Owner:** DMO `[B]` (category method)  
**Parent design:** [`../../02-metadata-categories.md`](../../02-metadata-categories.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

Phase 8 locks **seven** Rafid metadata categories. This file defines **five working categories** used in the inventory and minimum metadata model.

These five names are a **Rafid working-pack grouping** `[A][B]`. They are **not** an official NDMO metadata taxonomy. Official NDMO category names remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Mapping to Phase 8 (locked seven)

| Working category (this pack) | Phase 8 category | How the pack uses it |
| --- | --- | --- |
| **Business Metadata** | Business Metadata | Definition, term, purpose, usage |
| **Technical Metadata** | Technical Metadata | System, structure, table, column, data type |
| **Operational Metadata** | Operational Metadata | Refresh / availability context |
| **Governance Metadata** | Governance Metadata **and** Security / Classification Metadata | Owner, Steward, domain, classification, CDE flag, lifecycle, approval |
| **Data Quality Metadata** | Quality Metadata | Quality status, dimension, known issues — when Phase 7 capability exists |

**Lineage Metadata** (Phase 8 category 7) is recorded as the field **Lineage Reference**. It is not a sixth inventory category. Coarse lineage remains capability-dependent. Detailed lineage is Phase 9.

This mapping does **not** drop Security / Classification. Classification stays a **mandatory** governance field. Unlabeled is not Public.

---

## 3. The five working categories

### 3.1 Business Metadata

Describes **meaning and intended use**.

| Example field | Occupancy in this pack |
| --- | --- |
| Asset Name | Required |
| Business Definition | Required |
| Business Term / Related Business Terms | Optional (recommended) |
| Business Domain | Required |
| Business Purpose / intended use | Optional |
| Business Rules | Optional |
| Approved Usage | Optional |

**Owner of meaning:** Data Owner **A**. Steward drafts.

### 3.2 Technical Metadata

Describes **where the asset sits technically**, at a governance minimum.

| Example field | Occupancy in this pack |
| --- | --- |
| Source System / Primary System | Required |
| Source Dataset | Conditional (when the element sits in a parent dataset) |
| Database / Schema | Optional |
| Table | Conditional (Table or Data Element) |
| Column | Conditional (Data Element) |
| Data Type | Conditional (Data Element) |
| Technical Description | Optional |

Year-1 publish does **not** require column-level metadata. Element rows in this pack are teaching records for CDEs and selected watch-items.

### 3.3 Operational Metadata

Describes **how current the asset is expected to be**, at governance level. Not a monitoring platform.

| Example field | Occupancy in this pack |
| --- | --- |
| Refresh Frequency | Conditional (when a useful frequency is known) |
| Last Updated (metadata) | Optional |
| Data Availability / SLA | Optional — no numeric SLA is invented |
| Processing Frequency | Optional |
| Data Pipeline | Optional |

Absence is a known gap, not a fake complete record.

### 3.4 Governance Metadata

Describes **accountability, classification, and catalog state**.

| Example field | Occupancy in this pack |
| --- | --- |
| Data Owner | Required |
| Business Data Steward | Required |
| Classification | Required (Rafid Public / Internal / Confidential / Restricted) |
| Criticality | Optional (working High / Medium / Low — **not** a CDE rank) |
| CDE Status | Conditional (required for Data Element rows in this pack) |
| Domain | Required |
| Lifecycle Status | Required |
| Approval Status | Required |

Classification labels are Rafid working tiers `[A][B]`. They are **not** NDMO national tiers.

### 3.5 Data Quality Metadata

Describes **whether quality governance exists for the asset**. It is not a second Data Quality Framework.

| Example field | Occupancy in this pack |
| --- | --- |
| Data Quality Status | Conditional (when Phase 7 applies) |
| Quality Dimension | Optional |
| Quality Rule | Optional (pointer only — rules live in Phase 7) |
| Known Issues | Conditional (when logged) |
| Remediation Status | Conditional (when an issue exists) |

Do **not** invent quality scores. This repository does not measure Rafid performance.

---

## 4. Mandatory vs capability-dependent (unchanged)

| Group | Working categories | Phase 8 rule |
| --- | --- | --- |
| **Mandatory for publish** | Business (minimum); Governance including classification; Technical (system context) | Required for a published operational catalog asset |
| **Capability-dependent** | Operational; Data Quality; Lineage Reference | Recorded when the capability exists |

---

## 5. What this file does not do

- Does not replace the seven Phase 8 categories
- Does not claim NDMO category names
- Does not require all five categories to be fully populated on day one
