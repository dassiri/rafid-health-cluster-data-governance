# Lifecycle by Data Domain

**Document ID:** RHC-DG-P11-013  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Each domain Data Owner **A**; DMO method `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 4 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Eight Phase 4 domains; no invented periods or Owner titles.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Statutory periods; new Owner titles

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document **applies the framework conceptually** to all eight approved Phase 4 domains.

**Use ONLY the 8 exact Phase 4-approved Owner titles.**  
**Steward role: Business Data Steward only.**  
**Do NOT invent retention periods.**

Every domain’s Retention Period remains `[Legal / regulatory verification required]` and `[NDMO verification required]` until verified. Triggers below are `[A]` illustrative.

Classification **influences handling**. **Classification does NOT automatically determine retention duration.**

---

## 2. Patient / Person Master

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Identity data is created at registration, used across care, and remains sensitive after a relationship ends. MDM deactivation (Phase 10) is **not** the same as enterprise disposal. |
| **Approved Data Owner** | Patient Access & Experience Director |
| **Steward** | Business Data Steward |
| **Classification considerations** | Typically Restricted `[A][B]` when identifying — handling, not a clock |
| **Retention trigger examples** `[A]` illustrative | Patient relationship end; last activity |
| **Archive considerations** | Reduced active registration use; still retained until a **verified** rule allows otherwise; Archive ≠ Backup |
| **Disposal considerations** | Hold check; Owner **A**; evidence; period must be verified first |

---

## 3. Clinical / Medical Records

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Encounter and clinical documentation support care and may be evidential records. Records Management is **distinct** and **not built** here. |
| **Approved Data Owner** | Chief Medical Officer (CMO) |
| **Steward** | Business Data Steward |
| **Classification considerations** | Typically Restricted `[A][B]` — handling for access, sharing, disposal method class |
| **Retention trigger examples** `[A]` illustrative | Record completion; case closure; patient relationship end |
| **Archive considerations** | Historical/reference and legal/record value when verified; classification persists |
| **Disposal considerations** | Do not invent health-record clocks; unverified period ≠ eligible |

---

## 4. Financial / Billing & Claims

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Claims and billing events (transaction data) follow financial accountability; not Core MDM (Phase 10). |
| **Approved Data Owner** | Chief Financial Officer (CFO) |
| **Steward** | Business Data Steward |
| **Classification considerations** | Often Confidential `[A][B]`; Restricted if combined with identifiers in a way the Owner classifies as Restricted — Owner **A** |
| **Retention trigger examples** `[A]` illustrative | Case closure; contract termination; record completion |
| **Archive considerations** | Reduced active billing use; financial/reference value |
| **Disposal considerations** | Owner **A**; hold check; no invented financial statutory period |

---

## 5. Provider / Clinician

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Provider identity is Core MDM (Phase 10). Deactivate in MDM ≠ dispose of credentialing history. |
| **Approved Data Owner** | Medical Affairs Officer |
| **Steward** | Business Data Steward |
| **Classification considerations** | Often Confidential / Restricted depending on content — Owner **A**; not auto-duration |
| **Retention trigger examples** `[A]` illustrative | Last activity; contract termination; record completion |
| **Archive considerations** | Historical credentialing reference while retained |
| **Disposal considerations** | Downstream clinical/financial use (lineage) before any disposal |

---

## 6. HR / Workforce

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Employment records; Non-MDM at Phase 10 maturity. Personal data → PDPO **C**. |
| **Approved Data Owner** | HR Director |
| **Steward** | Business Data Steward |
| **Classification considerations** | Typically Confidential / Restricted `[A][B]` — handling |
| **Retention trigger examples** `[A]` illustrative | Contract termination; last activity; record completion |
| **Archive considerations** | Workforce history while a **verified** rule still requires keep |
| **Disposal considerations** | No invented labour-law period; verification required |

---

## 7. Supply Chain & Asset

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Item/asset operational data; Item treated as **reference data** in Phase 10 — no MDM-specific retention rule. |
| **Approved Data Owner** | Supply Chain Director |
| **Steward** | Business Data Steward |
| **Classification considerations** | Internal to Restricted depending on asset — Owner **A** |
| **Retention trigger examples** `[A]` illustrative | Contract termination; last activity; case closure (incident-linked assets) |
| **Archive considerations** | Equipment/item history for reference while retained |
| **Disposal considerations** | Physical media destruction only when media is in scope — conceptual |

---

## 8. Quality & Patient Safety

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Incidents and quality events may have investigation and learning value; may intersect records/legal hold. |
| **Approved Data Owner** | Chief Quality & Patient Safety Officer (CQPSO) |
| **Steward** | Business Data Steward |
| **Classification considerations** | Often Confidential / Restricted `[A][B]` |
| **Retention trigger examples** `[A]` illustrative | Case closure; record completion |
| **Archive considerations** | Learning/reference value; hold may apply |
| **Disposal considerations** | Hold overrides; no invented patient-safety statutory period |

---

## 9. Reference / Organizational Master

| Item | Statement |
| --- | --- |
| **Typical lifecycle considerations** | Facility/org codes and reference lists; Facility is lightweight supporting MDM only (Phase 10). Code retirement ≠ enterprise disposal of historical reports using those codes. |
| **Approved Data Owner** | Strategy & Planning Director |
| **Steward** | Business Data Steward |
| **Classification considerations** | Often Internal / Public for non-sensitive org lists; Owner **A** |
| **Retention trigger examples** `[A]` illustrative | Last activity; record completion (list version superseded) |
| **Archive considerations** | Historical code lists needed to interpret old reports (lineage) |
| **Disposal considerations** | Downstream impact review (Phase 9) before dispose |

---

## 10. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Domain application; illustrative triggers | Sections 2–9 |
| `[B]` | Same lifecycle method across domains | Entire document |
| `[NDMO verification required]` | NDMO domain retention specifications | Periods |
| `[Legal / regulatory verification required]` | Healthcare and other sector law | Periods |
