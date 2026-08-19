# Metadata Quality

**Document ID:** RHC-DG-P8-008  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Business Data Steward **R**; Data Owner **A** for accepting residual metadata-quality risk on domain assets  
**Approver:** CDO `[B]` (method)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Metadata quality distinct from Phase 7 data quality; no second DQ framework.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Metadata-quality scorecards with numeric targets; a parallel issue procedure

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Two questions (locked)

| Concept | Question |
| --- | --- |
| **Data Quality** | Is the **data itself** correct? (Phase 7) |
| **Metadata Quality** | Is the **description of the data** correct, complete, current, and governed? (this file) |

Do **not** create a second Data Quality Framework. Do **not** copy Phase 7 CDE catalogues, thresholds, or scorecards into metadata.

Trusted Data includes transparency about quality as an NDMO principle **name** `[C]`. That does not merge the two questions.

---

## 2. Illustrative metadata-quality checks `[A][B]`

Phase 7 dimension **names** are reused **only** as metadata-quality application:

| Check (Phase 7 name) | Applied to metadata |
| --- | --- |
| **Completeness** | Mandatory fields and mandatory categories are present |
| **Accuracy** | Description and definition match Owner-accepted meaning |
| **Consistency** | Owner, domain, and glossary links do not contradict other governed records |
| **Timeliness** | Record is current relative to known change (qualitative — **no numeric SLA**) |
| **Validity** | Classification is a Rafid tier; status is one of the five trust statuses; asset type is a Year-1 type |

Uniqueness and Integrity remain Phase 7 **data** dimensions. They are not added as extra metadata-quality frameworks here.

---

## 3. What happens when metadata is poor

| Defect | Path |
| --- | --- |
| Missing mandatory metadata | Steward completes registration workflow; DMO check fails publish until mandatory is present |
| Wrong business meaning | Owner **A**; not IT rewrite |
| Fitness-for-use of the **data** | Data Quality Issue Management Procedure (Phase 6/7) — not this file |
| Inability to meet Policy/Standard | Data Governance Exception Procedure (**DMC = A**) |

---

## 4. What this file does not do

- No metadata completeness % targets
- No enterprise metadata score
- No second CDE method
- No claim that NDMO mandates these five metadata checks `[NDMO verification required]`

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Two-question split; five illustrative checks | Sections 1–2 |
| `[C]` | Trusted Data principle **name**; Data Quality and Catalog domain **names** | Context |
| `[NDMO verification required]` | Official NDMO metadata-quality specifications | Not claimed |
