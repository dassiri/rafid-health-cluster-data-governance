# Matching and Duplicate Management

**Document ID:** RHC-DG-P10-006  
**Version:** 1.0  
**Status:** Implemented (conceptual only)  
**Owner:** Data Owner **A** for match **intent** and merge/split decisions; Steward **R** operationally  
**Approver:** CDO `[B]` (framework)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual matching; no algorithms; no numeric thresholds.

**Phase:** 10 — Master data management  
**Does not decide:** Match scores, vendor matchers, ML models

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records a **conceptual matching framework** `[A][B]`.

**Do not prescribe exact matching algorithms.**  
**Do not create numeric matching thresholds.**

Duplicates remain **data issues** under the existing **Data Quality Issue Management Procedure**:

`06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

---

## 2. Three methods (locked)

| # | Method | Year-1 use |
| --- | --- | --- |
| 1 | **Deterministic matching** | Same strong identifier (for example same National ID in the governed population) — **concept**, not a coded rule engine |
| 2 | **Probabilistic / fuzzy matching** | **Conceptual only** — possible name/DOB similarity; **no** weights, **no** score cut-offs |
| 3 | **Manual review** | Required when deterministic is inconclusive or fuzzy is only a **hint** |

Facility matching **engine** is **not** in MVP supporting scope.

---

## 3. Matching considerations (illustrative, not algorithms) `[A]`

**Patient**

- National ID where applicable  
- Date of birth  
- Name  
- Contact details  

**Provider**

- Provider identifier  
- License information  
- Name  
- Specialty  

**Facility** (context only — no separate Facility matcher program)

- Facility identifier  
- Facility name  
- Location  

These lists are **considerations**. They are not a match formula.

---

## 4. Risks and handling `[B]`

| Risk | Meaning | Handling |
| --- | --- | --- |
| **False positive** | Two different people/providers treated as one | Patient-safety / credentialing harm; **manual review**; Owner oversight; do not auto-merge |
| **False negative** | Same person/provider left as duplicates | Fragmented history, duplicate claims risk; issue path; Steward chase |
| **Manual review** | Human Steward (with Custodian facts) decides propose-merge | Owner **A** for business merge/split **intent** |
| **Exception handling** | Out-of-policy merge | **Data Governance Exception Procedure** — `06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md` (**DMC = A**, existing right) |
| **Data Owner oversight** | Owner accepts residual duplicate risk or requires merge | Phase 4 issue-resolution **A** |

No numeric “match confidence ≥ x%.”

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Consideration lists | Section 3 |
| `[B]` | Three methods; FP/FN | Sections 2, 4 |
| `[C]` | Data Quality domain **name** (duplicates as quality issues) | Context |
| `[NDMO verification required]` | Official NDMO matching mandates | Not claimed |
