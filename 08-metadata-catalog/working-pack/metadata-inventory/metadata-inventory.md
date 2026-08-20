# Metadata Inventory (Working Pack)

**Document ID:** RHC-DG-P8-WP-008  
**Version:** 1.0  
**Status:** Implemented (synthetic inventory only — not a live register)  
**Owner:** Each domain Data Owner **A** for assets in that domain; DMO owns the inventory method `[B]`  
**Parent design:** Phase 8 asset model and minimum metadata standard  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This inventory is a **synthetic** working register of 20 Rafid data assets `[A]`.

It applies the minimum metadata model to healthcare entities already used in the framework: Patient, Provider, Facility, Encounter, and Claim.

It is **not** a live Rafid inventory, **not** a catalog product extract, and **not** measured operational evidence.

Machine-readable register: [`metadata-inventory.csv`](metadata-inventory.csv)

---

## 2. Coverage

| Domain | Assets | Catalog MVP |
| --- | --- | --- |
| Patient / Person Master Data | 6 | In MVP |
| Clinical / Medical Records Data | 7 | In MVP |
| Financial / Billing & Claims Data | 3 | In MVP |
| Provider / Clinician Data | 2 | Outside MVP (framework only) |
| Reference / Organizational Master Data | 2 | Outside MVP (framework only) |

HR / Workforce, Supply Chain & Asset, and Quality & Patient Safety remain in the Phase 8 **framework** ([`../../13-metadata-by-domain.md`](../../13-metadata-by-domain.md)). They are not expanded in this working inventory.

Provider and Facility are inventoried because Encounter depends on them. They are **not** in the Year-1 catalog MVP operating cut ([`../../14-catalog-mvp.md`](../../14-catalog-mvp.md)).

---

## 3. Asset list

| Asset ID | Asset Name | Type | Domain | CDE Status | Classification | MVP |
| --- | --- | --- | --- | --- | --- | --- |
| META-PAT-001 | Patient | Master Data Entity | Patient / Person Master Data | Context for CDE-001, CDE-002 | Restricted | In MVP |
| META-PAT-002 | Patient Registration Dataset | Dataset | Patient / Person Master Data | Contains CDE-001, CDE-002 | Restricted | In MVP |
| META-PAT-003 | Patient_ID | Data Element | Patient / Person Master Data | Yes — CDE-002 | Restricted | In MVP |
| META-PAT-004 | National_ID | Data Element | Patient / Person Master Data | Yes — CDE-001 | Restricted | In MVP |
| META-PAT-005 | Date_of_Birth | Data Element | Patient / Person Master Data | No — watch-item | Restricted | In MVP |
| META-PAT-006 | Gender | Data Element | Patient / Person Master Data | No | Restricted | In MVP |
| META-ENC-001 | Encounter | Master Data Entity | Clinical / Medical Records Data | Context for CDE-003, CDE-004 | Restricted | In MVP |
| META-ENC-002 | Encounter Documentation Dataset | Dataset | Clinical / Medical Records Data | Contains CDE-003, CDE-004 | Restricted | In MVP |
| META-ENC-003 | Encounter_ID | Data Element | Clinical / Medical Records Data | No | Restricted | In MVP |
| META-ENC-004 | Encounter_Date | Data Element | Clinical / Medical Records Data | Yes — CDE-004 | Restricted | In MVP |
| META-ENC-005 | Admission_Date | Data Element | Clinical / Medical Records Data | No — watch-item | Restricted | In MVP |
| META-ENC-006 | Discharge_Date | Data Element | Clinical / Medical Records Data | No — watch-item | Restricted | In MVP |
| META-ENC-007 | Diagnosis_Code | Data Element | Clinical / Medical Records Data | Yes — CDE-003 | Restricted | In MVP |
| META-CLM-001 | Claim Submission Dataset | Dataset | Financial / Billing & Claims Data | Contains CDE-007, CDE-008 | Restricted | In MVP |
| META-CLM-002 | Claim_ID | Data Element | Financial / Billing & Claims Data | Yes — CDE-007 | Restricted | In MVP |
| META-CLM-003 | Charge_Code | Data Element | Financial / Billing & Claims Data | Yes — CDE-008 | Restricted | In MVP |
| META-PRV-001 | Provider | Master Data Entity | Provider / Clinician Data | Context for CDE-005 | Confidential | Outside MVP |
| META-PRV-002 | Provider_ID | Data Element | Provider / Clinician Data | Yes — CDE-005 | Confidential | Outside MVP |
| META-FAC-001 | Facility | Master Data Entity | Reference / Organizational Master Data | Context for CDE-013 | Internal | Outside MVP |
| META-FAC-002 | Facility_ID | Data Element | Reference / Organizational Master Data | Yes — CDE-013 | Internal | Outside MVP |

**Count:** 20 assets. No real patient or provider identifiers.

---

## 4. Ownership (Phase 4 — unchanged)

| Domain | Data Owner | Business Data Steward | IT / Data Custodian (system class) |
| --- | --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access | Registration / MPI Custodian |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | EMR Application Custodian |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager | Billing / Claims Custodian |
| Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator | Credentialing System Custodian |
| Reference / Organizational Master Data | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | Reference Data Custodian |

Typical classification follows Phase 5 domain guidance. Dataset-level exceptions remain possible; none are invented here.

---

## 5. Quality integration

| CDE ID | Inventory asset | Quality status in this pack |
| --- | --- | --- |
| CDE-001 National ID | META-PAT-004 | CDE — quality rules designed (Phase 7) |
| CDE-002 Patient identifier (MRN) | META-PAT-003 | CDE — quality rules designed (Phase 7) |
| CDE-003 Diagnosis code | META-ENC-007 | CDE — quality rules designed (Phase 7) |
| CDE-004 Encounter documentation timestamp | META-ENC-004 | CDE — quality rules designed (Phase 7) |
| CDE-005 Provider identifier | META-PRV-002 | CDE — quality rules designed (Phase 7) |
| CDE-007 Claim identifier | META-CLM-002 | CDE — quality rules designed (Phase 7) |
| CDE-008 Billed service / charge code | META-CLM-003 | CDE — quality rules designed (Phase 7) |
| CDE-013 Facility / department code | META-FAC-002 | CDE — quality rules designed (Phase 7) |

CDE-006, CDE-009, CDE-010, CDE-011, and CDE-012 remain in the Phase 7 catalogue. They have no row in this working inventory.

No quality **score** is recorded. Scores would come from a monitoring process (Phase 7 design; complementary scorecard project is a separate portfolio repository).

---

## 6. Lineage pointers (conceptual)

| Reference | Coarse path `[A]` |
| --- | --- |
| LIN-REG-PAT-001 | Registration / MPI → Person master → Encounter and billing consumers |
| LIN-ENC-001 | Person master + EMR clinical → Encounter documentation → Claims / quality consumers |
| LIN-CLM-001 | Encounter → Charge capture → Claim submission → External claims interchange (generic; not a named national product) |
| LIN-PRV-001 | Credentialing → Provider master → EMR / encounter |
| LIN-FAC-001 | Org reference → Facility code → Encounter and provider home facility |

Detailed lineage remains Phase 9. These IDs are teaching pointers, not a lineage platform.

---

## 7. What this file does not do

- Does not catalog the whole fictional organization
- Does not add CDEs
- Does not use real personal data
- Does not claim Purview or other catalog ingestion
