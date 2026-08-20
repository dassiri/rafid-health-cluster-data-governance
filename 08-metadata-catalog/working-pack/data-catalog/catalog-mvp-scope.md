# Catalog MVP Scope (Working Pack)

**Document ID:** RHC-DG-P8-WP-011  
**Version:** 1.0  
**Status:** Implemented (MVP design only — not a live catalog)  
**Owner:** CDO / DMO (programme) `[B]`; domain Data Owners **A** for MVP content  
**Parent design:** [`../../14-catalog-mvp.md`](../../14-catalog-mvp.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

---

## 1. Purpose

The MVP is a **scope cut**, not a platform implementation.

It does **not** attempt to catalog the entire fictional organization. Success is **qualitative**. Numeric coverage targets are not invented.

---

## 2. Priority domains (locked — same as Phase 8)

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Financial / Billing & Claims Data  

| Domain | Data Owner | Business Data Steward |
| --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager |

**Outside MVP operating scope:** Provider / Clinician; Reference / Organizational Master (Facility); HR / Workforce; Supply Chain & Asset; Quality & Patient Safety.

Those domains remain in the Phase 8 framework. Provider and Facility appear in the working **inventory** because Encounter depends on them. They are not Year-1 published catalog operating coverage.

---

## 3. Priority data assets (working pack)

| Asset ID | Asset Name | Type |
| --- | --- | --- |
| META-PAT-001 | Patient | Master Data Entity |
| META-PAT-002 | Patient Registration Dataset | Dataset |
| META-PAT-003 | Patient_ID | Data Element (CDE-002) |
| META-PAT-004 | National_ID | Data Element (CDE-001) |
| META-PAT-005 | Date_of_Birth | Data Element (watch-item) |
| META-ENC-001 | Encounter | Master Data Entity |
| META-ENC-002 | Encounter Documentation Dataset | Dataset |
| META-ENC-004 | Encounter_Date | Data Element (CDE-004) |
| META-ENC-007 | Diagnosis_Code | Data Element (CDE-003) |
| META-CLM-001 | Claim Submission Dataset | Dataset |
| META-CLM-002 | Claim_ID | Data Element (CDE-007) |
| META-CLM-003 | Charge_Code | Data Element (CDE-008) |

Gender, Encounter_ID, Admission_Date, and Discharge_Date are in the inventory and may be described. They are **not** extra CDEs and are not required to declare the MVP **design** complete.

Asset types required in the Phase 8 MVP cut: **Dataset** and **Master Data Entity**. Data Element rows in this pack are teaching records for CDEs and watch-items.

---

## 4. Required metadata (MVP)

MVP uses the **full** Required set. It is not a reduced schema.

| Group | Fields |
| --- | --- |
| Required | Asset ID; Asset Name; Business Domain; Business Definition; Business Owner; Business Data Steward; Source System; Classification; Lifecycle Status; Approval Status |
| Conditional on type | Source Dataset; Table; Column; Data Type; CDE Status (elements) |
| Conditional on capability | Data Quality Status (CDEs / parents that contain CDEs); Lineage Reference (Dataset and Master Data Entity); Refresh Frequency when known |
| Optional | Asset Type (filled here); Criticality; Business Rules; Last Reviewed; Related Business Terms; Database / Schema |

---

## 5. Required ownership

Every published MVP asset has:

- Phase 4 Data Owner title  
- Phase 4 Business Data Steward title  
- IT / Data Custodian as technical contact class (not Owner)

---

## 6. Required classification

Every published MVP asset has a Rafid tier. Typical MVP values in this pack:

| Domain | Typical tier `[A][B]` |
| --- | --- |
| Patient / Person Master Data | Restricted |
| Clinical / Medical Records Data | Restricted |
| Financial / Billing & Claims (patient-linked claims) | Restricted |

Unlabeled is not Public.

---

## 7. Required glossary coverage

MVP glossary coverage in this pack:

| Domain | Terms that must exist |
| --- | --- |
| Patient / Person Master Data | Patient; Patient ID; National ID |
| Clinical / Medical Records Data | Encounter; Encounter Date; Diagnosis |
| Financial / Billing & Claims Data | Claim; Claim Identifier; Charge Code |

Additional related terms (Date of Birth, Admission, Discharge) may be present. They do not expand the CDE catalogue.

---

## 8. Required lineage reference

MVP Dataset and Master Data Entity rows carry a coarse pointer:

| Asset | Lineage Reference |
| --- | --- |
| Patient / Patient Registration Dataset | LIN-REG-PAT-001 |
| Encounter / Encounter Documentation Dataset | LIN-ENC-001 |
| Claim Submission Dataset | LIN-CLM-001 |

Pointers are conceptual. They are not automated lineage.

---

## 9. Quality information

| When | What the MVP record shows |
| --- | --- |
| Confirmed CDE | CDE — quality rules designed (Phase 7) |
| Watch-item | Watch-item — not in the 13-CDE catalogue |
| No Phase 7 link | Not applicable — do not invent a score |

Issue status is recorded only when a Phase 6/7 issue exists. This pack does not log fake tickets.

---

## 10. MVP users

- Data Owners  
- Business Data Stewards  
- DMO  

---

## 11. MVP completion checklist

Use one row per published MVP asset.

| Check | Done? |
| --- | --- |
| Domain identified (one of the three MVP domains) | ☐ |
| Owner assigned (Phase 4 title) | ☐ |
| Steward assigned (Phase 4 title) | ☐ |
| Minimum metadata completed (Required fields) | ☐ |
| Classification assigned (Rafid tier; unlabeled is not Public) | ☐ |
| CDE status identified (elements) / contained CDEs noted (datasets) | ☐ |
| Business definition approved (Data Owner) | ☐ |
| Quality status available (or explicitly capability-gap) | ☐ |
| Lineage reference available (Dataset / Master Data Entity) | ☐ |
| Glossary term linked | ☐ |
| DMO governance check completed | ☐ |
| Catalog approval completed | ☐ |
| Published (Lifecycle Status = Active) | ☐ |

**Design-complete (this repository):** the checklist is demonstrated on the eight sample pages in [`../examples/sample-catalog-assets.md`](../examples/sample-catalog-assets.md). Live Rafid completion is **not** claimed.

---

## 12. Qualitative success (unchanged from Phase 8)

- MVP-scope operational assets can be identified and registered  
- Mandatory metadata is present before publish  
- Classification is linked  
- Owner and Steward are visible  
- DMO can check completeness without rewriting meaning  
- MVP users can discover **metadata**, not Restricted **data**  
- No catalog product is required to declare the MVP **design** complete  

---

## 13. What this file does not do

- Does not add Provider or Facility to Year-1 operating scope  
- Does not set “80% of datasets catalogued” or similar targets  
- Does not implement a catalog tool
