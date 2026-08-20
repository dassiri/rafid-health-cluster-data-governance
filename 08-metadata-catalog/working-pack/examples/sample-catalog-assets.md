# Sample Catalog Assets (Working Pack)

**Document ID:** RHC-DG-P8-WP-012  
**Version:** 1.0  
**Status:** Implemented (illustrative pages only — not a live catalog)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

These eight pages are **synthetic**. They use inventory IDs from [`../metadata-inventory/metadata-inventory.md`](../metadata-inventory/metadata-inventory.md). No real patient or provider information is used.

Certification language is Rafid **internal trust** (Phase 8). It is not regulatory or NDMO certification.

All eight assets are in **catalog MVP** domains.

---

## 1. Patient

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-PAT-001 |
| Asset Name | Patient |
| Asset Type | Master Data Entity |
| Domain | Patient / Person Master Data |
| Definition | Logical person master identity used for registration and care access. Not a physical MDM hub in this drop. |
| Owner | Patient Access & Experience Director |
| Steward | Head of Patient Registration & Access |
| Source | Registration / MPI (SYN-REG) |
| Classification | Restricted |
| Criticality | High |
| CDE | Context for CDE-001 (National ID) and CDE-002 (Patient identifier / MRN) |
| Quality Status | CDE — quality rules designed (Phase 7) for contained CDEs |
| Refresh Frequency | Event-driven (registration create/update) |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Certified (illustrative Owner acceptance of the description) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Patient; Patient ID; National ID |
| Lineage Reference | LIN-REG-PAT-001 — Registration / MPI → Person master → Encounter and billing consumers |

MVP checklist: domain, Owner, Steward, minimum metadata, classification, CDE context, definition approved, quality status, lineage, catalog approval — complete (illustrative).

---

