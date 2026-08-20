# Minimum Metadata Model (Working Pack)

**Document ID:** RHC-DG-P8-WP-005  
**Version:** 1.0  
**Status:** Implemented (working design only — not a physical catalog schema)  
**Owner:** DMO `[B]` (field method); Data Owner **A** for business field values  
**Parent design:** [`../../04-minimum-metadata-standard.md`](../../04-minimum-metadata-standard.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This is a **proportionate** minimum metadata model for Rafid healthcare data assets `[A][B]`.

It is implementable. It is not a maximum enterprise schema. It is not an official NDMO field list `[NDMO verification required]`. **No compliance is claimed.**

Field-by-field definitions: [`metadata-field-definitions.md`](metadata-field-definitions.md)  
Machine-readable list: [`minimum-metadata-model.csv`](minimum-metadata-model.csv)

---

## 2. Occupancy rules

Phase 8 uses Mandatory / Recommended / Capability-dependent. This pack uses the same three ideas with working labels:

| Occupancy | Meaning | Maps to Phase 8 |
| --- | --- | --- |
| **Required** | Needed to **publish** an operational catalog asset | Mandatory |
| **Conditional** | Required **when a condition is true**; otherwise omit rather than invent | Capability-dependent, plus type-specific technical fields |
| **Optional** | Expected for a healthy record; absence is a metadata-quality gap, not a publish block if Required is complete | Recommended, and remaining capability-dependent fields |

Not every field is required. A model that makes every column mandatory cannot be implemented in Year-1 `[B]`.

---

## 3. Why some metadata is required

| Required field | Why it is required |
| --- | --- |
| Asset ID | Stable handle for the record; without it, review and lineage pointers break |
| Asset Name | People cannot discover what they cannot name |
| Business Domain | Ownership and Steward assignment are domain-based (Phase 4) |
| Business Definition | Catalog content is Owner-accepted meaning (Phase 4 row 1 / row 8) |
| Data Owner | Accountability cannot sit on “the system” or on DMO |
| Business Data Steward | Day-to-day maintenance needs a named executing role |
| Source System | Primary system **context where one applies** — not a demand for exactly one source |
| Classification | Unlabeled is not Public (Phase 5 / PRC-002) |
| Lifecycle Status | Distinguishes draft, active, deprecated, and retired |
| Approval Status | Distinguishes work-in-progress from Owner/DMO-accepted records |

**System / Primary System** remains required even for derived assets. Derived or aggregated assets may list multiple contributing systems, or “derived / none directly,” with contributors noted. The field is not dropped.

---

## 4. Field list

| Field | Category | Occupancy | Condition (if Conditional) |
| --- | --- | --- | --- |
| Asset ID | Governance | Required | — |
| Asset Name | Business | Required | — |
| Asset Type | Technical | Optional | Filled throughout this pack so Dataset / Master Data Entity / Data Element is visible. Phase 8 lists it as Recommended, not Mandatory for publish |
| Business Domain | Governance | Required | — |
| Business Definition | Business | Required | — |
| Business Owner (Data Owner) | Governance | Required | — |
| Business Data Steward | Governance | Required | — |
| Source System | Technical | Required | — |
| Source Dataset | Technical | Conditional | Required when Asset Type = Data Element or Table and a parent dataset is registered |
| Database / Schema | Technical | Optional | — |
| Table | Technical | Conditional | Required when Asset Type = Table or Data Element |
| Column | Technical | Conditional | Required when Asset Type = Data Element |
| Data Type | Technical | Conditional | Required when Asset Type = Data Element |
| Classification | Governance | Required | — |
| Criticality | Governance | Optional | Working High / Medium / Low. **Not** a numeric CDE rank. Phase 7 does not rank CDEs |
| CDE Status | Governance | Conditional | Required when Asset Type = Data Element |
| Business Rules | Business | Optional | — |
| Data Quality Status | Data Quality | Conditional | Required when the asset is a confirmed CDE or a parent asset that contains confirmed CDEs **and** Phase 7 design exists |
| Refresh Frequency | Operational | Conditional | Required when a useful operational frequency is known for a Dataset |
| Lifecycle Status | Governance | Required | — |
| Approval Status | Governance | Required | — |
| Last Reviewed | Operational | Optional | — |
| Related Business Terms | Business | Optional | — |
| Lineage Reference | Governance (stores Phase 8 Lineage Metadata) | Conditional | Required for MVP Dataset / Master Data Entity rows; optional for watch-item elements |

---

## 5. Allowed values (working)

| Field | Allowed values `[A]` |
| --- | --- |
| Asset Type | Dataset · Table · Report · Dashboard · Master Data Entity · Data Element (working-pack teaching type) |
| Business Domain | The eight Phase 4 domain names |
| Classification | Public · Internal · Confidential · Restricted |
| CDE Status | Yes — {CDE-ID} · No — watch-item · No |
| Lifecycle Status | Draft · Active · Deprecated · Retired |
| Approval Status | Pending Steward Validation · Pending Owner Approval · Pending DMO Check · Approved · Returned |
| Criticality | High · Medium · Low |
| Data Quality Status | CDE — quality rules designed (Phase 7) · Watch-item — not in the 13-CDE catalogue · Not applicable · Known issue logged (illustrative) |

Trust / certification status from Phase 8 (Registered / Reviewed / Certified / Deprecated / Retired) remains the catalog **trust** language. Lifecycle Status in this pack is the operational catalog state. Certified is the Owner’s trust decision; it is not a national seal.

---

## 6. Asset hierarchy in this model

```text
Data Domain → Data Asset (Dataset / Master Data Entity)
                → Data Structure (Table)
                  → Data Element (column)
```

Publish can stop at Dataset. This pack also registers selected elements so CDEs and watch-items are visible beside their parent asset.

---

## 7. What this file does not do

- Does not implement a database schema or a catalog tool
- Does not add CDEs
- Does not invent NDMO field IDs
