# Master Data Change Management

**Document ID:** RHC-DG-P10-014  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (change method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Locked triggers; Phase 4 rights unchanged.

**Phase:** 10 — Master data management  
**Does not decide:** CAB design; numeric SLAs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **when master data governance must be revisited**.

It uses **existing Phase 3/4 authority**. It does **not** modify Phase 4 decision rights.

---

## 2. Approved triggers (locked)

1. New master entity  
2. Attribute change  
3. Source system change  
4. Matching rule change  
5. Survivorship rule change  
6. Ownership change  
7. Classification change  
8. Reference code change  
9. System migration  

| Trigger | Existing path |
| --- | --- |
| Ownership change | Ownership Appointment Procedure (Phase 6) — Owner **A** still one per domain |
| Classification change | Phase 5 / Classification Procedure — Owner **A** |
| Matching / survivorship rule change | Owner **A** + Steward **R**; DMO registry |
| Reference code change | Code-set Owner **A** (not automatically Core MDM) |
| Policy-breaking change | Data Governance Exception Procedure (**DMC = A**, existing) |

Matching rule change does **not** authorize numeric thresholds or a match engine.

---

## 3. Roles

Steward: operational awareness and register update.  
Owner: business meaning of the change.  
DMO: registry consistency.  
Custodian: technical implementation in existing systems.

No new DMC class.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Nine triggers | Section 2 |
| `[C]` | Role **names** | Context |
| `[NDMO verification required]` | Official NDMO MDM-change mandates | Not claimed |
