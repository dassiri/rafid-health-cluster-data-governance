# Data Quality Framework Overview

**Document ID:** RHC-DG-P7-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]` (DMC informed; DMC **A** for Policy-level exceptions)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 7 framework implementation.

**Phase:** 7 — Data quality  
**Does not decide:** Catalog platform, lineage architecture, MDM matching, live KPIs, or NDMO specification completion

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved **closed-loop data quality framework** for the fictional Rafid Health Cluster `[A]`.

It is a governance operating design `[B]`. It is not a quality-tool configuration, not a measured baseline, and not an NDMO compliance pack.

Trusted Data (high-quality data and transparency about quality) is an NDMO guiding principle **name** `[C]`. Data Quality is an NDMO knowledge-domain **name** `[C]`. Using those names does not complete the national domain. Control- and specification-level NDMO Data Quality requirements remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Closed-loop lifecycle (locked)

```text
Governance
→ Data Quality Dimensions
→ Critical Data Elements
→ Quality Rules
→ Measurement
→ Monitoring
→ Issue Management
→ Root Cause Analysis
→ Remediation
→ Verification
→ Continuous Improvement
```

The loop is **closed**: verification and improvement feed back into dimensions, CDE confirmation, rules, and thresholds. A one-way “measure and forget” dashboard is not this framework `[B]`.

---

## 3. What each stage does

| Stage | Intent | This phase file |
| --- | --- | --- |
| **Governance** | Authority, accountability, and parent Standard/Procedure | This file; [`12-quality-roles.md`](12-quality-roles.md); Phase 6 STD-003 |
| **Data Quality Dimensions** | What “fit for use” means | [`02-quality-dimensions.md`](02-quality-dimensions.md) |
| **Critical Data Elements** | Which fields receive dedicated quality governance | [`03-cde-methodology.md`](03-cde-methodology.md), [`04-cde-catalogue.md`](04-cde-catalogue.md) |
| **Quality Rules** | Testable expectations on CDEs | [`05-quality-rules.md`](05-quality-rules.md) |
| **Measurement** | How conformance is expressed | [`06-thresholds.md`](06-thresholds.md), [`07-quality-scoring.md`](07-quality-scoring.md) |
| **Monitoring** | Who reviews what, at which forum | [`11-scorecard-monitoring.md`](11-scorecard-monitoring.md) |
| **Issue Management** | Defect path from detection to close | [`08-issue-management.md`](08-issue-management.md) |
| **Root Cause Analysis** | Lightweight cause category | [`09-root-cause-analysis.md`](09-root-cause-analysis.md) |
| **Remediation** | Preferred fix patterns; source first | [`10-remediation.md`](10-remediation.md) |
| **Verification** | Confirm the defect is gone or residual is accepted | Issue procedure + Owner close |
| **Continuous Improvement** | Rule, threshold, and CDE confirmation updates | [`14-quality-lifecycle.md`](14-quality-lifecycle.md) |

---

## 4. Parent governance (consumed, not redesigned)

| Source | What Phase 7 uses |
| --- | --- |
| Phase 3 | Federated-by-domain; Steward operational monitoring; Domain Huddle; DMC summarized reporting; no numeric SLAs |
| Phase 4 | Exactly one Data Owner per domain; Owner **A** for quality rules and issue resolution; Steward **R**; Custodian technical; DMO coordinates |
| Phase 5 | Classification remains dataset-level; quality rules do not replace classification |
| Phase 6 POL-001 / STD-003 | Enterprise quality accountability |
| Phase 6 Data Quality Issue Management Procedure | Log → Triage → Assign → Resolve → Verify → Close → Escalate when required |

---

## 5. What this framework is not

- Not a Phase 8 metadata model or catalog product
- Not a Phase 9 lineage framework
- Not a Phase 10 MDM matching / survivorship design
- Not an enterprise-wide single quality score
- Not a claim that Rafid has measured production quality
- Not NDMO compliance

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Phase 7 design; Rafid fiction | Loop, illustrative later files |
| `[B]` | Closed-loop quality governance practice | Structure |
| `[C]` | NDMO Trusted Data principle **name**; Data Quality domain **name** (Standards v1.5) | Alignment names only |
| `[NDMO verification required]` | NDMO quality dimensions, thresholds, CDE rules, scoring, specification IDs | Not invented |
