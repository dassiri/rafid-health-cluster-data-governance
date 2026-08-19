# Phase 10 — Master Data Management

**Document ID:** RHC-DG-P10-000  
**Phase:** 10 — Master data management  
**Status:** Implemented  
**Does not decide:** MDM vendor, matching engine, physical hub, APIs, ETL, or enterprise data lifecycle (Phase 11)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Status

**Implemented** — conceptual **MDM governance framework** for the fictional Rafid Health Cluster `[A]`. No MDM product is implemented. No NDMO compliance is claimed.

This is **not** SAP MDG, Informatica MDM, Reltio, Semarchy, a matching engine, a production API, an MDM database, ETL, machine-learning matching, or technical MDM architecture.

---

## Purpose

Phase 10 defines **how shared business identities are governed** so Patient, Provider, and (lightly) Facility representations stay consistent across processes — without a physical MDM platform.

It consumes Phase 4 ownership, Phase 5 classification **method**, Phase 6 **Master Data Management Standard** (standalone), Phase 7 quality **dimensions**, Phase 8 catalog **hierarchy**, and Phase 9 lineage **as impact context**. It does **not** redesign those phases.

Reference and Master Data Management is an NDMO knowledge-domain **name** `[C]`. This phase is an entity design `[A][B]`. Specific NDMO MDM/master-data requirements remain `[NDMO verification required]`. **Do not claim MDM requirements are NDMO-mandated unless verified.**

---

## MDM lifecycle (locked)

```text
Identify master domain
→ Define master entity
→ Assign ownership
→ Define business rules
→ Identify source systems
→ Define matching requirements
→ Define survivorship principles
→ Create / reconcile master record
→ Distribute trusted representation
→ Monitor quality
→ Resolve conflicts
→ Maintain
→ Retire
```

---

## Master vs Reference vs Transaction

**Master Data** = persistent shared business identity (Patient, Provider, Facility).  
**Reference Data** = controlled code sets (diagnosis codes, claim status, item-type codes).  
**Transaction Data** = events (Encounter, Claim, Payment, Appointment).

Not every reused dataset is Master Data. Candidate criteria are `[B]` / `[A]` application — not NDMO controls.

---

## Master domain assessment (this maturity)

| Class | Domains |
| --- | --- |
| **CORE MDM** | Patient / Person Master; Provider / Clinician Master; Facility / Organization Master |
| **REFERENCE DATA / GOVERNED REFERENCE** | Supply Chain / Item-type; other controlled code sets |
| **NON-MDM AT THIS MATURITY** | HR / Workforce; Financial / Billing & Claims; Quality & Patient Safety |

Reference / Organizational Master **relates to** Facility / Organization Master; it is **not** a second full MDM workstream.

---

## Entity model, golden record, matching, survivorship

Reuses Phase 8 hierarchy. Golden record = **logical/governed** trusted representation — **not** one physical database or platform.

Matching: deterministic, conceptual probabilistic/fuzzy, manual review. **No** prescribed algorithms. **No** numeric thresholds.

Survivorship: **per master domain and attribute**, set by Data Owner and Steward. **No** universal priority order.

---

## Source of truth

Distinguish System of Record, System of Reference, and Master Representation. A system may be authoritative for an **attribute** without being universal for the **entity**.

---

## Ownership and governance

Phase 4 titles only:

| Master | Data Owner |
| --- | --- |
| Patient / Person | Patient Access & Experience Director |
| Provider / Clinician | Medical Affairs Officer |
| Facility / Organization | Strategy & Planning Director |

Steward examples: **Business Data Steward** only.

DMC: *Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework.* **Not** routine approver of every master entity. **No new DMC decision right.**

---

## Quality, reference data, lifecycle, change, integration

Phase 7 dimensions reused (MDM quality = consistency of shared entities across systems). MDM ≠ Reference Data Management; both need governance. Entity lifecycle is **MDM-only** (not Phase 11). Integration is conceptual (DQ, catalog, lineage, classification, ownership, sharing) — no technical architecture.

---

## MDM MVP

**Primary:** Patient / Person; Provider / Clinician.  
**Supporting (lightweight only):** Facility / Organization — facility-code consistency, basic reference alignment, relationship context. **Not** a third full matching/survivorship/golden-record workstream.

Success indicators are **qualitative**.

---

## Governance artifacts `[A]` Proposed Rafid governance artifacts

Master Domain Registry · Master Entity Registry · Attribute Authority Matrix · Matching Rule Register · Survivorship Rule Register · Duplicate Review Register · Master Data Change Record · Master Data Quality Report · Reference Data Register

**Not** claimed as NDMO-mandated. **No additional MDM standards or procedures.**

---

## NDMO verification limitations

Specific NDMO MDM/master-data requirements remain `[NDMO verification required]`.

---

## Boundary with Phase 11

Phase 11 (enterprise Create→Dispose lifecycle) lives in `11-data-lifecycle/`. This Phase 10 folder was **not** redesigned. The MDM entity lifecycle (create → deactivate → retire) is **not** the enterprise data-lifecycle framework. **No MDM-specific retention rules.**

---

## Files

| Path | ID |
| --- | --- |
| [01-framework-overview.md](01-framework-overview.md) | RHC-DG-P10-001 |
| [02-master-reference-transaction.md](02-master-reference-transaction.md) | RHC-DG-P10-002 |
| [03-master-domain-assessment.md](03-master-domain-assessment.md) | RHC-DG-P10-003 |
| [04-master-entity-model.md](04-master-entity-model.md) | RHC-DG-P10-004 |
| [05-golden-record.md](05-golden-record.md) | RHC-DG-P10-005 |
| [06-matching-duplicate-management.md](06-matching-duplicate-management.md) | RHC-DG-P10-006 |
| [07-survivorship.md](07-survivorship.md) | RHC-DG-P10-007 |
| [08-source-of-truth.md](08-source-of-truth.md) | RHC-DG-P10-008 |
| [09-mdm-ownership.md](09-mdm-ownership.md) | RHC-DG-P10-009 |
| [10-mdm-governance.md](10-mdm-governance.md) | RHC-DG-P10-010 |
| [11-master-data-quality.md](11-master-data-quality.md) | RHC-DG-P10-011 |
| [12-reference-data-management.md](12-reference-data-management.md) | RHC-DG-P10-012 |
| [13-master-data-lifecycle.md](13-master-data-lifecycle.md) | RHC-DG-P10-013 |
| [14-mdm-change-management.md](14-mdm-change-management.md) | RHC-DG-P10-014 |
| [15-mdm-integration.md](15-mdm-integration.md) | RHC-DG-P10-015 |
| [16-mdm-mvp.md](16-mdm-mvp.md) | RHC-DG-P10-016 |
| [17-mdm-governance-artifacts.md](17-mdm-governance-artifacts.md) | RHC-DG-P10-017 |
| [18-interview-defensibility.md](18-interview-defensibility.md) | RHC-DG-P10-018 |
| [19-ndmo-alignment.md](19-ndmo-alignment.md) | RHC-DG-P10-019 |
