# Lineage Ownership

**Document ID:** RHC-DG-P9-011  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 4 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 4 roles applied to lineage; no new RACI; no new DMC class.

**Phase:** 9 — Data lineage  
**Does not decide:** Named incumbents; a lineage-only Owner

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document applies **Phase 4 roles exactly** to lineage. It does **not** modify the Phase 4 decision RACI.

Pointer: `04-ownership-stewardship/03-ownership-decision-matrix.md`

Cross-domain flows have **one Owner per asset**, not one Owner for the whole chain. DMO coordinates. No shared **A**.

NDMO role **names** `[C]`: Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office, Entity Data Management Committee. Specification-level duties `[NDMO verification required]`.

---

## 2. Responsibilities (locked)

| Role | Lineage responsibility |
| --- | --- |
| **Data Owner** | **Accountable** for **business lineage correctness** of assets in that domain |
| **Business Data Steward** | **Responsible** for **maintaining lineage metadata** |
| **IT Data Steward / Custodian** | **Responsible** for **technical lineage information where applicable** (Year-1: conceptual description, not a scanner) |
| **DMO** | Lineage governance **methodology**; **registry**; **quality oversight** of lineage records |
| **DMC** | Governance escalation and decisions **within the approved Phase 3 governance authority and decision-right framework** |

---

## 3. DMC — no new decision right

This phase does **not** add DMC approval of every lineage record.

DMC remains **A** only for **existing** classes (L3 policy, material exceptions, residual sharing risk, Owner non-participation, access exception). Out-of-policy lineage handling uses the existing exception path (**DMC = A**).

---

## 4. MVP Owner titles (Phase 4 — unchanged) `[A]`

| Domain | Data Owner |
| --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) |

Steward examples use **Business Data Steward** only.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Phase 4 titles | Section 4 |
| `[B]` | Owner A / Steward R / Custodian technical / DMO method | Section 2 |
| `[C]` | NDMO role **names** | Naming |
| `[NDMO verification required]` | Organizational Manual | Not used as IDs |
