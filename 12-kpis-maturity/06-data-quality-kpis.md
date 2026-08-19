# Data Quality KPIs

**Document ID:** RHC-DG-P12-006  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for domain quality interpretation; DMO method `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 7 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 7 reused; no second DQ framework; no enterprise index.

**Phase:** 12 — KPIs and maturity  
**Does not decide:** New dimensions, CDE scores, or live quality results

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **reuses Phase 7**.

Locked dimensions: Accuracy, Completeness, Validity, Uniqueness, Consistency, Timeliness, Integrity `[A][B]`.

**No second Data Quality Framework.**  
**No enterprise-wide single quality score.**  
**No arbitrary weighting.**

Issue path (title/path): `06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

---

## 2. KPIs in this domain

| KPI ID | Role |
| --- | --- |
| DG-KPI-005 | Executive — CDE Quality Composite (per-CDE unweighted; DMC sees **status distribution**, not a cluster index) |
| DG-KPI-006 | Executive — DQ Issue Closure Rate |
| DG-KPI-012 | Executive — Critical Issue Aging (severity reused) |

Per-dimension % remains the **operational** metric for Domain huddles (Phase 7 reporting table). It is not replaced by DG-KPI-005.

---

## 3. Composite rule (locked from Phase 7)

If a composite would mask a baseline or safety-critical dependent failure, **do not use the composite** for DMC reporting; show the failing dimension.

Phase 7’s thirteen CDEs remain **illustrative** `[A]`. They are not measured Rafid performance. This KPI does not invent CDE numeric scores.

Target Status: **To be established after baseline measurement.**

Illustrative threshold language from Phase 7 (Target / Warning / Breach) remains **`[A] Illustrative Rafid target`** there — not copied here as a live number.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Phase 7 scoring reuse | Sections 2–3 |
| `[C]` | Data Quality domain **name**; Trusted Data **name** | Context |
| `[NDMO verification required]` | Official NDMO quality KPIs | Not claimed |
