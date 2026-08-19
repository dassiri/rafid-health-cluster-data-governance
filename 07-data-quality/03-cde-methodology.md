# Critical Data Element Methodology

**Document ID:** RHC-DG-P7-003  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Qualitative CDE method; corrected two-step decision logic; no numeric scoring.

**Phase:** 7 — Data quality  
**Does not decide:** Live CDE inventory beyond the 13 illustrative examples; NDMO-mandated CDE lists `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records **how** Rafid identifies a Critical Data Element (CDE) `[A][B]`.

It does not score candidates numerically. It does not publish a live production inventory. Specific NDMO CDE requirements remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Approved CDE definition (locked)

A **Critical Data Element** is a specific data **field** whose quality has a material impact on areas such as patient safety, regulatory compliance, financial integrity, operational continuity, decision-making, privacy/security, cross-domain dependency, or executive reporting `[A][B]`.

A CDE is **not**:

- An entire domain
- An entire dataset (datasets are classified in Phase 5)
- A report or dashboard
- A system name

---

## 3. Eight qualitative selection criteria (locked) `[A][B]`

A candidate is assessed against:

1. **Patient safety impact**
2. **Regulatory impact**
3. **Financial impact**
4. **Operational impact**
5. **Decision-making impact**
6. **Privacy/security impact**
7. **Cross-domain dependency**
8. **Executive reporting importance**

Criteria are **qualitative**. There is **no** points model, weight, or passing score.

---

## 4. Decision logic (locked — two steps)

**Withdrawn wording:** any suggestion that a single criterion **automatically** qualifies an element as a CDE is **not** used.

**Approved wording:**

> A CDE candidate is identified when one or more selection criteria indicate material business impact. The Data Owner and Steward then confirm whether dedicated CDE governance is warranted.

| Step | Who | What happens |
| --- | --- | --- |
| 1. Identify candidate | Business Data Steward (with consumers / Custodian as needed) | Record which criteria show **material** impact. One or more criteria may fire. That **identifies a candidate**. It does **not** auto-confirm a CDE. |
| 2. Confirm CDE | Data Owner **A**, Steward **R** | Decide whether **dedicated CDE governance** (baseline dimensions, rules, monitoring, issue path) is warranted **now**. |

If Step 2 is “not now,” the field may still be governed as ordinary domain data. Quality issues still follow the Phase 6 issue procedure. The field is simply not in the CDE Registry.

DMO checks method consistency. DMO does **not** become Data Owner of the field.

---

## 5. What “dedicated CDE governance” means `[B]`

For a confirmed CDE:

- Baseline dimensions (Accuracy, Completeness, Validity) apply
- CDE-dependent dimensions are confirmed or explicitly marked not applicable
- At least one representative quality rule is designed or scheduled
- The CDE is listed in the CDE Registry
- Issues on that CDE use the Phase 6 issue procedure with quality severity

---

## 6. Ownership (Phase 4 — not redesigned)

| Role | CDE decision |
| --- | --- |
| Data Owner | **A** — confirms or declines CDE status for fields in that domain |
| Business Data Steward | **R** — proposes candidates, documents criteria, maintains registry content |
| IT Data Steward / Custodian | **C** on measurability / source location; never **A** for CDE confirmation |
| DMO | Method owner; registry oversight; not business Owner |
| PDPO | **C** when privacy/security impact or personal data is material |
| DMC | Escalation if Owner non-participation or cross-domain deadlock |

This is the Phase 4 quality-rules / issue-resolution pattern applied to CDE confirmation. No new RACI row is invented.

---

## 7. What this file does not do

- No numeric CDE scoring
- No automatic CDE from a single criterion
- No requirement that every domain field become a CDE
- No claim that NDMO mandates this 13-CDE list `[NDMO verification required]`

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 7 CDE definition, eight criteria, two-step logic | Sections 2–4 |
| `[C]` | Data Quality domain **name**; Trusted Data principle **name** | Context |
| `[NDMO verification required]` | Whether NDMO specifies CDE identification method or lists | Not claimed |
