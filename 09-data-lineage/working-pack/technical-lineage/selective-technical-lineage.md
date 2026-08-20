# Selective Technical / Field-Level Lineage (Working Pack)

**Document ID:** RHC-DG-P9-WP-010  
**Version:** 1.0  
**Status:** Implemented (illustrative field hops only — not a scanner)  
**Owner:** IT / Data Custodian **R** for technical facts; domain Data Owner **A** for business meaning of the elements  
**Parent design:** [`../../04-granularity-model.md`](../../04-granularity-model.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

**Synthetic / Illustrative / Non-production.**

These examples are **described**, not scanned. They do **not** claim automated technical lineage, a production ETL system, Microsoft Purview column lineage, or enterprise-wide field coverage.

---

## 1. Purpose and limit

Year-1 technical lineage is a **description pattern**. Level 4 is **selective only**, and only when a CDE or a specific reporting count warrants it.

This file records **four** field-level examples `[A]`. Schema and table names are copied from the Phase 8 inventory as teaching locations. They are not a live database.

Illustrative locations already recorded in the catalog working pack:

| Catalog ID | Element | Illustrative location |
| --- | --- | --- |
| META-PAT-003 | Patient_ID (CDE-002) | `mpi.patient.patient_master.patient_id` |
| META-PAT-004 | National_ID (CDE-001) | `mpi.patient.patient_master` (national identifier column) |
| META-ENC-007 | Diagnosis_Code (CDE-003) | `emr.clinical.encounter_documentation.diagnosis_code` |
| META-ENC-003 | Encounter_ID | `emr.clinical.encounter_documentation.encounter_id` |
| META-ENC-004 | Encounter_Date (CDE-004) | `emr.clinical.encounter_documentation.encounter_date` |
| META-CLM-002 | Claim_ID (CDE-007) | `bill.claims.claim_submission.claim_id` |

---

## 2. Example 1 — Patient_ID (CDE-002)

```text
SYN-REG / mpi.patient.patient_master.patient_id
        ↓  persist identity (conceptual)
Patient Master Patient_ID (META-PAT-003)
        ↓  identity used on encounter
emr.clinical.encounter_documentation.patient_id
```

| Field | Value `[A]` |
| --- | --- |
| **Source field** | Patient Registration Dataset / `patient_id` (META-PAT-003 context) |
| **Transformation / relationship** | Identity persist; same person key reused on encounter documentation — **not** a scanned job |
| **Target field** | Encounter documentation `patient_id` (consumed; person meaning remains Patient domain) |
| **Business meaning** | Cluster patient identifier (MRN) used to locate the person in operational systems |
| **Criticality** | Critical |
| **Data Owner** | Patient Access & Experience Director (identity meaning). CMO consumes the key on the encounter asset |
| **Business Data Steward** | Head of Patient Registration & Access |
| **IT / Data Custodian** | Registration / MPI Custodian **C**; EMR Application Custodian **C** on the encounter table |
| **Validation status** | Published (illustrative) |
| **Register** | LIN-006 (master persist); identity on encounter also supports LIN-002 |

Related hop: person master consumed on claims is LIN-011 (asset-level, Important).

---

## 3. Example 2 — National_ID (CDE-001)

```text
SYN-REG registration capture of National_ID
        ↓  persist identity (conceptual)
Patient Master National_ID (META-PAT-004)
```

| Field | Value `[A]` |
| --- | --- |
| **Source field** | Patient Registration Dataset / National_ID |
| **Transformation / relationship** | Persist the national identifier on the person master — described, not scanned |
| **Target field** | Patient (META-PAT-001) / National_ID (META-PAT-004) |
| **Business meaning** | National identifier used in identity uniqueness and completeness controls (DQ-001, DQ-003) |
| **Criticality** | Critical |
| **Data Owner** | Patient Access & Experience Director |
| **Business Data Steward** | Head of Patient Registration & Access |
| **Validation status** | Published (illustrative) |
| **Register** | LIN-007 |

This hop does **not** document National_ID on the claims extract as enterprise field lineage. Downstream presence of identity elements is a **classification reassessment prompt** (Phase 5), not automatic field mapping.

---

## 4. Example 3 — Diagnosis_Code (CDE-003) to claims

```text
emr.clinical.encounter_documentation.diagnosis_code
        ↓  consumed as billing input (conceptual)
bill.claims.claim_submission (diagnosis as billing input)
```

| Field | Value `[A]` |
| --- | --- |
| **Source field** | Diagnosis_Code (META-ENC-007 / CDE-003) |
| **Transformation / relationship** | Clinical diagnosis code reused as billing input — **not** a mapping engine and **not** an ICD product claim |
| **Target field** | Diagnosis code as billing input on Claim Submission Dataset |
| **Business meaning** | Structured diagnosis that can affect claim acceptance if invalid (DQ-002) |
| **Criticality** | Critical |
| **Data Owner** | CFO for the **claim asset**. CMO remains **A** for clinical diagnosis meaning |
| **Business Data Steward** | Revenue Cycle Manager (claim hop); HIM remains **R** for the source element |
| **Validation status** | Published (illustrative) |
| **Register** | LIN-008 |

---

## 5. Example 4 — Claim_ID (CDE-007) to Claim_Count

```text
bill.claims.claim_submission.claim_id
        ↓  illustrative aggregation
Financial reporting Claim_Count
```

**Illustrative transformation (not deployed ETL):**

```text
Claim_Count = COUNT(DISTINCT Claim_ID)
```

| Field | Value `[A]` |
| --- | --- |
| **Source field** | Claim_ID (META-CLM-002 / CDE-007) |
| **Transformation / relationship** | Distinct count of claim identifiers for an illustrative financial / rejection-rate denominator context |
| **Target field** | Derived `Claim_Count` on an illustrative reporting consumer — **not** a new CDE |
| **Business meaning** | Count of distinct claims in the governed claims population used by the illustrative KPI story |
| **Criticality** | Important (CDE-007 + reporting candidacy; Level 4 kept selective vs Critical Register field hops) |
| **Data Owner** | Chief Financial Officer (CFO) |
| **Business Data Steward** | Revenue Cycle Manager |
| **Validation status** | Published (illustrative) |
| **Register** | LIN-009 |

`Claim_Count` is a **derived reporting expression**. It is not added to the 13-CDE catalogue.

A Standard (Priority 3) companion hop, LIN-013, carries Encounter_ID onto the claim as an operational link. Encounter_ID is **not** a catalogue CDE.

---

## 6. When Level 4 is warranted (locked rule, applied)

Field-level lineage may be warranted for:

- CDE-related root-cause analysis (Phase 7)
- Classification reassessment prompts (Phase 5 method — lineage only surfaces the question)
- Specific audit / investigation needs

Warrant does **not** auto-expand to all fields in the domain. Charge_Code (CDE-008 / META-CLM-003) remains a confirmed CDE; this pack does **not** add a fifth Level 4 example for it, so selectivity stays visible. Asset-level hop LIN-003 already carries CDE-008 as context.

---

## 7. What this file does not do

- Does not claim automated technical lineage
- Does not claim a production lineage engine or ETL deployment
- Does not create fake Microsoft Purview / Collibra screenshots
- Does not implement enterprise-wide column-level lineage
- Does not add CDEs
