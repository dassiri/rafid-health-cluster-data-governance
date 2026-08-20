# Lineage MVP Scope (Working Pack)

**Document ID:** RHC-DG-P9-WP-005  
**Version:** 1.0  
**Status:** Implemented (MVP design only — not a live lineage graph)  
**Owner:** CDO / DMO (programme) `[B]`; domain Data Owners **A** for MVP content  
**Parent design:** [`../../16-lineage-mvp.md`](../../16-lineage-mvp.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

The lineage MVP is a **scope cut**, not a platform implementation.

It respects the approved Phase 8 catalog MVP. It does **not** add domains. It does **not** attempt enterprise-wide lineage. Success is **qualitative**. Numeric coverage targets are not invented.

---

## 2. Priority domains (locked — same as Phase 8 and Phase 9)

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Financial / Billing & Claims Data  

| Domain | Data Owner | Business Data Steward |
| --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager |

**Outside MVP operating scope:** Provider / Clinician; Reference / Organizational Master (Facility); HR / Workforce; Supply Chain & Asset; Quality & Patient Safety.

Coarse catalog pointers `LIN-PRV-001` and `LIN-FAC-001` already exist in the Phase 8 inventory. They are **not** expanded in this Year-1 register.

---

## 3. Locked initial use cases (unchanged)

1. Patient Registration → Clinical → Billing/Claims lineage (the single E2E example, including generic external interchange as consumer)  
2. Patient Claim Rejection Rate business lineage  

This pack instantiates those two use cases. It does not add a third Year-1 use case.

---

## 4. Locked initial assets (unchanged)

| Phase 9 name | Catalog ID |
| --- | --- |
| Patient Master Record | META-PAT-001 |
| Encounter / Diagnosis record | META-ENC-001 / META-ENC-002 |
| Claims Extract | META-CLM-001 |

Supporting catalog rows (Patient Registration Dataset, selected CDE elements) are used as **sources/targets** on hops. They do not expand the catalog MVP domain list.

---

## 5. Working priority cut `[A][B]`

| Priority | Meaning | Register rows |
| --- | --- | --- |
| **Priority 1** | Critical assets / CDE-related lineage. Critical Lineage Register focus. | LIN-001 to LIN-008 |
| **Priority 2** | Major downstream reporting lineage and important operational hops. | LIN-009 to LIN-012 |
| **Priority 3** | Additional operational lineage, maintained where useful. | LIN-013 |

Year-1 **focus** remains the **Critical Lineage Register** (Priority 1), consistent with Phase 9.

---

## 6. Granularity in the MVP

| Level | MVP treatment |
| --- | --- |
| Level 1 Business | Both locked use cases |
| Level 2 Dataset / Asset | Three MVP assets plus the registration dataset as originating source |
| Level 3 Structure / Object | Named only where the Phase 8 inventory already records a table (`patient_master`, `encounter_documentation`, `claim_submission`) |
| Level 4 Data Element / Field | Selective: Patient_ID, National_ID, Diagnosis_Code, Claim_ID, Charge_Code, Encounter_Date, Encounter_ID |

Field-level rows are teaching records. They are **not** enterprise column-level lineage.

---

## 7. Qualitative success (unchanged from Phase 9)

- The two use cases can be described at Levels 1–2  
- Lineage Metadata fields are populated or explicitly gapped  
- Owners of the three domains can validate business meaning  
- Classification reassessment questions can be asked without auto-tiering  
- No lineage product is required to declare the MVP **design** complete  

---

## 8. What this file does not do

- Does not add Provider or Facility to Year-1 operating scope  
- Does not add CDEs  
- Does not set numeric lineage coverage targets  
- Does not implement a lineage tool
