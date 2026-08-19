# Data Quality Dimensions

**Document ID:** RHC-DG-P7-002  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Seven-dimension model; baseline vs CDE-dependent split locked.

**Phase:** 7 — Data quality  
**Does not decide:** NDMO official dimension names; numeric targets (see thresholds file); catalog attributes (Phase 8)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **seven Rafid data quality dimensions** and how they apply to Critical Data Elements `[A][B]`.

These dimension names are **Rafid design choices**. They are **not** claimed as NDMO-required dimension names. Exact NDMO Data Quality dimension requirements remain `[NDMO verification required]`. **No compliance is claimed. No NDMO control IDs are used.**

---

## 2. The seven dimensions (locked)

| # | Dimension | Meaning (working definition `[A][B]`) |
| --- | --- | --- |
| 1 | **Accuracy** | The value correctly represents the real-world fact it is meant to represent. |
| 2 | **Completeness** | A required value is present for in-scope records. |
| 3 | **Validity** | The value conforms to an agreed format, code list, or business constraint. |
| 4 | **Timeliness** | The value is available and current within the time the business use requires. |
| 5 | **Uniqueness** | The same real-world entity is not represented by conflicting duplicate keys in the governed population. |
| 6 | **Consistency** | The same fact does not conflict across agreed sources or representations in scope. |
| 7 | **Integrity** | Required relationships hold (for example a code exists in the reference list; a child record points to a valid parent). |

Working definitions are entity language `[A][B]`. They are not official NDMO glossary text `[NDMO verification required]`.

---

## 3. Baseline vs CDE-dependent (locked) `[A][B]`

| Group | Dimensions | Application |
| --- | --- | --- |
| **Baseline** | Accuracy, Completeness, Validity | Apply to **every** confirmed CDE. |
| **CDE-dependent** | Timeliness, Uniqueness, Consistency, Integrity | Apply **only** where the Owner and Steward confirm the dimension is material for that CDE. |

**Do not** treat all seven dimensions as mandatory on every field. That would recreate an unmanageable rule factory `[B]`.

**Do not** drop Accuracy, Completeness, or Validity from a confirmed CDE. If a baseline dimension cannot yet be measured, record that gap; do not pretend the dimension does not apply.

---

## 4. How dimensions relate to rules and scoring

- A **quality rule** tests **one** CDE against **one** dimension (see [`05-quality-rules.md`](05-quality-rules.md)).
- A **threshold** is set per rule, not as a single enterprise number (see [`06-thresholds.md`](06-thresholds.md)).
- A **score** is reported per dimension (and optionally, conceptually, per CDE). There is **no** enterprise-wide single score (see [`07-quality-scoring.md`](07-quality-scoring.md)).

---

## 5. What this file does not do

- It does not list NDMO specification-level quality criteria.
- It does not invent additional Rafid dimensions (for example “usability” or “believability”) beyond the locked seven.
- It does not set numeric targets.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 7 dimension set and baseline/dependent split | Sections 2–3 |
| `[C]` | Data Quality knowledge-domain **name**; Trusted Data principle **name** | Why quality is in the program |
| `[NDMO verification required]` | Official NDMO dimension names, definitions, and mandates | Not resolved |
