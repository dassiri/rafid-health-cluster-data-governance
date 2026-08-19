# Lineage Governance Artifacts

**Document ID:** RHC-DG-P9-015  
**Version:** 1.0  
**Status:** Implemented (proposed artifacts only)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual index; exceptions reuse Phase 6.

**Phase:** 9 — Data lineage  
**Does not decide:** Physical schemas; NDMO-mandated registers `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document is a **conceptual design/index** of proposed Rafid lineage artifacts `[A][B]`.

They are **not** claimed as NDMO-mandated. **No compliance is claimed. No NDMO control IDs are invented.**

---

## 2. Proposed artifacts (locked list)

| Artifact `[A][B]` | Purpose |
| --- | --- |
| **Lineage Registry** | Working list of documented flows (candidate and confirmed) |
| **Lineage Record** | One flow: Source → Transformation → Target → Consumer; granularity; Owners |
| **Lineage Change Record** | Evidence that a trigger was handled |
| **Lineage Review Record** | Periodic confirmation |
| **Critical Lineage Register** | Confirmed prioritized coverage (Year-1 MVP **focus**) |
| **Lineage Exception Record** | Pointer to out-of-policy handling |

---

## 3. Lineage Exception Record — reuse Phase 6

Do **not** create a new exception procedure.

**Data Governance Exception Procedure**

`06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md`

**DMC remains Accountable.** The Lineage Exception Record is a catalog/registry **pointer**, not a second law.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Six proposed artifacts | Section 2 |
| `[C]` | Catalog / Governance domain **names** | Context |
| `[NDMO verification required]` | Whether NDMO mandates these named artifacts | Not claimed |
