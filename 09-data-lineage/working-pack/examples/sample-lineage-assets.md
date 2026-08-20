# Sample Catalog Assets with Lineage (Working Pack)

**Document ID:** RHC-DG-P9-WP-013  
**Version:** 1.0  
**Status:** Implemented (illustrative pages only — not a live catalog)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

**Synthetic / Illustrative / Non-production.**

These pages show how **catalog assets connect to lineage**. They reuse Phase 8 working-pack IDs and minimum metadata. They do **not** duplicate the Metadata Management working pack.

Full catalog samples remain in [`../../../08-metadata-catalog/working-pack/examples/sample-catalog-assets.md`](../../../08-metadata-catalog/working-pack/examples/sample-catalog-assets.md).

Certification language is Rafid **internal trust** (Phase 8). It is not regulatory or NDMO certification.

---

## Integration pattern

```text
Data Catalog
      ↓
Data Asset
      ↓
Metadata (Phase 8 minimum model)
      ↓
Lineage Reference
      ↓
Source / Transformation / Target / Consumer
```

The catalog points to lineage (`LIN-*` / chain IDs). Lineage points back to catalog Asset IDs (`META-*`).

---

## 1. Patient (MVP master)

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-PAT-001 |
| Asset Name | Patient |
| Asset Type | Master Data Entity |
| Domain | Patient / Person Master Data |
| Business Definition | Logical person master identity used for registration and care access. Not a physical MDM hub in this drop. |
| Data Owner | Patient Access & Experience Director |
| Business Data Steward | Head of Patient Registration & Access |
| System | Registration / MPI (SYN-REG) |
| Classification | Restricted |
| CDE Status | Context for CDE-001 (National ID) and CDE-002 (Patient identifier / MRN) |
| Quality Status | CDE — quality rules designed (Phase 7) for contained CDEs |
| Lineage Reference | LIN-REG-PAT-001; LIN-001 (from registration); LIN-002 (to encounter); LIN-006 / LIN-007 (selective field hops) |
| Lifecycle Status | Active |
| Catalog Status | Certified (illustrative Owner acceptance of the **description**) |

**Lineage snapshot (asset-level):**

```text
Source: Patient Registration Dataset (META-PAT-002)
Transformation: persist / match identity (conceptual)
Target: Patient (META-PAT-001)
Consumer: Encounter; billing identity use
```

---

## 2. Patient Registration Dataset

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-PAT-002 |
| Asset Name | Patient Registration Dataset |
| Asset Type | Dataset |
| Domain | Patient / Person Master Data |
| Business Definition | Originating capture dataset for registrable person identity. |
| Data Owner | Patient Access & Experience Director |
| Business Data Steward | Head of Patient Registration & Access |
| System | Registration / MPI (SYN-REG) |
| Classification | Restricted |
| CDE Status | Contains CDE-001, CDE-002 |
| Quality Status | CDE — quality rules designed (Phase 7) |
| Lineage Reference | LIN-001 (source hop); LIN-006; LIN-007 |
| Lifecycle Status | Active |
| Catalog Status | Certified (illustrative) |

**Lineage role:** Source (originating capture) on the locked E2E chain.

---

## 3. Encounter

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-ENC-001 |
| Asset Name | Encounter |
| Asset Type | Master Data Entity |
| Domain | Clinical / Medical Records Data |
| Business Definition | Logical encounter identity for a defined care interaction recorded in the clinical record context. |
| Data Owner | Chief Medical Officer (CMO) |
| Business Data Steward | Head of Health Information Management (HIM) |
| System | EMR clinical (SYN-EHR) |
| Classification | Restricted |
| CDE Status | Context for CDE-003 (Diagnosis code) and CDE-004 (Encounter documentation timestamp) |
| Quality Status | CDE — quality rules designed (Phase 7) for contained CDEs |
| Lineage Reference | LIN-ENC-001; LIN-002 (from Patient); LIN-003 (to claims via documentation dataset); LIN-010 |
| Lifecycle Status | Active |
| Catalog Status | Certified (illustrative) |

**Lineage snapshot:**

```text
Source: Patient (META-PAT-001) + EMR clinical documentation
Transformation: clinical documentation and coding (conceptual)
Target: Encounter / Encounter Documentation Dataset
Consumer: Claims extract; illustrative clinical reporting
```

---

## 4. Claim Submission Dataset (Claims Extract)

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-CLM-001 |
| Asset Name | Claim Submission Dataset |
| Asset Type | Dataset |
| Domain | Financial / Billing & Claims Data |
| Business Definition | Governed claims extract used to prepare a claim for reimbursement. Maps to the Phase 9 MVP asset “Claims Extract”. |
| Data Owner | Chief Financial Officer (CFO) |
| Business Data Steward | Revenue Cycle Manager |
| System | Billing / claims (SYN-BILL) |
| Classification | Restricted (illustrative Owner-assessed dataset-level tier — not auto-inherited) |
| CDE Status | Contains CDE-007, CDE-008 |
| Quality Status | CDE — quality rules designed (Phase 7) |
| Lineage Reference | LIN-CLM-001; LIN-003; LIN-004; LIN-005; LIN-008; LIN-009; LIN-011; LIN-012 |
| Lifecycle Status | Active |
| Catalog Status | Certified (illustrative) |

**Lineage snapshot:**

```text
Source: Encounter Documentation Dataset (META-ENC-002); Patient identity consumed
Transformation: charge capture and claim composition (conceptual)
Target: Claim Submission Dataset (META-CLM-001)
Consumer: Generic External Claims Interchange; Patient Claim Rejection Rate; financial reporting
```

---

## 5. Patient_ID (selective element page)

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-PAT-003 |
| Asset Name | Patient_ID |
| Asset Type | Data Element |
| Domain | Patient / Person Master Data |
| Business Definition | The cluster patient identifier (MRN) used to locate the person in operational systems. |
| Data Owner | Patient Access & Experience Director |
| Business Data Steward | Head of Patient Registration & Access |
| System | Registration / MPI (SYN-REG) |
| Classification | Restricted |
| CDE Status | Yes — **CDE-002** |
| Quality Status | CDE — quality rules designed (Phase 7) |
| Lineage Reference | LIN-006; chain LIN-REG-PAT-001 |
| Lifecycle Status | Active |
| Catalog Status | Certified (illustrative) |

Element-level cataloging is a teaching record. Year-1 publish of the parent master does **not** require every column to be a first-class catalog type.

---

## 6. Bidirectional index (this pack)

| Catalog asset | Points to lineage | Lineage points back |
| --- | --- | --- |
| META-PAT-001 | LIN-001, LIN-002, LIN-006, LIN-007 | Yes |
| META-PAT-002 | LIN-001, LIN-006, LIN-007 | Yes |
| META-PAT-003 | LIN-006 | Yes |
| META-ENC-001 | LIN-002, LIN-010 | Yes |
| META-ENC-002 | LIN-003, LIN-008, LIN-010, LIN-013 | Yes |
| META-CLM-001 | LIN-003–LIN-005, LIN-008–LIN-009, LIN-011–LIN-012 | Yes |
| META-CLM-002 | LIN-009 | Yes |
| META-ENC-007 | LIN-008 | Yes |

---

## 7. What this file does not do

- Does not replace the Phase 8 sample catalog pages
- Does not add CDEs or MVP domains
- Does not represent a Purview or Collibra extract
- Does not use real identifiers
