# Business Glossary Sample `[A]`

**Label:** `[A]` Fictional / illustrative Rafid assumption  
**Does not claim:** A live Rafid vocabulary or NDMO-mandated glossary

---

## Purpose

Fifteen terms using the **Phase 8 glossary structure**. Seven terms already exist in [`08-metadata-catalog/05-business-glossary.md`](../../08-metadata-catalog/05-business-glossary.md). This sample **repeats those seven** and adds eight related terms so a recruiter can see a slightly larger working set in one place.

This file does **not** replace Phase 8 and does **not** add CDEs.

```text
Business Glossary  ↔  Metadata / Catalog  ↔  Data Assets
```

Steward: **Business Data Steward**. Owner titles: Phase 4 only.

---

## Terms (15)

| Term | Business Definition | Domain | Owner | Steward | CDE? | Related asset (sample) |
| --- | --- | --- | --- | --- | --- | --- |
| Patient | A person registered to receive care in the cluster, identified in the person master. | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Context for CDE-001 / CDE-002 | CAT-A02 |
| Patient ID | The cluster patient identifier (MRN) used to locate the person in operational systems. | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | **CDE-002** | CAT-A01 |
| National ID | The national identity number captured at registration where required. | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | **CDE-001** | CAT-A01 |
| Provider | A clinician or practitioner identity used for care delivery and credentialing, distinct from the HR employee record. | Provider / Clinician Data | Medical Affairs Officer | Business Data Steward | Context for CDE-005 | — (outside catalog MVP) |
| Facility | An organizational location in the cluster reference structure. | Reference / Organizational Master Data | Strategy & Planning Director | Business Data Steward | Context for CDE-013 | Supporting MDM only |
| Encounter | A defined care interaction or visit recorded in the clinical record context. | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | Context for CDE-004 | CAT-A04 |
| Appointment | A scheduled care slot; not the same as a completed encounter. | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | No (not an extra CDE) | — |
| Admission | The recorded start of an inpatient (or equivalent) stay, where used. | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | No | CAT-A04 |
| Discharge | The recorded end of an inpatient (or equivalent) stay, where used. | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | No | CAT-A04 |
| Diagnosis | A recorded clinical diagnosis (coded or structured) in the medical record context. | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | **CDE-003** | CAT-A05 |
| Claim | A billing/claims record submitted or prepared for reimbursement of services. | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | Context for CDE-007 | CAT-A07 |
| Claim Identifier | The unique identifier of a claim record in the governed claims population. | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | **CDE-007** | CAT-A07 |
| Department | An organizational unit within a facility (or cluster structure) as represented in organizational reference data. | Reference / Organizational Master Data | Strategy & Planning Director | Business Data Steward | Context for CDE-013 | — |
| Charge Code | A billed service / charge code used in the revenue cycle. | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | **CDE-008** | CAT-A08 |
| Golden Record | The logical, Owner-accepted trusted master representation of a person (or other master) — not a required physical database. | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Uses CDE-001 / CDE-002 | CAT-A02 |

Glossary status for all rows: **Approved (illustrative)** — not a live Owner signature.

Appointment / Admission / Discharge are **not** new CDEs. Domain quality watch-items remain outside the locked 13-CDE catalogue.
