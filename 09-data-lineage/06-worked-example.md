# Worked End-to-End Lineage Example

**Document ID:** RHC-DG-P9-006  
**Version:** 1.0  
**Status:** Implemented (exactly one illustrative example)  
**Owner:** DMO `[B]` (example as teaching artifact); domain Owners **A** for meaning in a live process  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Single E2E example; architecture disclaimers locked.

**Phase:** 9 — Data lineage  
**Does not decide:** Real integration design; national interchange specifications

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose and disclaimers (mandatory)

This file contains **exactly one** detailed illustrative end-to-end example `[A]`.

```text
Patient Registration
→ Patient Master
→ Clinical Encounter
→ Billing / Claims
→ External Claims Interchange
```

**This example does not represent:**

- Real MOH architecture
- Real NPHIES architecture
- Real Rafid architecture

“External Claims Interchange” is **generic national claims interchange** terminology `[A]`. It is **not** a named national product. If NPHIES or other national-interchange-specific requirements are asserted, they remain `[NDMO verification required]` and are **not** designed here.

All rows below are `[A]` illustrative. Steward is labeled **Business Data Steward** only. Classification values are **illustrative Owner-assessed Rafid tiers** using the Phase 5 method — **not** automatic inheritance from upstream ([`09-lineage-and-classification.md`](09-lineage-and-classification.md)).

---

## 2. Step 1 — Patient Registration `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| **Asset** | Patient Registration dataset |
| **Example data elements** | National ID (CDE-001), Patient identifier / MRN (CDE-002), contact fields (watch-item, not extra CDE) |
| **Data Owner** | Patient Access & Experience Director |
| **Business Data Steward** | Business Data Steward |
| **Classification** | Restricted — illustrative dataset-level assessment (Phase 5); not an NDMO national tier |
| **Quality considerations** | Completeness/uniqueness of National ID and MRN (Phase 7 DQ-001, DQ-003) |
| **Business purpose** | Create a registrable person identity for care access |

**Lineage role:** Source (originating capture).

---

## 3. Step 2 — Patient Master `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| **Asset** | Patient Master Record (MVP asset) |
| **Example data elements** | National ID, Patient identifier (MRN), demographics used for matching |
| **Data Owner** | Patient Access & Experience Director |
| **Business Data Steward** | Business Data Steward |
| **Classification** | Restricted — **separately assessed** under Phase 5; not auto-copied from Registration |
| **Quality considerations** | Uniqueness / identity duplication (Phase 7 Patient Master priorities) |
| **Business purpose** | Cluster person master used by downstream care and billing processes |

**Lineage role:** Target of registration; source to clinical and billing. Transformation (conceptual): identity persist / MPI-style match **described**, not a matching engine (Phase 10 is Designed / Documented as conceptual MDM; operational implementation is not claimed).

---

## 4. Step 3 — Clinical Encounter `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| **Asset** | Encounter / Diagnosis record (MVP asset) |
| **Example data elements** | Encounter documentation timestamp (CDE-004), Diagnosis code (CDE-003), Patient identifier (consumed, not owned as clinical meaning) |
| **Data Owner** | Chief Medical Officer (CMO) |
| **Business Data Steward** | Business Data Steward |
| **Classification** | Restricted — illustrative; Owner (CMO) assesses this **dataset** under Phase 5 |
| **Quality considerations** | Diagnosis validity (DQ-002); documentation timeliness (CDE-004) |
| **Business purpose** | Record the care encounter and structured diagnosis |

**Lineage role:** Consumes Patient Master identity; source to billing. Transformation (conceptual): clinical documentation and coding.

---

## 5. Step 4 — Billing / Claims `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| **Asset** | Claims Extract (MVP asset) / claims dataset |
| **Example data elements** | Claim identifier (CDE-007), billed service / charge code (CDE-008), diagnosis code as billing input (consumed) |
| **Data Owner** | Chief Financial Officer (CFO) |
| **Business Data Steward** | Business Data Steward |
| **Classification** | Restricted — illustrative combined-impact assessment possible under Phase 5 **highest applicable impact**; **still an Owner decision**, not a Phase 9 inheritance rule |
| **Quality considerations** | Duplicate claims (DQ-005); charge completeness (DQ-006); coding mismatch vs clinical diagnosis |
| **Business purpose** | Prepare a claim for reimbursement |

**Lineage role:** Target of encounter/coding; source to external interchange. Transformation (conceptual): charge capture and claim composition.

---

## 6. Step 5 — External Claims Interchange `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| **Asset** | Outbound claims interchange extract (generic) |
| **Example data elements** | Claim identifier, billed codes, identity elements as required for the interchange **context** (not specified as a national schema here) |
| **Data Owner** | Chief Financial Officer (CFO) for the cluster **extract asset**; sharing still uses two Phase 4 decisions (Owner business **A**; PDPO privacy **A** where personal data applies) |
| **Business Data Steward** | Business Data Steward |
| **Classification** | Assessed under Phase 5 for **this extract dataset**; lineage only flags that source elements may still be present |
| **Quality considerations** | Invalid codes or duplicate claim IDs propagate to rejection risk (see [`07-business-lineage-example.md`](07-business-lineage-example.md)) |
| **Business purpose** | Submit or stage a claim to a **generic national claims interchange** |

**Lineage role:** Consumer of the claims extract. This is **not** NPHIES architecture. National-interchange-specific requirements: `[NDMO verification required]`.

---

## 7. Conceptual chain (summary) `[A]`

```text
Registration dataset (source)
  → persist/match (transformation — conceptual)
→ Patient Master Record (target / source)
  → identity used on encounter (movement)
→ Encounter / Diagnosis record (target / source)
  → charge/claim composition (transformation — conceptual)
→ Claims Extract (target / source)
  → outbound mapping (transformation — conceptual)
→ External Claims Interchange (consumer)
```

This remains the **only** detailed end-to-end example in Phase 9.

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative flow, assets, elements, tiers | Sections 2–7 |
| `[B]` | Cross-domain conceptual lineage | Structure |
| `[C]` | PDPO **name** (privacy review remains a separate sharing decision) | Step 5 note |
| `[NDMO verification required]` | NPHIES / national interchange specifications | Disclaimer |
