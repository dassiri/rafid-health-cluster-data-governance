# Year-1 MVP

**Document ID:** RHC-DG-P13-020  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (MVP method); listed Data Owners **A** in MVP domains  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phases 7–11 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — MVP boundaries copied, not expanded.

**Phase:** 13 — Implementation roadmap  
**Does not decide:** A wider Year-1 cut

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

Dedicated Year-1 MVP file. **Do not expand any MVP.**

Steward: **Business Data Steward**.

---

## 2. Phase 7 — Data Quality

**Existing 13 illustrative CDEs only** (copied from Phase 7 `04-cde-catalogue.md` — **not expanded**):

| CDE ID `[A]` | CDE (field) `[A]` | Domain | Data Owner (Phase 4) |
| --- | --- | --- | --- |
| CDE-001 | National ID | Patient / Person Master Data | Patient Access & Experience Director |
| CDE-002 | Patient identifier (MRN) | Patient / Person Master Data | Patient Access & Experience Director |
| CDE-003 | Diagnosis code | Clinical / Medical Records Data | Chief Medical Officer (CMO) |
| CDE-004 | Encounter documentation timestamp | Clinical / Medical Records Data | Chief Medical Officer (CMO) |
| CDE-005 | Provider identifier | Provider / Clinician Data | Medical Affairs Officer |
| CDE-006 | Credential expiry date | Provider / Clinician Data | Medical Affairs Officer |
| CDE-007 | Claim identifier | Financial / Billing & Claims Data | Chief Financial Officer (CFO) |
| CDE-008 | Billed service / charge code | Financial / Billing & Claims Data | Chief Financial Officer (CFO) |
| CDE-009 | Employee / staff identifier | Human Resources / Workforce Data | HR Director |
| CDE-010 | Item master code | Supply Chain & Asset Data | Supply Chain Director |
| CDE-011 | Item expiry date | Supply Chain & Asset Data | Supply Chain Director |
| CDE-012 | Incident severity classification | Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) |
| CDE-013 | Facility / department code | Reference / Organizational Master Data | Strategy & Planning Director |

**Do not add CDEs.**

---

## 3. Phase 8 — Metadata / Catalog

**Existing 3 priority domains only:**

1. Patient / Person Master Data — Patient Access & Experience Director  
2. Clinical / Medical Records Data — Chief Medical Officer (CMO)  
3. Financial / Billing & Claims Data — Chief Financial Officer (CFO)  

---

## 4. Phase 10 — MDM

| Entity | Scope |
| --- | --- |
| Patient / Person Master | **Primary** |
| Provider / Clinician Master | **Primary** |
| Facility / Organization Master | **Supporting only** |

**Do NOT create a third full MDM workstream.** Owners: Patient Access & Experience Director; Medical Affairs Officer; Strategy & Planning Director (Facility supporting).

---

## 5. Phase 11 — Lifecycle

- Patient / Person Master  
- Clinical / Medical Records  
- Financial / Billing & Claims  

**Do not expand these scopes.** **No invented retention periods.** Periods remain `[NDMO verification required]` / `[Legal / regulatory verification required]`.

---

## 6. Other Year-1 notes

Classification uses Rafid tiers `[A][B]` on in-scope datasets — not NDMO national names. Lineage Year-1 remains Critical Lineage focus for the same three domains as Phase 9 design. KPI baseline uses Phase 12’s 12 executive KPIs with **no live results** in this repository.

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | MVP cut application to the roadmap | Entire file |
| `[B]` | Pilot narrow, then scale | Purpose |
| `[NDMO verification required]` | Official MVP mandates | Not claimed |
