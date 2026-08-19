# Disposal Evidence

**Document ID:** RHC-DG-P11-011  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (record method); Data Owner **A** for authorization on the record  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Disposal Record fields; proposed artifact only.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Certificate formats or vendor evidence templates

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the **Disposal Record**.

**Label:** `[A]` Proposed Rafid governance artifact.

**Do NOT claim it is NDMO-mandated.**

Principle: **Evidence of disposition** ([02](02-lifecycle-principles.md)). Disposal is not closed on an informal email.

---

## 2. Minimum fields (locked)

| Field | Intent |
| --- | --- |
| **Disposal Record ID** | Unique identifier |
| **Asset / Record Type** | What was disposed (catalog-aligned) |
| **Owner** | Exact Phase 4 Data Owner title |
| **Classification** | Rafid tier at disposal |
| **Retention Rule** | Retention Rule ID applied |
| **Eligibility Date** | When the candidate was treated as eligible (must not rest on an invented period) |
| **Legal Hold Check** | Confirmation that no active hold blocked disposal |
| **Authorization** | Data Owner **A** (Phase 4 row 10) |
| **Disposal Date** | When execution occurred |
| **Disposal Method** | Conceptual method class used ([10](10-disposal-destruction.md)) |
| **Executing Party** | Custodian or approved provider |
| **Evidence / Reference** | Pointer to certificates, tickets, or provider confirmation — conceptual |
| **Verification** | Independent check that evidence matches authorization |
| **Closure Status** | Open / verified / closed |

---

## 3. Illustrative occupancy `[A]`

| Field | Example occupancy (not live) |
| --- | --- |
| Disposal Record ID | DR-ILL-001 `[A]` |
| Asset / Record Type | Illustrative extract no longer required for operations `[A]` |
| Owner | Chief Medical Officer (CMO) *(only if that domain asset)* |
| Classification | Restricted `[A][B]` |
| Retention Rule | RR-ILL-002 (period still `[Legal / regulatory verification required]` — **would not authorize live disposal**) |
| Eligibility Date | Not claimed — unverified period means **not eligible** in a live process |
| Legal Hold Check | Required before any live close |
| Authorization | Data Owner **A** when actually eligible |
| Closure Status | Documentation example only — **not** a completed destruction |

The illustrative row is **deliberately not a completed live disposal**. Unverified retention does not produce a closed destruction.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Proposed Disposal Record | Entire document |
| `[B]` | Evidence of disposition as practice | Section 1 |
| `[NDMO verification required]` | Official NDMO disposal-evidence specifications | Not claimed |
