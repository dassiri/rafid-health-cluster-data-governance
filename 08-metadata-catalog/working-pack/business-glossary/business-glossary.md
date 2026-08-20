# Business Glossary (Working Pack)

**Document ID:** RHC-DG-P8-WP-007  
**Version:** 1.0  
**Status:** Implemented (illustrative glossary only)  
**Owner:** Domain Data Owner **A** for terms in that domain; DMO owns glossary method `[B]`  
**Parent design:** [`../../05-business-glossary.md`](../../05-business-glossary.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This working glossary records **25 business terms** for Rafid `[A]`.

It **extends** the Phase 8 structure (seven locked illustrative terms) and the 15-term recruiter sample. It does **not** replace either file. Definitions that already exist in Phase 8 are reused unchanged.

This is **not** a live Rafid vocabulary, **not** SNOMED/ICD, and **not** an official national healthcare terminology standard.

Machine-readable list: [`business-glossary.csv`](business-glossary.csv)

```text
Business Glossary  ↔  Data Catalog  ↔  Data Assets
```

---

## 2. Term structure (unchanged)

| Field | Intent |
| --- | --- |
| Term | Preferred cluster term |
| Business Definition | Owner-accepted meaning in business language |
| Domain | Phase 4 domain, or Enterprise Data Governance (method) for governance terms |
| Data Owner | Phase 4 title, or CDO for method terms |
| Business Data Steward | Phase 4 appointed title |
| Related Data Assets | Working-pack Asset IDs |
| Status | Draft / Approved / Retired (glossary status — not catalog certification) |
| Notes | CDE link, watch-item, or scope note |

---

## 3. Terms (25)

Status for every row: **Approved (illustrative)** — not a live Owner signature.

### Patient / Person Master Data

| Term | Business Definition | Data Owner | Business Data Steward | Related Data Assets | Notes |
| --- | --- | --- | --- | --- | --- |
| Patient | A person registered to receive care in the cluster, identified in the person master. | Patient Access & Experience Director | Head of Patient Registration & Access | META-PAT-001, META-PAT-002 | Phase 8 term. Context for CDE-001 / CDE-002 |
| Patient ID | The cluster patient identifier (MRN) used to locate the person in operational systems. | Patient Access & Experience Director | Head of Patient Registration & Access | META-PAT-003 | **CDE-002** |
| National ID | The national identity number captured at registration where required. | Patient Access & Experience Director | Head of Patient Registration & Access | META-PAT-004 | **CDE-001** |
| Date of Birth | The recorded date of birth used to confirm identity and derive age. | Patient Access & Experience Director | Head of Patient Registration & Access | META-PAT-005 | Watch-item — **not** a 14th CDE |
| Gender | The administrative gender recorded at registration, using the approved value set. | Patient Access & Experience Director | Head of Patient Registration & Access | META-PAT-006 | Not a catalogue CDE |

### Provider / Clinician Data

| Term | Business Definition | Data Owner | Business Data Steward | Related Data Assets | Notes |
| --- | --- | --- | --- | --- | --- |
| Provider | A clinician or practitioner identity used for care delivery and credentialing, distinct from the HR employee record. | Medical Affairs Officer | Credentialing Coordinator | META-PRV-001 | Phase 8 term. Outside catalog MVP |
| Provider Identifier | The unique identifier of the practitioner in the credentialing master. | Medical Affairs Officer | Credentialing Coordinator | META-PRV-002 | **CDE-005**. Outside catalog MVP |

### Reference / Organizational Master Data

| Term | Business Definition | Data Owner | Business Data Steward | Related Data Assets | Notes |
| --- | --- | --- | --- | --- | --- |
| Facility | An organizational location in the cluster reference structure (hospital or other delivery site as used in org master). | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | META-FAC-001 | Phase 8 term. Outside catalog MVP. DMO hosts the Steward; DMO is not Owner |
| Department | An organizational unit within a facility (or cluster structure) as represented in organizational reference data. | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | META-FAC-001 | Phase 8 term. Outside catalog MVP |
| Facility / Department Code | The reference code that identifies a facility or department in organizational master data. | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | META-FAC-002 | **CDE-013**. Outside catalog MVP |

### Clinical / Medical Records Data

| Term | Business Definition | Data Owner | Business Data Steward | Related Data Assets | Notes |
| --- | --- | --- | --- | --- | --- |
| Encounter | A defined care interaction or visit recorded in the clinical record context. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-001, META-ENC-002 | Phase 8 term. Context for CDE-004 |
| Encounter ID | The unique identifier of a recorded care encounter. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-003 | Not a catalogue CDE |
| Encounter Date | The date (and, where used, time) associated with encounter documentation. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-004 | Maps to **CDE-004** Encounter documentation timestamp |
| Admission | The recorded start of an inpatient (or equivalent) stay, where used. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-005 | Phase 8 sample term. Not a new CDE |
| Admission Date | The date the inpatient (or equivalent) stay is recorded as started. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-005 | Watch-item — **not** a 14th CDE |
| Discharge | The recorded end of an inpatient (or equivalent) stay, where used. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-006 | Phase 8 sample term. Not a new CDE |
| Discharge Date | The date the inpatient (or equivalent) stay is recorded as ended. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-006 | Watch-item — **not** a 14th CDE |
| Diagnosis | A recorded clinical diagnosis (coded or structured) in the medical record context. | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | META-ENC-007 | Phase 8 term. **CDE-003** |

### Financial / Billing & Claims Data

| Term | Business Definition | Data Owner | Business Data Steward | Related Data Assets | Notes |
| --- | --- | --- | --- | --- | --- |
| Claim | A billing/claims record submitted or prepared for reimbursement of services. | Chief Financial Officer (CFO) | Revenue Cycle Manager | META-CLM-001 | Phase 8 term. Context for CDE-007 |
| Claim Identifier | The unique identifier of a claim record in the governed claims population. | Chief Financial Officer (CFO) | Revenue Cycle Manager | META-CLM-002 | **CDE-007** |
| Charge Code | A billed service / charge code used in the revenue cycle. | Chief Financial Officer (CFO) | Revenue Cycle Manager | META-CLM-003 | **CDE-008** |

### Enterprise Data Governance (method)

These four terms are **method vocabulary**. They are not a ninth data domain. CDO / DMO owns the method; they are not Data Owner of Patient, Clinical, or Finance data.

| Term | Business Definition | Data Owner (method) | Steward (method) | Related Data Assets | Notes |
| --- | --- | --- | --- | --- | --- |
| Critical Data Element | A data element whose quality has a material effect on identity, care operations, eligibility, safety, or executive reporting, confirmed through the Phase 7 two-step method. | CDO (catalogue method) | Data Governance Officer | META-PAT-003, META-PAT-004, META-ENC-004, META-ENC-007, META-CLM-002, META-CLM-003 | Exactly **13** catalogue CDEs. This term does not add CDEs |
| Data Asset | A governed unit registered in the catalog (Dataset, Table, Report, Dashboard, or Master Data Entity). | CDO (catalog method) | Data Governance Officer | META-PAT-001, META-ENC-001, META-CLM-001 | See Phase 8 asset model |
| Metadata | Governed information about a data asset: meaning, ownership, classification, source, and trust of the **description**. Not the underlying data. | CDO (catalog method) | Data Governance Officer | — | Publishing metadata is not a data release |
| Data Classification | The Rafid working label applied to a dataset (Public / Internal / Confidential / Restricted) using the Phase 5 method. | CDO (method); Data Owner **A** for the value | Domain Business Data Steward | All inventory assets | **Not** NDMO national tiers |

---

## 4. Terms held in the Phase 8 sample and not repeated here

Appointment and Golden Record remain in [`../../../assets/practical-evidence/03-business-glossary-sample.md`](../../../assets/practical-evidence/03-business-glossary-sample.md). They are not removed. They are omitted here so this working set stays focused on inventory assets.

---

## 5. What this file does not do

- Does not add CDEs
- Does not claim SNOMED, ICD, or national terminology authority
- Does not replace Phase 8 [`../../05-business-glossary.md`](../../05-business-glossary.md)
