# Metadata Ownership

**Document ID:** RHC-DG-P8-012  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 4 ownership model `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Applies Phase 4 RACI to metadata; no new decision rows; no new DMC class.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Named incumbents; a new RACI; hospital catalogs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document states **who owns metadata** using **Phase 4 exactly**.

It does **not** modify the Phase 4 decision RACI. Pointer:

`04-ownership-stewardship/03-ownership-decision-matrix.md`

Relevant existing rows:

| Row | Decision | Single **A** |
| --- | --- | --- |
| 1 | Data definition | Data Owner |
| 3 | Data classification | Data Owner |
| 8 | Metadata/catalog **content** approval | Data Owner |
| 5 | Access approval (**exception**) | DMC |

Catalog **programme** remains CDO/DMO (Phase 3 / STD-004). That is not a new DMC class and not a change to row 8.

NDMO names: Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office, Entity Data Management Committee `[C]`. Specification-level duties `[NDMO verification required]`.

---

## 2. Metadata responsibilities (locked)

| Role | Metadata responsibility |
| --- | --- |
| **Data Owner** | **Accountable** for business metadata and definitions (and for **Certified** status) |
| **Business Data Steward** | **Responsible** for metadata maintenance and metadata quality; Registered and Reviewed statuses |
| **IT Data Steward / Custodian** | **Responsible** for technical metadata **where applicable**; never **A** for business meaning |
| **DMO** | Metadata governance **methodology**; catalog **oversight**; registration **governance check** (cannot rewrite meaning) |
| **DMC** | Governance escalation and decisions **within the approved Phase 3 governance authority and decision-right framework** only — **no new DMC decision class** |
| **PDPO** | **C** when the definition is personal/health-identifying (Phase 4 note on row 1); **A** only on the existing sharing **privacy** row — not on catalog publish |

---

## 3. What DMC does **not** gain in this phase

This phase does **not** add:

- DMC approval of every catalog asset
- DMC as catalog content Owner
- A “metadata exception” decision separate from the existing Policy exception path

Policy-level exceptions still use:

**Data Governance Exception Procedure** — `06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md` (**DMC = A**).

---

## 4. Domain Owner titles (Phase 4 — unchanged) `[A]`

Used when an example must name the Owner. Steward examples use only **Business Data Steward**.

| Domain | Data Owner |
| --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) |
| Provider / Clinician Data | Medical Affairs Officer |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) |
| Human Resources / Workforce Data | HR Director |
| Supply Chain & Asset Data | Supply Chain Director |
| Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) |
| Reference / Organizational Master Data | Strategy & Planning Director |

IT is not Owner of any domain. DMO hosts the Steward for Domain 8 only; DMO is not Owner.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Phase 4 title map | Section 4 |
| `[B]` | Owner A / Steward R / Custodian technical / DMO method | Section 2 |
| `[C]` | NDMO role **names** | Naming |
| `[NDMO verification required]` | Organizational Manual duties | Not used as IDs |
