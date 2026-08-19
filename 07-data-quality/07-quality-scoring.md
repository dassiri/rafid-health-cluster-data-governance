# Quality Scoring

**Document ID:** RHC-DG-P7-007  
**Version:** 1.0  
**Status:** Implemented (conceptual scoring only)  
**Owner:** DMO (method) `[B]`; Data Owner **A** for interpretation of domain scores  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Per-dimension metrics; optional CDE composite conceptual only; no enterprise score.

**Phase:** 7 — Data quality  
**Does not decide:** Weighted enterprise index; live Rafid scores; NDMO scoring method `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records **how quality is expressed as a metric** for the fictional Rafid Health Cluster `[A]`.

It is conceptual. It does **not** publish measured Rafid performance. Any formula below is a **Rafid design choice** `[A]`. Specific NDMO scoring requirements remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Per-dimension metrics (locked approach) `[A][B]`

Report quality **by dimension** for a CDE (or for a rule that tests that dimension):

| Metric | Typical use |
| --- | --- |
| Completeness % | Baseline; DQ-003, DQ-006 style rules |
| Validity % | Baseline; DQ-002, DQ-007 style rules |
| Accuracy % | Baseline; used when a trusted comparison source exists — not faked if no comparison exists |
| Timeliness % | CDE-dependent; DQ-004 style rules (or a count converted to a percentage only if the denominator is defined) |
| Uniqueness % | CDE-dependent; DQ-001, DQ-005 style rules (or duplicate-group counts) |

**Consistency** and **Integrity** may be reported as a percentage of records satisfying the relationship, or as an exception count. Do not invent a third scoring family.

---

## 3. Conceptual formulas `[A]`

These formulas are **Rafid design choices**. They are not NDMO-mandated.

**Completeness %** `[A]`

```text
Completeness % = (in-scope records with the CDE present or valid exception)
                 / (in-scope records)
                 × 100
```

**Validity %** `[A]`

```text
Validity % = (in-scope records whose CDE value conforms to the agreed constraint)
             / (in-scope records with a value present)
             × 100
```

**Accuracy %** `[A]`

```text
Accuracy % = (sampled or matched records whose CDE value matches the agreed real-world or trusted source)
             / (records in the accuracy sample)
             × 100
```

If no trusted comparison exists, **do not invent Accuracy %**. Record “not yet measurable” and keep Accuracy as a baseline dimension with a qualitative control (for example registration verification process).

**Timeliness %** `[A]` (only if a time condition is defined)

```text
Timeliness % = (in-scope events meeting the time condition)
               / (in-scope events)
               × 100
```

**Uniqueness %** `[A]` (optional expression)

```text
Uniqueness % = (distinct real-world entities correctly represented once)
               / (distinct real-world entities in scope)
               × 100
```

Duplicate-group **counts** are acceptable and often clearer than Uniqueness %.

---

## 4. Optional CDE-level composite (conceptual only) `[A]`

A Data Owner **may** view a simple CDE composite as the **unweighted average of the dimensions that apply to that CDE** (baseline always; dependents only if confirmed).

This optional composite is:

- Conceptual
- Per CDE
- **Not** mandatory
- **Not** an enterprise-wide single score
- **Not** an arbitrary weighting system
- **Not** a complex scoring model

**Forbidden in this phase:**

- One cluster-wide quality number
- Secret weights (for example “safety × 5”)
- Scoring that hides a Critical uniqueness failure behind a high completeness average

If a composite would mask a baseline or safety-critical dependent failure, **do not use the composite** for DMC reporting; show the failing dimension `[B]`.

---

## 5. What is reported where

| Audience | Score content |
| --- | --- |
| Steward | Rule-level dimension metrics and exception lists |
| Domain Huddle | CDE dimension metrics vs illustrative thresholds; open issues |
| DMC | Summarized themes and breaches — **not** a fake enterprise index |

Cadence is Phase 3 conceptual (operational / huddle / quarterly committee). **No numeric SLAs.**

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Formulas; optional unweighted CDE composite; prohibitions | Sections 3–4 |
| `[B]` | Per-dimension reporting; do not mask failures | Design |
| `[C]` | Trusted Data principle **name** (transparency about quality) | Why scores are shown, not hidden |
| `[NDMO verification required]` | Official NDMO scoring / index requirements | Not claimed |