## 2. Patient_ID

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-PAT-003 |
| Asset Name | Patient_ID |
| Asset Type | Data Element |
| Domain | Patient / Person Master Data |
| Definition | The cluster patient identifier (MRN) used to locate the person in operational systems. |
| Owner | Patient Access & Experience Director |
| Steward | Head of Patient Registration & Access |
| Source | Registration / MPI (SYN-REG) |
| Source Dataset | Patient Registration Dataset (META-PAT-002) |
| Database / Schema | mpi.patient |
| Table | patient_master |
| Column | patient_id |
| Data Type | String |
| Classification | Restricted |
| Criticality | High |
| CDE | Yes — **CDE-002** |
| Business Rules | Must be unique in the governed person population; must not be blank for Active patients. |
| Quality Status | CDE — quality rules designed (Phase 7). Baseline dimensions: Accuracy, Completeness, Validity. Dependent: Uniqueness, Consistency, Integrity |
| Refresh Frequency | Inherited from parent dataset |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Certified (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Patient ID; Patient |
| Lineage Reference | LIN-REG-PAT-001 |

---

## 3. Date_of_Birth

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-PAT-005 |
| Asset Name | Date_of_Birth |
| Asset Type | Data Element |
| Domain | Patient / Person Master Data |
| Definition | The recorded date of birth used to confirm identity and derive age. |
| Owner | Patient Access & Experience Director |
| Steward | Head of Patient Registration & Access |
| Source | Registration / MPI (SYN-REG) |
| Source Dataset | Patient Registration Dataset (META-PAT-002) |
| Database / Schema | mpi.patient |
| Table | patient_master |
| Column | date_of_birth |
| Data Type | Date |
| Classification | Restricted |
| Criticality | Medium |
| CDE | No — watch-item. **Not** a 14th CDE |
| Business Rules | Must be a valid past date. |
| Quality Status | Watch-item — not in the 13-CDE catalogue |
| Refresh Frequency | Inherited from parent dataset |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Reviewed (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Date of Birth; Patient |
| Lineage Reference | LIN-REG-PAT-001 |

This page shows a **complete** catalog record for a non-CDE element. Completeness of the description does not promote the field into the CDE catalogue.

---

## 4. Encounter

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-ENC-001 |
| Asset Name | Encounter |
| Asset Type | Master Data Entity |
| Domain | Clinical / Medical Records Data |
| Definition | Logical encounter identity for a defined care interaction recorded in the clinical record context. |
| Owner | Chief Medical Officer (CMO) |
| Steward | Head of Health Information Management (HIM) |
| Source | EMR clinical (SYN-EHR) |
| Classification | Restricted |
| Criticality | High |
| CDE | Context for CDE-003 (Diagnosis code) and CDE-004 (Encounter documentation timestamp) |
| Quality Status | CDE — quality rules designed (Phase 7) for contained CDEs |
| Refresh Frequency | Event-driven (encounter documentation) |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Certified (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Encounter; Encounter ID; Encounter Date |
| Lineage Reference | LIN-ENC-001 — Person master + EMR clinical → Encounter documentation → Claims / quality consumers |

---

## 5. Encounter_ID

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-ENC-003 |
| Asset Name | Encounter_ID |
| Asset Type | Data Element |
| Domain | Clinical / Medical Records Data |
| Definition | The unique identifier of a recorded care encounter. |
| Owner | Chief Medical Officer (CMO) |
| Steward | Head of Health Information Management (HIM) |
| Source | EMR clinical (SYN-EHR) |
| Source Dataset | Encounter Documentation Dataset (META-ENC-002) |
| Database / Schema | emr.clinical |
| Table | encounter_documentation |
| Column | encounter_id |
| Data Type | String |
| Classification | Restricted |
| Criticality | High |
| CDE | No — not one of the 13 catalogue CDEs |
| Business Rules | Must be unique in the governed encounter population. |
| Quality Status | Watch-item — not in the 13-CDE catalogue |
| Refresh Frequency | Inherited from parent dataset |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Reviewed (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Encounter ID; Encounter |
| Lineage Reference | LIN-ENC-001 |

---

## 6. Encounter_Date

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-ENC-004 |
| Asset Name | Encounter_Date |
| Asset Type | Data Element |
| Domain | Clinical / Medical Records Data |
| Definition | The date associated with encounter documentation (Phase 7 CDE-004 timestamp context). |
| Owner | Chief Medical Officer (CMO) |
| Steward | Head of Health Information Management (HIM) |
| Source | EMR clinical (SYN-EHR) |
| Source Dataset | Encounter Documentation Dataset (META-ENC-002) |
| Database / Schema | emr.clinical |
| Table | encounter_documentation |
| Column | encounter_date |
| Data Type | Date |
| Classification | Restricted |
| Criticality | High |
| CDE | Yes — **CDE-004** |
| Business Rules | Must not be in the future relative to the documentation calendar. |
| Quality Status | CDE — quality rules designed (Phase 7). Baseline dimensions plus Timeliness and Integrity as dependent dimensions |
| Refresh Frequency | Inherited from parent dataset |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Certified (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Encounter Date; Encounter |
| Lineage Reference | LIN-ENC-001 |

---

## 7. Diagnosis_Code

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-ENC-007 |
| Asset Name | Diagnosis_Code |
| Asset Type | Data Element |
| Domain | Clinical / Medical Records Data |
| Definition | A recorded clinical diagnosis code in the medical record context. |
| Owner | Chief Medical Officer (CMO) |
| Steward | Head of Health Information Management (HIM) |
| Source | EMR clinical (SYN-EHR) |
| Source Dataset | Encounter Documentation Dataset (META-ENC-002) |
| Database / Schema | emr.clinical |
| Table | encounter_documentation |
| Column | diagnosis_code |
| Data Type | String |
| Classification | Restricted |
| Criticality | High |
| CDE | Yes — **CDE-003** |
| Business Rules | Must exist on the approved diagnosis reference list used for validity. |
| Quality Status | CDE — quality rules designed (Phase 7). Dependent dimensions typically Integrity and Consistency |
| Refresh Frequency | Inherited from parent dataset |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Certified (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Diagnosis; Encounter |
| Lineage Reference | LIN-ENC-001 |

---

## 8. Claim_ID

| Field | Value `[A]` |
| --- | --- |
| Asset ID | META-CLM-002 |
| Asset Name | Claim_ID |
| Asset Type | Data Element |
| Domain | Financial / Billing & Claims Data |
| Definition | The unique identifier of a claim record in the governed claims population. |
| Owner | Chief Financial Officer (CFO) |
| Steward | Revenue Cycle Manager |
| Source | Billing / claims (SYN-BILL) |
| Source Dataset | Claim Submission Dataset (META-CLM-001) |
| Database / Schema | bill.claims |
| Table | claim_submission |
| Column | claim_id |
| Data Type | String |
| Classification | Restricted |
| Criticality | High |
| CDE | Yes — **CDE-007** |
| Business Rules | Must be unique in the governed claims population. |
| Quality Status | CDE — quality rules designed (Phase 7). Dependent dimensions typically Uniqueness and Integrity |
| Refresh Frequency | Inherited from parent dataset (daily batch — illustrative, not an SLA) |
| Lifecycle Status | Active |
| Approval Status | Approved |
| Trust status (Phase 8) | Certified (illustrative) |
| Last Reviewed | 2026-08-01 |
| Related Glossary Terms | Claim Identifier; Claim |
| Lineage Reference | LIN-CLM-001 — Encounter → Charge capture → Claim submission → External claims interchange (generic; not a named national product) |

---

## Out of these eight pages (still in inventory)

Provider (`META-PRV-001`), Provider_ID (`META-PRV-002`), Facility (`META-FAC-001`), and Facility_ID (`META-FAC-002`) are complete in the inventory CSV. They are **outside** catalog MVP operating scope and are therefore not presented as Year-1 published sample pages.

---

## What this file does not do

- Does not represent a Purview or Collibra extract
- Does not use real identifiers
- Does not add CDEs
