# Interview Defensibility — Data Quality

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P7-016  
**Phase:** 7 — Data quality  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## What makes a data element critical?

A **Critical Data Element** is a **field** whose quality has **material impact** on patient safety, regulatory compliance, financial integrity, operational continuity, decision-making, privacy/security, cross-domain dependency, or executive reporting `[A][B]`.

Identification is **two steps**, not automatic:

> A CDE candidate is identified when one or more selection criteria indicate material business impact. The Data Owner and Steward then confirm whether dedicated CDE governance is warranted.

There is **no numeric CDE score**. One criterion does **not** auto-qualify the field.

---

## Why use multiple quality dimensions?

Fitness for use fails in different ways `[B]`. A National ID can be present (complete) but duplicated (uniqueness) or malformed (validity). Rafid uses **seven** dimensions `[A][B]`: Accuracy, Completeness, Validity (baseline on every CDE); Timeliness, Uniqueness, Consistency, Integrity (CDE-dependent).

These names are **not** briefed as NDMO-required dimensions `[NDMO verification required]`.

---

## How are thresholds established?

Three levels: **Target / Warning / Breach** `[A][B]`. The Data Owner is Accountable for the business target on that CDE rule. Numbers in this repo are **`[A] Illustrative Rafid target`** — not NDMO, not regulation, not measured Rafid performance.

Thresholds **may vary** by CDE criticality, domain, business impact, lifecycle stage, and **confirmed** regulatory context. Unverified “the regulator requires 99%” is `[NDMO verification required]`.

---

## Who owns data quality?

**Data Owner = Accountable** for business quality outcomes (Phase 4). **Business Data Steward = Responsible** for operational quality management. **Custodian** does technical remediation. **DMO** owns the framework and registries, not the domain. **DMC** handles escalation and Policy exceptions. **PDPO is Consulted** when personal-data/privacy implications exist — PDPO is not the quality Owner.

IT is never business Owner.

---

## What happens when quality fails?

Follow **Data Quality Issue Management Procedure**:

`06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

```text
Issue detected → Log → Triage → Severity → Assign Owner/Steward → Root Cause → Remediation → Verification → Closure → Trend Analysis
```

Severity: Critical / High / Medium / Low `[A][B]`. **Close = Data Owner A**. Escalate qualitatively (Phase 3) — **no numeric SLA**.

---

## Why fix the source?

If only the report is patched, the source keeps generating the defect `[B]`. Preferred approaches: correct the record **and** correct the source where practical; then validation, transformation, reference data, process, training, or governance change. Downstream-only patches need visible residual risk. Out-of-policy residual → exception procedure, **DMC = A**.

---

## How is data quality measured?

**Per-dimension** metrics (Completeness %, Validity %, Accuracy % when a comparison exists, Timeliness %, Uniqueness % or duplicate counts) `[A]`. Optional **CDE composite** is conceptual, unweighted, and must not hide a critical failure. **No** enterprise-wide single score. **No** arbitrary weighting model.

Scorecard columns: Domain, CDE, Dimension, Current score, Target, Trend, Open issues, Breaches, Owner, Status. Example numbers in the repo are **illustrative**, not Rafid results.

---

## How do you avoid thousands of rules?

Govern **13 illustrative CDEs**, not every field. Baseline three dimensions on each CDE; add dependents only when material. Keep a **representative** rule library (DQ-001, DQ-002, and a handful more). Domain **priorities** that are not CDEs stay watch-items. That is how documentation stays manageable `[B]`.

---

## How are quality problems prioritized?

1. CDE confirmation (material impact + Owner/Steward warrant dedicated governance).  
2. Issue **severity** Critical → Low `[A][B]`.  
3. Forum altitude: Steward operational → Domain Huddle → DMC summary — Phase 3 cadence, no numeric SLAs.  
4. Patient-safety and identity defects outrank cosmetic completeness on non-CDE fields.

---

## Must-nots

| Do not say | Say instead |
| --- | --- |
| “These seven dimensions are NDMO’s.” | Rafid `[A][B]`; NDMO dimensions `[NDMO verification required]`. |
| “Any safety-related field is automatically a CDE.” | Candidate, then Owner/Steward confirmation. |
| “Our completeness is 98%.” | Illustrative target only unless you have a live measurement. |
| “We completed NDMO Data Quality.” | Framework documented; no specification evidenced; **no compliance claim**. |
| “PRC-003 is the quality framework.” | Phase 6 is the **issue path**; Phase 7 is dimensions/CDEs/rules/measurement. |
| “We built Purview/Collibra for quality.” | Phase 8 is Designed / Documented as conceptual catalog design; this is not a catalog implementation. |
