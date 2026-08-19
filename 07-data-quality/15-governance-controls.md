# Quality Governance Artifacts and Controls

**Document ID:** RHC-DG-P7-015  
**Version:** 1.0  
**Status:** Implemented (proposed artifacts only)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Proposed Rafid artifacts; not claimed as NDMO-mandated.

**Phase:** 7 — Data quality  
**Does not decide:** Tool schemas; Phase 8 catalog; live registers populated with production data

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records **proposed Rafid quality-governance artifacts** `[A][B]`.

They are entity design. They are **not** claimed as NDMO-mandated registers `[NDMO verification required]`. **No compliance is claimed. No NDMO control IDs are invented.**

Phase 6 already indexes a Data Quality Issue Record as a supporting template. This phase **names** the quality set; it does not build detailed future-phase schemas.

---

## 2. Proposed artifacts (locked list)

| Artifact `[A][B]` | Purpose | Owner of content | DMO role |
| --- | --- | --- | --- |
| **CDE Registry** | List of confirmed CDEs (this drop: the 13 illustrative rows as the starting design) | Data Owner **A** per domain row | Method and oversight |
| **Data Quality Rule Registry** | Representative rules (DQ-001 …) | Data Owner **A** per rule | Method and oversight |
| **Data Quality Issue Register** | Issues from the Phase 6 procedure | Data Owner **A** for close | Routing visibility |
| **Scorecard** | Domain / CDE / dimension monitoring view | Data Owner **A** for domain truth | Pack coordination |
| **Quality Review** | Domain Huddle / Steward Forum review record | Steward **R**; Owner **A** for decisions | Cadence oversight |
| **Exception Record** | Residual quality risk or out-of-policy handling pointer | Owner **A** in-policy residual; **DMC A** if Policy exception | Register hygiene |
| **Trend Reporting** | Recurring defects and direction of scores (qualitative + illustrative metrics) | Steward **R**; DMO for cross-domain themes | DMC summary support |

---

## 3. Minimum content (governance-level, not a physical schema)

### CDE Registry

CDE ID, field name, domain, Owner, Steward, criteria notes, baseline dimensions (always), dependent dimensions confirmed or N/A, status (candidate / confirmed / retired), `[A]` illustrative vs live.

### Data Quality Rule Registry

The approved rule structure in [`05-quality-rules.md`](05-quality-rules.md).

### Data Quality Issue Register

Align to Phase 6 Data Quality Issue Record: identity of issue, domain, CDE/rule if known, severity `[A][B]`, assignment, RCA category, remediation approach, verification, close (Owner **A**), escalation.

Path of the governing procedure:

`06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

### Scorecard

Columns in [`11-scorecard-monitoring.md`](11-scorecard-monitoring.md).

### Quality Review

Date, forum (Domain Huddle / Steward Forum / DMC summary), decisions, actions. No numeric SLA.

### Exception Record

Link to in-policy residual on the issue register **or** to the Policy Exception Register when the Data Governance Exception Procedure applies (**DMC = A**).

### Trend Reporting

By domain and CDE: direction, open Critical/High issues, repeated RCA categories. Not a Phase 12 maturity score.

---

## 4. Control statements (entity, not NDMO IDs) `[A][B]`

1. Confirmed CDEs are visible in the CDE Registry.
2. Measured rules are visible in the Rule Registry.
3. Fitness-for-use defects are visible in the Issue Register — not only in email.
4. Scorecard values used in forums are labeled illustrative until a live measurement process exists.
5. No second quality procedure besides the Phase 6 path.

These are **Rafid proposed controls**. They are not NDMO specification IDs.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Seven proposed artifacts | Section 2 |
| `[C]` | Data Quality domain **name**; Trusted Data principle **name** | Why registers exist conceptually |
| `[NDMO verification required]` | Whether NDMO mandates these named artifacts | Not claimed |
