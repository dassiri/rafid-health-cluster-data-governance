# Data Governance Scorecard (Working Pack)

**Document ID:** RHC-DG-P12-WP-004  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (conceptual scorecard only)

**Does not decide:** Live Rafid scores; a second Data Quality Framework; dashboard software

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Responsible:** DMO (scorecard method) · **Review:** CDO · **Approval:** CDO (method)

**Parent design:** [`../../05-core-kpi-set.md`](../../05-core-kpi-set.md) · Phase 7 [`../../../07-data-quality/11-scorecard-monitoring.md`](../../../07-data-quality/11-scorecard-monitoring.md)

---

## 1. Purpose

This document is the **conceptual Data Governance Scorecard** `[A][B]`. It summarizes Reporting & Analytics status across eight governance areas.

It is **not** a live organizational scorecard. No performance percentages are published as Rafid results.

**Synthetic / Illustrative / Non-production portfolio project.**

---

## 2. Relationship to the Phase 7 Data Quality scorecard

Phase 7 already provides a **CDE / dimension** scorecard structure (Domain, CDE, Dimension, illustrative current score, target, trend, issues, breaches, Owner, status).

This pack does **not** duplicate that surface.

| Scorecard | What it proves | What this pack does |
| --- | --- | --- |
| Phase 7 `11-scorecard-monitoring.md` | How a CDE-dimension row is read; illustrative cells only | **Link** the Data Quality area here to that structure |
| This governance scorecard | Whether each **governance area** has defined KPIs, an owner, a source, and measurement readiness | Summarize eight areas; do not copy CDE rows |

Illustrative Phase 7 cells remain `[A] Illustrative Rafid target` / example values. They are **not** imported as governance performance scores.

---

## 3. Scorecard face (eight areas)

Structure file: [`scorecard-structure.csv`](scorecard-structure.csv).

| Column | Content |
| --- | --- |
| Governance Area | One of the eight Reporting & Analytics areas |
| KPI Count | Executive + supporting + working-pack supporting IDs mapped to the area |
| Evidence State | Designed / Operational (project source only) / Measured — **KPI row state** |
| Current Status | Organizational performance status |
| Measurement Readiness | Whether definition, source, owner, and cadence exist |
| Key Risk / Gap | What would block a defensible result |
| Owner | Existing role (method vs domain **A**) |
| Next Review | Existing Phase 3 forum |

**Current Status** for every area in this drop: **Not evidenced**.

**Evidence State** for every area’s KPIs: **Designed**. Metadata and lineage **sources** may be Operational (project); that does not change Current Status.

---

## 4. Area summary (not Rafid performance)

| Governance Area | KPI Count | KPI IDs | Evidence State | Current Status | Measurement Readiness | Key Risk / Gap | Owner | Next Review |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Data Quality | 3 | DG-KPI-005; DG-KPI-WP-001; DG-KPI-WP-002 | Designed | Not evidenced | Definition complete; baseline not taken. Phase 7 structure exists | Illustrative scorecard cells or the eight-row teaching extract presented as Measured | Data Owner **A** (domain); DMO method | Domain huddle (monthly / by risk); DMC quarterly themes |
| Ownership | 3 | DG-KPI-001; DG-KPI-002; DG-KPI-WP-003 | Designed | Not evidenced | Definition complete; domain titles designed; asset-level source is a teaching inventory | Vacant Owner; treating catalog teaching occupancy as assignment coverage | DMO **R** (registries); Data Owner **A** (Steward acceptance; catalog content) | DMC quarterly; Steward Forum monthly |
| Classification | 1 | DG-KPI-003 | Designed | Not evidenced | Definition complete; Classification Registry not occupied as a live register | Unlabeled datasets treated as Public; Restricted volume used as vanity | Data Owner **A**; DMO registry | Steward Forum monthly; DMC quarterly summary |
| Metadata | 2 | DG-KPI-004; DG-KPI-014 | Designed | Not evidenced | Definition complete; Phase 8 working pack is Operational (project) as a **source** | Publishing assets with incomplete mandatory fields; expanding MVP | Data Owner **A**; DMO method | Steward Forum monthly |
| Lineage | 3 | DG-KPI-007; DG-KPI-015; DG-KPI-WP-004 | Designed | Not evidenced | Definition complete; Phase 9 register is Operational (project) as a **source** | Treating the 13-row register as cluster coverage; scanner vanity | Data Owner **A**; DMO method | Steward Forum monthly; DMC quarterly |
| MDM | 2 | DG-KPI-008; DG-KPI-016 | Designed | Not evidenced | Definition complete; no occupied Master Entity or Duplicate Review register | Match-score KPIs; Facility forced to Core MDM bar | Core MDM Owner **A**; Business Data Steward **R** | Domain huddle monthly |
| Lifecycle | 3 | DG-KPI-009; DG-KPI-017; DG-KPI-WP-005 | Designed | Not evidenced | Definition complete; Retention Schedule not occupied; periods unverified | Briefing coverage as legal retention compliance | Data Owner **A**; DMO register | DMC quarterly |
| Governance Issues | 5 | DG-KPI-006; DG-KPI-011; DG-KPI-012; DG-KPI-019; DG-KPI-WP-006 | Designed | Not evidenced | Definition complete; issue and exception procedures exist; registers not live | Invented SLAs; new DMC class; counting Phase 14 risks as DQ issues | Data Owner **A** (issues); DMC **A** (policy exceptions, existing) | DMO weekly (Critical list); Steward Forum monthly; DMC quarterly |

**KPI count on the face: 22.** Related locked KPIs not on this face: DG-KPI-010, 013, 018, 020 (see framework).

---

## 5. How to read a row

1. **KPI Count** is a catalogue occupancy number, not a performance score.  
2. **Current Status = Not evidenced** means no defensible Rafid result exists.  
3. **Measurement Readiness** can be “definition complete” while Current Status remains Not evidenced.  
4. Do not average the eight areas into “Rafid governance = n%.”  

---

## 6. `[A]` Illustrative reading (not a result)

**Illustrative assessment only.** A reviewer *might* say: “Metadata **definitions** are ready and a synthetic inventory exists, so measurement *could* start on MVP assets; Ownership **titles** are designed but the Ownership Registry is not a working record, so DG-KPI-001 remains not evidenced.”

That sentence is **not** a Rafid scorecard result.

---

## 7. What this scorecard is not

- Not a replacement for Phase 7 CDE monitoring  
- Not a Power BI visual  
- Not NDMO-mandated  
- Not a maturity level  
- Not measured organizational performance  

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Eight-area face | Sections 3–4 |
| Phase 7 scorecard | CDE / dimension structure | Section 2 |
| Phase 12 catalogue | KPI IDs | Section 4 |
