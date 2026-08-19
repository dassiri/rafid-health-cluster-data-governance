# Root Cause Analysis

**Document ID:** RHC-DG-P7-009  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Business Data Steward **R** (perform); Data Owner **A** (accept cause for closure)  
**Approver:** CDO `[B]` (method)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Lightweight RCA categories; no incident-management methodology.

**Phase:** 7 — Data quality  
**Does not decide:** ITIL/incident tool design; full safety-investigation protocol for clinical incidents (those remain quality/safety process under CQPSO where applicable)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records a **lightweight** root-cause category set for data quality issues `[A][B]`.

It is not a complex incident-management methodology. It is not a clinical sentinel-event protocol. Where a quality **data** issue is also a patient-safety **incident**, the CQPSO domain process still applies to the incident; this file only categorizes the **data** defect.

---

## 2. Approved categories (locked) `[A][B]`

Record **one primary** category. Additional contributing categories may be listed; they do not create a second Owner.

| Category | Meaning |
| --- | --- |
| **Source system defect** | The originating application stores or emits an incorrect value. |
| **Manual entry error** | A person entered or selected the wrong value. |
| **Integration failure** | The value was lost, duplicated, or altered in a feed/interface. |
| **Transformation logic** | Mapping, derivation, or conversion produced the defect. |
| **Reference/master data problem** | Code lists, masters, or identity keys are wrong or drifted. |
| **Process design** | The business process allows or encourages the defect. |
| **User training** | The process is adequate; execution knowledge is not. |
| **Governance gap** | Definition, ownership, rule, or exception handling was missing or unclear. |

These categories are Rafid design `[A][B]`. They are not NDMO-mandated RCA codes `[NDMO verification required]`.

---

## 3. How RCA is used

| Step | Who |
| --- | --- |
| Propose category | Steward, with Custodian if technical |
| Challenge measurability / system fact | Custodian |
| Accept category for the issue record | Data Owner **A** (may be with closure) |
| Recurring governance-gap themes | DMO to Steward Forum; DMC if residual enterprise risk |

Do not require a five-whys workshop for every Low issue. Depth follows qualitative severity `[B]`. **No numeric SLA** for “RCA complete in N days.”

---

## 4. What this file does not do

- No fishbone templates as mandatory artifacts
- No ITIL priority matrix
- No Phase 10 matching-algorithm RCA
- No invented NDMO control IDs

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved eight categories; lightweight use | Sections 2–3 |
| `[C]` | Data Quality domain **name** | Context |
| `[NDMO verification required]` | Official NDMO RCA method | Not claimed |
