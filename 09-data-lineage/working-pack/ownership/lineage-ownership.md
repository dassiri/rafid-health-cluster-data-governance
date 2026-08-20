# Lineage Ownership (Working Pack)

**Document ID:** RHC-DG-P9-WP-011  
**Version:** 1.0  
**Status:** Implemented (working design only)  
**Owner:** DMO `[B]` (method)  
**Parent design:** [`../../11-lineage-ownership.md`](../../11-lineage-ownership.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

This file applies **existing** Phase 4 roles to lineage working records. It does **not** create new roles, a new RACI, or a new Data Management Committee decision class.

Role types: [`../../../03-operating-model/03-role-catalogue.md`](../../../03-operating-model/03-role-catalogue.md)  
Domain titles: [`../../../04-ownership-stewardship/02-enterprise-ownership-matrix.md`](../../../04-ownership-stewardship/02-enterprise-ownership-matrix.md)

NDMO role **names** `[C]`: Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office, Entity Data Management Committee. Specification-level duties remain `[NDMO verification required]`.

---

## 2. Roles applied to lineage (locked — reused)

| Role | Lineage responsibility |
| --- | --- |
| **Data Owner** | **Accountable** for **business lineage correctness** of assets in that domain |
| **Business Data Steward** | **Responsible** for **maintaining lineage metadata** |
| **IT / Data Custodian** (IT Data Steward) | **Responsible** for **technical lineage information where applicable** (Year-1: conceptual description, not a scanner) |
| **DMO** | Lineage governance **methodology**; **registry**; **quality oversight** of lineage records |
| **DMC** | Governance escalation and decisions **within the approved Phase 3 framework only** |

There is **no lineage-only Owner**. IT is **not** the Data Owner.

---

## 3. MVP titles (Phase 4 — unchanged)

| Domain | Data Owner | Business Data Steward | IT / Data Custodian (system class) |
| --- | --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access | Registration / MPI Custodian |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | EMR Application Custodian |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager | Billing / Claims Custodian |

Steward **role type** remains Business Data Steward. Named titles above are the Phase 4 appointed seats already used in the Phase 8 working pack.

---

## 4. Responsibilities by lineage activity `[A][B]`

| Activity | Data Owner | Business Data Steward | DMO | IT / Data Custodian |
| --- | --- | --- | --- | --- |
| **Lineage submission** (draft ID, candidate hop) | Informed; confirms domain | **R** — creates the draft Lineage Record | Method / ID convention | **C** — system / structure facts |
| **Lineage validation** | Accepts business meaning where required | **R** — completeness of Source → Target → Consumer | Completeness / consistency check | **C** — technical location accuracy |
| **Lineage approval** | **A** when the flow’s **business meaning** is at stake | Prepares the pack; cannot approve meaning alone | Governance check; cannot rewrite clinical or finance meaning | None for business meaning |
| **Lineage maintenance** | **A** for material business-driven change | **R** — updates metadata on approved triggers | Registry consistency | **C** — technical facts of system / transformation change |
| **Lineage review** | **A** for material change; periodic confirmation of meaning | **R** — periodic confirmation | Oversight of review evidence | **C** when systems changed |
| **Lineage exception handling** | Raises or accepts business exception need | Coordinates the record | Routes via existing exception procedure | Supplies technical impact |

DMC does **not** approve every lineage record. Out-of-policy handling reuses the Phase 6 **Data Governance Exception Procedure** (**DMC = A**).

---

## 5. Cross-domain rule (unchanged)

Cross-domain flows have **one Owner per asset**, not one Owner for the whole chain.

| Example hop | Source Owner (still A for source) | Target Owner (row primary) |
| --- | --- | --- |
| LIN-002 Patient → Encounter | Patient Access & Experience Director | CMO |
| LIN-003 Encounter → Claims | CMO | CFO |
| LIN-011 Patient → Claims | Patient Access & Experience Director | CFO |

DMO coordinates. No shared **A**.

---

## 6. Applied to the 13-row register

| Domain Owner | Rows where that Owner is primary on the record |
| --- | --- |
| Patient Access & Experience Director | LIN-001, LIN-006, LIN-007 |
| CMO | LIN-002, LIN-010 |
| CFO | LIN-003, LIN-004, LIN-005, LIN-008, LIN-009, LIN-011, LIN-012, LIN-013 |

---

## 7. What this file does not do

- Does not invent a lineage council or a second Owner
- Does not let Custodian classify or define meaning
- Does not add a DMC decision class for routine lineage publish
