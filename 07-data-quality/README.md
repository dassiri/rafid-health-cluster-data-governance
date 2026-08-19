# Phase 7 — Data Quality Framework

**Document ID:** RHC-DG-P7-000  
**Phase:** 7 — Data quality  
**Status:** Implemented  
**Does not decide:** Metadata/catalog design (Phase 8), technical lineage (Phase 9), MDM matching or survivorship (Phase 10), live measurement, or named tool implementation

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Status

**Implemented** — the data quality **framework** for the fictional Rafid Health Cluster `[A]` is documented. No live scorecard, no measured Rafid performance, and no NDMO compliance are claimed.

---

## Purpose

Phase 7 defines **how data quality is governed**: dimensions, Critical Data Elements (CDEs), representative rules, illustrative thresholds, conceptual scoring, issue management integration, root-cause and remediation patterns, monitoring, roles, and proposed artifacts.

It consumes:

- Phase 3 federated-by-domain forums (Steward operational monitoring, Domain Huddle, DMC summarized reporting)
- Phase 4 ownership (one Data Owner per domain; Steward operational; Custodian technical; DMO coordination)
- Phase 6 **Data Quality Standard** and **Data Quality Issue Management Procedure**

It does **not** redesign those phases.

Trusted Data is an NDMO guiding principle **name** `[C]`. Data Quality is an NDMO knowledge-domain **name** `[C]`. This phase is an entity framework `[A][B]`. It is **not** a completed NDMO Data Quality domain implementation. Specification-level NDMO quality requirements remain `[NDMO verification required]`. **No compliance is claimed. No NDMO control IDs are invented.**

---

## Framework overview

Closed loop `[A][B]`:

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

Detail: [`01-framework-overview.md`](01-framework-overview.md).

---

## Seven dimensions `[A][B]`

These are **Rafid design choices**, not claimed as NDMO-required dimension names.

| Group | Dimensions |
| --- | --- |
| **Baseline (every CDE)** | Accuracy, Completeness, Validity |
| **CDE-dependent** | Timeliness, Uniqueness, Consistency, Integrity |

Exact NDMO Data Quality dimensions: `[NDMO verification required]`.

---

## CDE methodology

A **Critical Data Element** is a specific data field whose quality has a material impact on areas such as patient safety, regulatory compliance, financial integrity, operational continuity, decision-making, privacy/security, cross-domain dependency, or executive reporting `[A][B]`.

**No numeric CDE scoring.**

Decision logic (locked):

> A CDE candidate is identified when one or more selection criteria indicate material business impact. The Data Owner and Steward then confirm whether dedicated CDE governance is warranted.

---

## Quality rules

Representative rule library only. Examples include **DQ-001** (National ID uniqueness) and **DQ-002** (diagnosis code validity). Not hundreds of rules. All examples are illustrative `[A]`.

---

## Thresholds

Each measured rule uses **Target / Warning / Breach**. Numeric examples are **`[A] Illustrative Rafid target`**. They are not NDMO requirements, not regulatory requirements, and not real Rafid performance.

Thresholds may vary by CDE criticality, domain, business impact, lifecycle stage, and confirmed regulatory context `[NDMO verification required]` where a regulator is asserted.

---

## Scoring

Per-dimension metrics (for example Completeness %, Validity %, Accuracy %, Timeliness %, Uniqueness %). An optional CDE-level composite may be described conceptually. **No** enterprise-wide single score. **No** arbitrary weighting system. Formula/design choices are `[A]`.

---

## Issue management

Operational issues follow the Phase 6 procedure by **title and path**:

**Data Quality Issue Management Procedure** — `06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

(That file also records Document ID **RHC-DG-PRC-003**.)

Severity model: Critical / High / Medium / Low `[A][B]`. No numeric SLAs.

---

## Roles (Phase 4 — not redesigned)

| Role | Quality role |
| --- | --- |
| Data Owner | **A** for business quality outcomes |
| Business Data Steward | **R** for operational quality management |
| IT Data Steward / Custodian | Technical remediation |
| DMO | Framework ownership and registry oversight |
| DMC | Governance escalation and decisions |
| PDPO | **C** where issues have personal-data / privacy implications |

---

## Governance artifacts (proposed `[A][B]`)

CDE Registry · Data Quality Rule Registry · Data Quality Issue Register · Scorecard · Quality Review · Exception Record · Trend Reporting

**Not** claimed as NDMO-mandated.

---

## Relationship to Phase 6

| Phase 6 | Phase 7 |
| --- | --- |
| STD-003 — who is accountable; issue governance expectations | Dimensions, CDEs, rules, measurement, monitoring design |
| Data Quality Issue Management Procedure | Same issue path, with severity, RCA, and remediation patterns added |

Phase 6 documents are **not** rewritten by this phase.

---

## Boundary with Phase 8

Phase 8 metadata and conceptual catalog design lives in `08-metadata-catalog/`. This Phase 7 folder was **not** redesigned. CDE business definitions remain quality-governance content; catalog registration remains STD-004 / the Metadata Registration Procedure / Phase 8 operating design. **No catalog product** is implemented.

Lineage remains conceptual in Phase 7/8 quality-catalog integration; the **lineage framework** is Phase 9 (`09-data-lineage/`). This Phase 7 folder was **not** redesigned. MDM conceptual design lives in Phase 10 (`10-master-data-management/`) — Designed / Documented; operational implementation and measured performance are not claimed.

---

## NDMO verification limitations

The following remain `[NDMO verification required]`:

- Specific NDMO Data Quality dimensions
- Specific NDMO thresholds
- Specific CDE requirements
- Specific NDMO scoring requirements
- Specification-level Data Quality control/specification IDs (not invented here)

---

## Files

| Path | ID |
| --- | --- |
| [01-framework-overview.md](01-framework-overview.md) | RHC-DG-P7-001 |
| [02-quality-dimensions.md](02-quality-dimensions.md) | RHC-DG-P7-002 |
| [03-cde-methodology.md](03-cde-methodology.md) | RHC-DG-P7-003 |
| [04-cde-catalogue.md](04-cde-catalogue.md) | RHC-DG-P7-004 |
| [05-quality-rules.md](05-quality-rules.md) | RHC-DG-P7-005 |
| [06-thresholds.md](06-thresholds.md) | RHC-DG-P7-006 |
| [07-quality-scoring.md](07-quality-scoring.md) | RHC-DG-P7-007 |
| [08-issue-management.md](08-issue-management.md) | RHC-DG-P7-008 |
| [09-root-cause-analysis.md](09-root-cause-analysis.md) | RHC-DG-P7-009 |
| [10-remediation.md](10-remediation.md) | RHC-DG-P7-010 |
| [11-scorecard-monitoring.md](11-scorecard-monitoring.md) | RHC-DG-P7-011 |
| [12-quality-roles.md](12-quality-roles.md) | RHC-DG-P7-012 |
| [13-domain-priorities.md](13-domain-priorities.md) | RHC-DG-P7-013 |
| [14-quality-lifecycle.md](14-quality-lifecycle.md) | RHC-DG-P7-014 |
| [15-governance-controls.md](15-governance-controls.md) | RHC-DG-P7-015 |
| [16-interview-defensibility.md](16-interview-defensibility.md) | RHC-DG-P7-016 |
| [17-ndmo-alignment.md](17-ndmo-alignment.md) | RHC-DG-P7-017 |
