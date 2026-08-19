# Data Lifecycle and Data Quality

**Document ID:** RHC-DG-P11-015  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for quality rules (Phase 4 / 7); DMO method `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 7 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Seven Phase 7 dimensions reused; no second DQ framework.

**Phase:** 11 — Data lifecycle  
**Does not decide:** New dimensions, CDEs, or scorecards

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **reuses Phase 7**.

**Do NOT create a second Data Quality Framework.**

Locked dimensions: **Accuracy, Completeness, Validity, Uniqueness, Consistency, Timeliness, Integrity** `[A][B]`.

Issue path remains the existing Data Quality Issue Management Procedure (title/path only): `06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

---

## 2. How lifecycle events affect dimensions `[A][B]`

| Dimension | Lifecycle effect (conceptual) |
| --- | --- |
| **Accuracy** | Archive/migrate/dispose of a **source** can leave downstream values uncorrectable if lineage is not reviewed |
| **Completeness** | Early disposal or premature archive of required inputs can create gaps in active processes |
| **Validity** | Retired code lists (Reference domain) without archived versions make old records look “invalid” against current lists |
| **Uniqueness** | MDM match/merge (Phase 10) changes uniqueness; enterprise dispose of a survivor/victim copy needs Owner review |
| **Consistency** | Share/archive/migration can fork copies; retained copies must remain consistent with the approved rule |
| **Timeliness** | Archived data is not “late operational data”; active processes must not depend on archive as a real-time source |
| **Integrity** | Partial disposal (some tables, not related evidence) can break referential integrity of what remains |

Lifecycle events do **not** replace CDE scoring. Phase 7 scorecards remain illustrative there; this phase adds **no** numeric quality targets.

---

## 3. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Dimension impact notes | Section 2 |
| `[C]` | Quality domain **name** | Context |
| `[NDMO verification required]` | Official NDMO quality-during-lifecycle specs | Not claimed |
