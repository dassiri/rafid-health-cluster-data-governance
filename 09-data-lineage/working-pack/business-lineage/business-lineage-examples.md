# Business Lineage Examples (Working Pack)

**Document ID:** RHC-DG-P9-WP-008  
**Version:** 1.0  
**Status:** Implemented (illustrative examples only)  
**Owner:** Domain Data Owners **A** for business meaning in a live process; this file is a teaching artifact  
**Parent design:** [`../../07-business-lineage-example.md`](../../07-business-lineage-example.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

Business lineage shows the **business flow and meaning** of data: process → business data asset → business outcome.

This file records **four** healthcare business-lineage examples `[A]`. Example 4 instantiates the locked Phase 9 KPI example. Names and traces are **not** real Rafid, MOH, or payer metrics.

```text
Business process / question
→ Business data asset
→ Business transformation / process
→ Business target / outcome
```

---

## 2. Example A — Patient Registration → Patient Master

```text
Patient Registration
→ Patient Master
```

| Item | Illustrative value `[A]` |
| --- | --- |
| **Business source** | Patient registration process capturing a registrable person identity |
| **Source asset** | Patient Registration Dataset (META-PAT-002) |
| **Business transformation / process** | Persist / match identity into the cluster person master (conceptual MPI-style match — **not** a matching engine) |
| **Business target** | Patient Master Record (META-PAT-001) |
| **Business purpose** | Create a cluster person identity used by care access, encounter, and billing processes |
| **Data Owner** | Patient Access & Experience Director |
| **Business Data Steward** | Head of Patient Registration & Access |
| **IT / Data Custodian** | Registration / MPI Custodian |
| **Criticality** | Critical (CDE-001, CDE-002, master-data dependency, patient safety candidacy — confirmed Year-1 coverage) |
| **Register** | LIN-001 |
| **Consumer** | Encounter documentation and billing identity use |

---

## 3. Example B — Clinical Encounter → Clinical Reporting

```text
Clinical Encounter
→ Clinical Reporting
```

| Item | Illustrative value `[A]` |
| --- | --- |
| **Business source** | Documented care encounter in the medical record context |
| **Source asset** | Encounter Documentation Dataset (META-ENC-002) / Encounter (META-ENC-001) |
| **Business transformation / process** | Select encounter facts (including Encounter_Date, CDE-004) for an operational clinical summary |
| **Business target** | Illustrative clinical encounter reporting use (consumer — not a new catalog MVP asset) |
| **Business purpose** | Support in-domain clinical operational awareness; not a national quality submission design |
| **Data Owner** | Chief Medical Officer (CMO) |
| **Business Data Steward** | Head of Health Information Management (HIM) |
| **IT / Data Custodian** | EMR Application Custodian |
| **Criticality** | Important (operational process; CDE-004 on the path; not Year-1 Critical Register focus) |
| **Register** | LIN-010 |
| **Consumer** | Clinical domain reporting use (illustrative) |

This example stays inside the **Clinical / Medical Records** MVP domain. It does **not** add Quality & Patient Safety as a Year-1 domain.

---

## 4. Example C — Claims → Financial Reporting

```text
Claims
→ Financial Reporting
```

| Item | Illustrative value `[A]` |
| --- | --- |
| **Business source** | Claim submission / claims extract prepared for reimbursement |
| **Source asset** | Claim Submission Dataset (META-CLM-001) |
| **Business transformation / process** | Conceptual conform of claims facts for financial reporting — **not** a deployed warehouse |
| **Business target** | Illustrative financial / billing reporting consumer |
| **Business purpose** | Support revenue-cycle visibility of submitted claims |
| **Data Owner** | Chief Financial Officer (CFO) |
| **Business Data Steward** | Revenue Cycle Manager |
| **IT / Data Custodian** | Billing / Claims Custodian |
| **Criticality** | Important (downstream reporting; CDE-007 on the path) |
| **Register** | LIN-012 |
| **Consumer** | Financial / billing reporting (illustrative) |

Classification of any reporting extract remains **Owner-assessed** under Phase 5. Lineage only surfaces the reassessment question.

---

## 5. Example D — Patient Claim Rejection Rate (locked KPI example)

```text
Business KPI
→ Business Definition
→ Data Elements
→ Data Assets
→ Source Systems
→ Transformation
→ Consumer
```

| Step | Illustrative content `[A]` |
| --- | --- |
| **Business KPI** | Patient Claim Rejection Rate — proportion of submitted claims returned or rejected in a reporting period (**not** a measured rate) |
| **Business definition** | Owner-accepted meaning of “claim,” “rejection,” and the in-scope population (Financial domain **A** = CFO) |
| **Data elements** | Claim identifier (CDE-007); billed service / charge code (CDE-008); diagnosis code as billing input (CDE-003 consumed); Patient identifier on the claim (CDE-002 consumed) |
| **Data assets** | META-CLM-001; META-ENC-002; META-PAT-001 |
| **Source systems** | Billing / claims (SYN-BILL, primary context); EMR clinical (SYN-EHR, contributing); Registration / MPI (SYN-REG, identity context) — not exactly one source system |
| **Transformation** | Encounter coding → charge capture → claim composition → rejection flag from interchange response (**not** ETL code) |
| **Consumer** | Revenue-cycle Domain Huddle / DMC **summary** theme — not a published open-data statistic |
| **Data Owner** | CFO (KPI / claim extract meaning). CMO remains **A** for diagnosis meaning. Patient Access & Experience Director remains **A** for person identity |
| **Business Data Steward** | Revenue Cycle Manager (financial hop); HIM and Registration stewards remain **R** on their assets |
| **Criticality** | Critical (executive reporting, financial impact, CDE path, external sharing candidacy — confirmed Year-1 coverage) |
| **Register** | LIN-005 (with supporting hops LIN-003, LIN-004, LIN-008, LIN-009) |

No numeric target is given. This is **not** a Phase 12 KPI pack.

---

## 6. Business meaning vs catalog metadata

| Catalog field (Phase 8) | How business lineage uses it |
| --- | --- |
| Business Definition | Owner-accepted meaning of the source and target assets |
| Data Owner / Business Data Steward | Accountability for business lineage correctness / maintenance |
| Lineage Reference | Pointer from the catalog page to `LIN-*` |
| CDE Status | Explains why the hop was a lineage **candidate** |

Glossary terms reused unchanged: Patient, Encounter, Diagnosis, Claim ([`../../../08-metadata-catalog/working-pack/business-glossary/business-glossary.md`](../../../08-metadata-catalog/working-pack/business-glossary/business-glossary.md)).

---

## 7. What this file does not do

- Does not add a second business-lineage method
- Does not publish a live KPI
- Does not claim NDMO or payer reporting compliance
- Does not merge Owner business **A** and PDPO privacy **A**
