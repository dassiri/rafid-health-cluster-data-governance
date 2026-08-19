# Critical Data Element Catalogue (Illustrative)

**Document ID:** RHC-DG-P7-004  
**Version:** 1.0  
**Status:** Implemented (illustrative catalogue only)  
**Owner:** Chief Data Officer / DMO `[B]` (registry method); each domain **Data Owner** remains **A** for CDE confirmation in that domain  
**Approver:** CDO `[B]` (catalogue as framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Exactly 13 approved illustrative CDEs; Phase 4 titles unchanged.

**Phase:** 7 — Data quality  
**Does not decide:** Additional CDEs; live inventory; catalog records (Phase 8)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This catalogue records the **approved illustrative set of exactly 13 CDEs** for the fictional Rafid Health Cluster `[A]`.

All 13 examples are **fictional/illustrative**. They are **not** a measured Rafid inventory and **not** an NDMO-mandated CDE list `[NDMO verification required]`.

**Do not add CDEs in this phase.** Domain quality **priorities** that are not in this list remain watch-items ([`13-domain-priorities.md`](13-domain-priorities.md)); they are not extra CDEs.

Ownership titles are taken **unchanged** from Phase 4.

---

## 2. Coverage rule

| Requirement | Result |
| --- | --- |
| All 8 Phase 4 domains represented | Yes |
| Count of CDEs | **13** |
| Additional CDEs | **None** |

---

## 3. Approved illustrative CDEs `[A]`

Baseline dimensions (Accuracy, Completeness, Validity) apply to **every** row. **Dependent** columns list CDE-dependent dimensions the Owner/Steward would typically confirm as material `[A][B]` — still subject to Step 2 confirmation in a live process.

| CDE ID `[A]` | CDE (field) `[A]` | Domain | Data Owner (Phase 4) | Business Data Steward (Phase 4) | Why a candidate (criteria, illustrative) | Typical dependent dimensions `[A]` | Typical source class `[A]` |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **CDE-001** | National ID | Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access | Patient safety; regulatory; privacy/security; cross-domain | Uniqueness, Consistency, Integrity | EMR / MPI / registration |
| **CDE-002** | Patient identifier (MRN) | Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access | Patient safety; operational; cross-domain; decision-making | Uniqueness, Consistency, Integrity | EMR / MPI |
| **CDE-003** | Diagnosis code | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | Patient safety; regulatory; financial (downstream coding); executive reporting | Integrity, Consistency | EMR clinical |
| **CDE-004** | Encounter documentation timestamp | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | Patient safety; operational; decision-making | **Timeliness**, Integrity | EMR clinical |
| **CDE-005** | Provider identifier | Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator | Patient safety; operational; cross-domain (HR / EMR) | Uniqueness, Consistency, Integrity | Credentialing / EMR provider master |
| **CDE-006** | Credential expiry date | Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator | Patient safety; regulatory; operational | **Timeliness**, Validity (already baseline), Integrity | Credentialing system |
| **CDE-007** | Claim identifier | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager | Financial; operational; regulatory | Uniqueness, Integrity | Billing / claims |
| **CDE-008** | Billed service / charge code | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager | Financial; operational; cross-domain (clinical coding) | Consistency, Integrity, **Timeliness** | Billing / HIS financial |
| **CDE-009** | Employee / staff identifier | Human Resources / Workforce Data | HR Director | HR Operations Manager | Operational; financial (payroll); cross-domain (roster–EMR) | Uniqueness, Consistency, Integrity | HRIS |
| **CDE-010** | Item master code | Supply Chain & Asset Data | Supply Chain Director | Inventory / Procurement Manager | Operational; patient safety (wrong item); financial | Uniqueness, Consistency, Integrity | ERP / inventory |
| **CDE-011** | Item expiry date | Supply Chain & Asset Data | Supply Chain Director | Inventory / Procurement Manager | Patient safety; operational; regulatory | **Timeliness**, Integrity | ERP / inventory |
| **CDE-012** | Incident severity classification | Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) | Quality Improvement Manager | Patient safety; regulatory; executive reporting; decision-making | Consistency, Validity (baseline), Integrity | Quality / incident system |
| **CDE-013** | Facility / department code | Reference / Organizational Master Data | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | Cross-domain; operational; executive reporting; consistency of SOT | Uniqueness, Consistency, Integrity | Org reference / planning lists |

**Count check:** CDE-001 through CDE-013 = **13**. No additional CDE identifiers.

**Steward sitting in DMO (CDE-013):** DMO **hosts** the Steward. DMO is **not** the Data Owner. Owner remains Strategy & Planning Director (Phase 4).

---

## 4. Domain coverage map

| Domain | CDE IDs `[A]` |
| --- | --- |
| Patient / Person Master Data | CDE-001, CDE-002 |
| Clinical / Medical Records Data | CDE-003, CDE-004 |
| Provider / Clinician Data | CDE-005, CDE-006 |
| Financial / Billing & Claims Data | CDE-007, CDE-008 |
| Human Resources / Workforce Data | CDE-009 |
| Supply Chain & Asset Data | CDE-010, CDE-011 |
| Quality & Patient Safety Data | CDE-012 |
| Reference / Organizational Master Data | CDE-013 |

---

## 5. What this catalogue is not

- Not production measurement
- Not a license to add CDEs in this drop
- Not Phase 8 catalog entries
- Not Phase 10 golden-record design (even where uniqueness is a dependent dimension)
- Not an NDMO CDE register `[NDMO verification required]`

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved illustrative 13-CDE set; Phase 4 title map | Table |
| `[B]` | Field-level CDE; Owner confirmation | Method |
| `[C]` | Role **names** (BDE / BDS); Data Quality domain **name** | Role types only |
| `[NDMO verification required]` | Any official CDE mandate or list | Not used |
