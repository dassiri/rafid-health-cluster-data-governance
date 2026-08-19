# Master Data Quality

**Document ID:** RHC-DG-P10-011  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for master quality outcomes; DMO (this application note) `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 7 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 7 dimensions reused; no second DQ framework.

**Phase:** 10 — Master data management  
**Does not decide:** New dimensions, CDEs, or thresholds

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document applies the **Phase 7 Data Quality Framework** to master entities.

It does **not** create a second Data Quality Framework. It does **not** add CDEs.

Trusted Data is an NDMO principle **name** `[C]`. That does not complete NDMO Data Quality `[NDMO verification required]`.

---

## 2. Seven dimensions (Phase 7 — reused, not redesigned)

Accuracy · Completeness · Validity · Uniqueness · Consistency · Timeliness · Integrity  

Baseline vs CDE-dependent split remains Phase 7 (Accuracy, Completeness, Validity baseline on every CDE; others CDE-dependent).

---

## 3. Two questions (locked)

| Concept | Question |
| --- | --- |
| **General Data Quality** | Quality of data assets / CDEs (Phase 7) |
| **MDM Quality** | Quality and **consistency of shared master entities and their attributes across consuming systems** |

Example `[A]`: National ID uniqueness (DQ-001) is both a CDE rule **and** an MDM uniqueness concern. The rule is not rewritten here. Downstream EMR vs billing copies failing **consistency** is the MDM overlay.

Issues still follow the Data Quality Issue Management Procedure (Phase 6 path). Prefer source correction (Phase 7). Lineage shows impact (Phase 9).

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative National ID overlay | Section 3 |
| `[B]` | MDM quality as cross-system consistency | Distinction |
| `[C]` | Data Quality domain **name**; Trusted Data **name** | Context |
| `[NDMO verification required]` | Official NDMO master-quality specifications | Not claimed |
