# Lineage Change Management

**Document ID:** RHC-DG-P9-014  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (change method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Locked triggers; Phase 4 decision rights unchanged.

**Phase:** 9 — Data lineage  
**Does not decide:** Change-advisory-board design; numeric SLAs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **when lineage must be reviewed or updated** `[A][B]`.

It does **not** change Phase 4 decision rights.

---

## 2. Approved triggers (locked)

1. New source  
2. New target  
3. Transformation / ETL logic change  
4. New report/KPI  
5. System migration  
6. Data model change  
7. Ownership change  
8. Classification change  
9. Quality-rule change  

“ETL logic change” is a **trigger name**. It does **not** authorize an ETL implementation in this phase. Custodian describes the conceptual transformation change.

Classification change still uses the Phase 5 / classification procedure path. Lineage update **follows**; lineage does not reclassify.

Ownership change uses Phase 6 ownership appointment path. Lineage records are then updated.

Quality-rule change uses Phase 7 / Phase 4 quality-rules **A** = Data Owner. Lineage impact analysis may follow.

---

## 3. Roles (locked)

| Role | Change duty |
| --- | --- |
| **Business Data Steward** | Operational awareness and update of lineage metadata |
| **Data Owner** | Business-driven changes / business meaning of the flow |
| **DMO** | Registry consistency and governance oversight |
| **Custodian** | Technical facts of system/transformation change (input, not Owner) |

No new DMC class. Material Policy exceptions still **DMC = A**.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Nine triggers; role split | Sections 2–3 |
| `[C]` | Role **names** | Context |
| `[NDMO verification required]` | Official NDMO lineage-change mandates | Not claimed |
