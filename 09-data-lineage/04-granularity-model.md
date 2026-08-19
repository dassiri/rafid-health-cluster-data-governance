# Lineage Granularity Model

**Document ID:** RHC-DG-P9-004  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (granularity method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Four levels; Year-1 selective field-level; no scoring.

**Phase:** 9 — Data lineage  
**Does not decide:** Enterprise column-level graphs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **how deep** lineage is drawn `[A][B]`.

There is **no numeric lineage scoring model**.

---

## 2. Four levels (locked)

| Level | Name | Typical content |
| --- | --- | --- |
| **Level 1** | Business | KPI, process, or business question and its supporting terms |
| **Level 2** | Dataset / Asset | Catalog assets and system context |
| **Level 3** | Structure / Object | Table/file/object inside an asset |
| **Level 4** | Data Element / Field | Named fields (selective) |

---

## 3. Year-1 approach (locked)

| Level | Year-1 |
| --- | --- |
| Level 1 | **Priority-domain KPIs** (illustrative: Claim Rejection Rate) |
| Level 2 | **Priority-domain assets** (MVP assets) |
| Level 3 | **Only when** a specific CDE or governance issue requires it |
| Level 4 | **Selective only** |

**Field-level lineage is not required enterprise-wide.**

---

## 4. When Level 4 may be warranted `[B]`

Field-level (selective) lineage may be warranted for:

- **CDE-related root-cause analysis** (Phase 7)
- **Classification reassessment** (Phase 5 method — lineage only surfaces the question)
- **Specific audit/investigation needs**

Warrant does **not** auto-expand to all fields in the domain. Owner, Steward, and DMO still apply the criticality two-step for **prioritized coverage**.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Four levels and Year-1 cut | Sections 2–4 |
| `[C]` | Quality / Classification domain **names** | Why Level 4 can be justified |
| `[NDMO verification required]` | Official NDMO granularity mandates | Not claimed |
