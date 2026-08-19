# Data Quality Rules (Representative Library)

**Document ID:** RHC-DG-P7-005  
**Version:** 1.0  
**Status:** Implemented (illustrative rules only)  
**Owner:** Domain Data Owner **A** for each rule’s CDE; DMO owns the rule-library method `[B]`  
**Approver:** CDO `[B]` (library as framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Representative library; DQ-001 and DQ-002 included; not a large catalogue.

**Phase:** 7 — Data quality  
**Does not decide:** Hundreds of production rules; tool implementation; NDMO-mandated rule text `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records a **representative** quality-rule library for the fictional Rafid Health Cluster `[A]`.

It demonstrates the approved rule structure and a **small** set of examples. It is **not** a complete production rule book. All examples are illustrative `[A]`.

Phase 4 remains unchanged: Data Owner is **A** for data quality rules; Steward is **R**; Custodian is consulted on measurement method.

---

## 2. Approved rule structure (locked)

Each rule records:

| Field | Intent |
| --- | --- |
| Rule ID | Stable Rafid identifier `[A]` (not an NDMO control ID) |
| CDE | Field from the 13-CDE catalogue |
| Dimension | One of the seven Rafid dimensions |
| Business rule | What “good” means in business language |
| Measurement method | How conformance is observed (conceptual) |
| Expected outcome | Pass condition |
| Threshold | Target / Warning / Breach pointer (see [`06-thresholds.md`](06-thresholds.md)) |
| Severity | Default issue severity if the rule is breached `[A][B]` |
| Owner | Phase 4 Data Owner title |
| Steward | Phase 4 Business Data Steward title |
| Source/system | Typical system class `[A]` |
| Frequency | Conceptual cadence — **no numeric SLA** `[B]` |
| Exception handling | Link to issue path and/or governance exception |

---

## 3. How many rules

Keep the library **small on purpose** `[B]`. Dedicated CDE governance does **not** mean a rule for every possible defect. Additional production rules are confirmed later by the Owner/Steward using this structure; they are **not** added in this drop.

---

## 4. Illustrative rules `[A]`

Numeric threshold values used below are **`[A] Illustrative Rafid target`**. They are not NDMO requirements, not regulatory requirements, and not real Rafid performance.

### DQ-001 — National ID uniqueness

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-001 |
| **CDE** | CDE-001 National ID |
| **Dimension** | Uniqueness (CDE-dependent; confirmed material for this CDE) |
| **Business rule** | An in-scope, non-blank National ID value must identify one person in the governed patient/person population. |
| **Measurement method** | Count in-scope records sharing the same National ID where identity is not an approved linked-record exception. |
| **Expected outcome** | Duplicate National ID groups = 0 except documented exceptions. |
| **Threshold** | Target / Warning / Breach as in the thresholds file for uniqueness-style rules — **`[A] Illustrative Rafid target`** |
| **Severity** | Critical |
| **Owner** | Patient Access & Experience Director |
| **Steward** | Head of Patient Registration & Access |
| **Source/system** | EMR / MPI / registration |
| **Frequency** | Steward operational monitoring; Domain Huddle review (Phase 3 cadence — no numeric SLA) |
| **Exception handling** | Log via Data Quality Issue Management Procedure. Do not silently merge identities. Phase 10 matching is **not** designed here. Governance exceptions (out of policy) use the Data Governance Exception Procedure; DMC **A**. |

### DQ-002 — Diagnosis code validity

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-002 |
| **CDE** | CDE-003 Diagnosis code |
| **Dimension** | Validity (baseline) |
| **Business rule** | A recorded diagnosis code must exist on the cluster-approved diagnosis code list in force for that encounter context. |
| **Measurement method** | Compare recorded codes to the approved reference list (integrity of the list itself is CDE-013 / reference governance, not a second Owner here). |
| **Expected outcome** | Invalid (not-on-list) codes = 0 for in-scope coded encounters, except documented exceptions. |
| **Threshold** | Validity-style illustrative thresholds — **`[A] Illustrative Rafid target`** |
| **Severity** | High |
| **Owner** | Chief Medical Officer (CMO) |
| **Steward** | Head of Health Information Management (HIM) |
| **Source/system** | EMR clinical |
| **Frequency** | Steward operational monitoring; Domain Huddle review (no numeric SLA) |
| **Exception handling** | Issue procedure. Clinical meaning is not “fixed” by IT without Owner/Steward. |

### DQ-003 — National ID completeness

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-003 |
| **CDE** | CDE-001 National ID |
| **Dimension** | Completeness (baseline) |
| **Business rule** | In-scope registered patients must have a National ID value captured, except an Owner-approved reason code (for example eligible exception population). |
| **Measurement method** | Percent of in-scope records with non-blank National ID, or with a valid documented exception reason. |
| **Expected outcome** | Completeness meets the illustrative completeness thresholds. |
| **Threshold** | Completeness-style — **`[A] Illustrative Rafid target`** |
| **Severity** | High |
| **Owner** | Patient Access & Experience Director |
| **Steward** | Head of Patient Registration & Access |
| **Source/system** | EMR / MPI / registration |
| **Frequency** | Steward operational monitoring (no numeric SLA) |
| **Exception handling** | Issue procedure; residual completeness risk is Owner **A** to accept. |

### DQ-004 — Credential expiry monitoring

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-004 |
| **CDE** | CDE-006 Credential expiry date |
| **Dimension** | Timeliness (CDE-dependent; confirmed material) |
| **Business rule** | Active privileged practice must not continue on an undetected expired credential in the governed provider population. |
| **Measurement method** | Count active providers whose expiry date is in the past and whose status is not recorded as suspended/expired. |
| **Expected outcome** | Undetected expiry count = 0 except documented exceptions. |
| **Threshold** | Timeliness-style — **`[A] Illustrative Rafid target`** |
| **Severity** | Critical |
| **Owner** | Medical Affairs Officer |
| **Steward** | Credentialing Coordinator |
| **Source/system** | Credentialing system |
| **Frequency** | Steward operational monitoring (no numeric SLA) |
| **Exception handling** | Issue procedure. Patient-safety ageing uses Phase 3 qualitative escalation — still no numeric SLA. |

### DQ-005 — Claim identifier uniqueness

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-005 |
| **CDE** | CDE-007 Claim identifier |
| **Dimension** | Uniqueness |
| **Business rule** | A claim identifier must not be reused for a different claim in the governed claims population. |
| **Measurement method** | Duplicate claim-ID groups. |
| **Expected outcome** | Duplicate groups = 0 except documented resubmission/exception records. |
| **Threshold** | Uniqueness-style — **`[A] Illustrative Rafid target`** |
| **Severity** | High |
| **Owner** | Chief Financial Officer (CFO) |
| **Steward** | Revenue Cycle Manager |
| **Source/system** | Billing / claims |
| **Frequency** | Steward operational monitoring (no numeric SLA) |
| **Exception handling** | Issue procedure. |

### DQ-006 — Charge code completeness

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-006 |
| **CDE** | CDE-008 Billed service / charge code |
| **Dimension** | Completeness (baseline) |
| **Business rule** | In-scope billable encounters must have charge/service coding captured, except Owner-approved delay/exception. |
| **Measurement method** | Percent of in-scope encounters with a charge/service code present. |
| **Expected outcome** | Completeness meets illustrative completeness thresholds. |
| **Threshold** | Completeness-style — **`[A] Illustrative Rafid target`** |
| **Severity** | High |
| **Owner** | Chief Financial Officer (CFO) |
| **Steward** | Revenue Cycle Manager |
| **Source/system** | Billing / HIS financial |
| **Frequency** | Steward operational monitoring (no numeric SLA) |
| **Exception handling** | Issue procedure. Clinical documentation defects that **cause** missing charges may be **cross-domain**; DMO routes; each Owner remains **A** for their domain fields. |

### DQ-007 — Item master code validity

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-007 |
| **CDE** | CDE-010 Item master code |
| **Dimension** | Validity (baseline) |
| **Business rule** | An item code used in inventory/procurement transactions must exist on the approved item master. |
| **Measurement method** | Compare transaction item codes to the item master. |
| **Expected outcome** | Codes not on master = 0 except documented exceptions. |
| **Threshold** | Validity-style — **`[A] Illustrative Rafid target`** |
| **Severity** | Medium |
| **Owner** | Supply Chain Director |
| **Steward** | Inventory / Procurement Manager |
| **Source/system** | ERP / inventory |
| **Frequency** | Steward operational monitoring (no numeric SLA) |
| **Exception handling** | Issue procedure. |

### DQ-008 — Facility / department code integrity

| Field | Content `[A]` |
| --- | --- |
| **Rule ID** | DQ-008 |
| **CDE** | CDE-013 Facility / department code |
| **Dimension** | Integrity (CDE-dependent; confirmed material) |
| **Business rule** | Consuming records that require a facility/department code must reference a code that exists on the organizational reference list (single source of truth principle at governance level; Phase 10 architecture is not built). |
| **Measurement method** | Orphan codes in agreed consuming extracts vs the reference list. |
| **Expected outcome** | Orphan codes = 0 except documented exceptions. |
| **Threshold** | Integrity-style — **`[A] Illustrative Rafid target`** |
| **Severity** | Medium |
| **Owner** | Strategy & Planning Director |
| **Steward** | Enterprise Data / PMO Analyst within DMO |
| **Source/system** | Org reference / planning lists |
| **Frequency** | Steward operational monitoring (no numeric SLA) |
| **Exception handling** | Issue procedure. DMO hosts Steward only; DMO is not Owner. |

---

## 5. Rule index (this drop only)

| Rule ID `[A]` | CDE | Dimension |
| --- | --- | --- |
| DQ-001 | CDE-001 National ID | Uniqueness |
| DQ-002 | CDE-003 Diagnosis code | Validity |
| DQ-003 | CDE-001 National ID | Completeness |
| DQ-004 | CDE-006 Credential expiry date | Timeliness |
| DQ-005 | CDE-007 Claim identifier | Uniqueness |
| DQ-006 | CDE-008 Billed service / charge code | Completeness |
| DQ-007 | CDE-010 Item master code | Validity |
| DQ-008 | CDE-013 Facility / department code | Integrity |

Eight rules. Not a large catalogue. Remaining catalogue CDEs may receive rules later using the same structure; they are **not** invented as extra CDEs.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved representative examples including DQ-001 and DQ-002 | Section 4 |
| `[B]` | One dimension per rule; Owner **A**; small library | Structure |
| `[C]` | Data Quality domain **name** | Context |
| `[NDMO verification required]` | Official NDMO quality-rule mandates | Not claimed |
