# Phase 9 — Data Lineage Framework

**Document ID:** RHC-DG-P9-000  
**Phase:** 9 — Data lineage  
**Status:** Implemented  
**Does not decide:** Automated lineage tooling, graph databases, ETL build, enterprise-wide column-level lineage, or MDM architecture (Phase 10)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Status

**Implemented** — conceptual **data lineage governance framework** for the fictional Rafid Health Cluster `[A]`. No lineage product is implemented. No NDMO compliance is claimed.

This is **not** Microsoft Purview, Collibra, Informatica, Atlan, automated scanning, or a graph/ETL implementation.

---

## Purpose

Phase 9 defines **how data movement is described, prioritized, validated, and maintained as governed lineage** — without becoming a technical platform.

It consumes Phase 4 ownership, Phase 5 classification **method** (without adding classification rules), Phase 7 quality **concepts** (without a second quality framework), and Phase 8 catalog hierarchy and Lineage Metadata fields. It does **not** redesign those phases.

Lineage is **not** claimed to satisfy any specific regulatory or NDMO specification. Specific NDMO lineage requirements remain `[NDMO verification required]`.

---

## Lineage lifecycle (locked)

```text
Identify lineage scope
→ Identify source
→ Identify movement
→ Identify transformation
→ Identify target
→ Identify consumer
→ Validate lineage
→ Approve lineage
→ Publish lineage
→ Maintain lineage
→ Review lineage
→ Retire lineage
```

---

## Lineage types (locked)

| Type | Year-1 |
| --- | --- |
| **Business Lineage** | Priority |
| **Conceptual Lineage** | Priority |
| **Technical Lineage** | Conceptual only |
| **End-to-End Lineage** | One worked example only |

No enterprise-wide technical lineage.

---

## Lineage model

Reuses Phase 8 hierarchy **exactly**:

```text
Data Domain → Data Asset → Data Structure / Object → Data Element
```

Flow concepts: **Source → Transformation → Target → Consumer**. No parallel object model.

---

## Granularity

Level 1 Business · Level 2 Dataset/Asset · Level 3 Structure/Object · Level 4 Data Element/Field.

Year-1: Levels 1–2 on priority domains; Level 3 only when a CDE or governance issue requires it; Level 4 **selective only**. Field-level lineage is **not** enterprise-wide. **No numeric lineage scoring.**

---

## Criticality (two-step)

> A lineage candidate is identified when one or more criteria indicate material business impact or governance value. The Data Owner, Steward, and DMO then confirm whether prioritized lineage coverage is warranted.

Nine criteria retained. A criterion signals **candidacy**, not automatic Critical Lineage.

---

## Worked example and business lineage

Exactly **one** illustrative end-to-end flow: Patient Registration → Patient Master → Clinical Encounter → Billing / Claims → External Claims Interchange `[A]`. Not real MOH, NPHIES, or Rafid architecture.

One business-lineage example: **Patient Claim Rejection Rate** `[A]` illustrative — not a real organizational metric.

---

## Quality, classification, catalog

- Quality: reuse Phase 7; impact chain from source field to KPI; **no** second DQ framework.
- Classification: lineage **surfaces reassessment**; it does **not** auto-classify or apply a “highest-tier inheritance” rule. Phase 5 remains the sole classification method. Data Owner remains **A**.
- Catalog: lineage supplies Phase 8 Lineage Metadata (upstream source, downstream consumers, transformation reference). Asset-level Source → Target → Consumer may be exposed.

---

## Ownership and workflow

Phase 4 roles unchanged. DMC: escalation **within the approved Phase 3 governance authority and decision-right framework** only — **no new DMC decision class**.

Registration workflow is operating design; **no new Phase 6 procedure** and **no invented document ID**. Exceptions reuse the Phase 6 Data Governance Exception Procedure.

---

## Lineage quality and change

Lineage quality: Completeness, Accuracy, Timeliness, Consistency, Traceability (defined for lineage). Approved change triggers; Steward / Owner / DMO roles as locked.

---

## Governance artifacts (proposed `[A][B]`)

Lineage Registry · Lineage Record · Lineage Change Record · Lineage Review Record · Critical Lineage Register · Lineage Exception Record

**Not** claimed as NDMO-mandated.

---

## MVP

Three domains: Patient / Person Master; Clinical / Medical Records; Financial / Billing & Claims. Two use cases (E2E flow + Claim Rejection Rate). Three initial assets. Focus: **Critical Lineage Register**. Not enterprise-wide.

---

## NDMO verification limitations

Specific lineage requirements remain `[NDMO verification required]`. General governance benefit is not a confirmed regulatory requirement.

---

## Boundary with Phase 10

Phase 10 conceptual MDM lives in `10-master-data-management/`. This Phase 9 folder was **not** redesigned. Master-data **dependency** remains a lineage criticality criterion. Phase 10 does **not** implement a matching engine or hub. Phase 11 conceptual lifecycle lives in `11-data-lifecycle/` and does **not** redesign this folder.

---

## Files

| Path | ID |
| --- | --- |
| [01-framework-overview.md](01-framework-overview.md) | RHC-DG-P9-001 |
| [02-lineage-types.md](02-lineage-types.md) | RHC-DG-P9-002 |
| [03-lineage-model.md](03-lineage-model.md) | RHC-DG-P9-003 |
| [04-granularity-model.md](04-granularity-model.md) | RHC-DG-P9-004 |
| [05-lineage-criticality.md](05-lineage-criticality.md) | RHC-DG-P9-005 |
| [06-worked-example.md](06-worked-example.md) | RHC-DG-P9-006 |
| [07-business-lineage-example.md](07-business-lineage-example.md) | RHC-DG-P9-007 |
| [08-lineage-and-quality.md](08-lineage-and-quality.md) | RHC-DG-P9-008 |
| [09-lineage-and-classification.md](09-lineage-and-classification.md) | RHC-DG-P9-009 |
| [10-lineage-and-catalog.md](10-lineage-and-catalog.md) | RHC-DG-P9-010 |
| [11-lineage-ownership.md](11-lineage-ownership.md) | RHC-DG-P9-011 |
| [12-registration-workflow.md](12-registration-workflow.md) | RHC-DG-P9-012 |
| [13-lineage-quality.md](13-lineage-quality.md) | RHC-DG-P9-013 |
| [14-change-management.md](14-change-management.md) | RHC-DG-P9-014 |
| [15-governance-artifacts.md](15-governance-artifacts.md) | RHC-DG-P9-015 |
| [16-lineage-mvp.md](16-lineage-mvp.md) | RHC-DG-P9-016 |
| [17-interview-defensibility.md](17-interview-defensibility.md) | RHC-DG-P9-017 |
| [18-ndmo-alignment.md](18-ndmo-alignment.md) | RHC-DG-P9-018 |
