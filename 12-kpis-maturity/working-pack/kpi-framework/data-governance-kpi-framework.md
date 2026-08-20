# Data Governance KPI Framework (Working Pack)

**Document ID:** RHC-DG-P12-WP-001  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (documentation only)

**Does not decide:** Live Rafid results; a second KPI catalogue; new Data Owner titles; dashboard software

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Responsible:** DMO (method) · **Review:** CDO · **Approval:** CDO (method)

**Parent design:** [`../../04-kpi-catalogue.md`](../../04-kpi-catalogue.md) · [`../../05-core-kpi-set.md`](../../05-core-kpi-set.md) · [`../../03-kpi-domains.md`](../../03-kpi-domains.md)

---

## 1. Purpose

This document is the **applied Data Governance KPI framework** `[A][B]`. It shows how existing Phase 12 KPIs cover eight governance areas used for Reporting & Analytics, how they connect to evidence already in this repository, and how definition, proposed target, and measured result stay distinct.

It does **not** replace the locked catalogue. `DG-KPI-001`–`020` remain authoritative. Working-pack IDs (`DG-KPI-WP-001`–`006`) are supporting only.

**Synthetic / Illustrative / Non-production portfolio project.**

---

## 2. Three distinctions (mandatory)

| Concept | Meaning in this pack |
| --- | --- |
| **KPI definition** | Name, formula, owner, source, frequency — documented here and in the CSV |
| **Proposed target** | Future measurement target. Where no baseline exists: **To be established after baseline measurement.** Teaching numbers are `[A] Illustrative Rafid target` or **Proposed portfolio threshold** |
| **Actual measured result** | Repeatable occupancy or rate with method, period, and Owner — **not claimed** |

A formula is not a result. An illustrative scorecard cell is not a baseline.

---

## 3. Hierarchy (locked — reused)

```text
Strategic Objective
→ Governance Outcome
→ KPI
→ Metric Definition
→ Evidence Source
→ Reporting
→ Decision/Action
```

Source: [`../../02-kpi-hierarchy.md`](../../02-kpi-hierarchy.md).

---

## 4. Eight scorecard areas

The CV-facing Reporting & Analytics surface uses **eight** areas. They are measurement slices of existing Phases 4–11. They are **not** a ninth Data Owner.

| Scorecard area | Locked Phase 12 domain | Typical KPIs | Existing design consumed |
| --- | --- | --- | --- |
| **Data Quality** | Data Quality | DG-KPI-005; DG-KPI-WP-001; DG-KPI-WP-002 | Phase 7 dimensions, 13 CDEs, rules, scorecard structure |
| **Ownership** | Ownership; Stewardship | DG-KPI-001; DG-KPI-002; DG-KPI-WP-003 | Phase 4 eight Owner titles; Business Data Steward |
| **Classification** | Classification | DG-KPI-003 | Phase 5 Public / Internal / Confidential / Restricted |
| **Metadata** | Metadata / Catalog | DG-KPI-004; DG-KPI-014 | Phase 8 mandatory metadata; catalog MVP working pack |
| **Lineage** | Lineage | DG-KPI-007; DG-KPI-015; DG-KPI-WP-004 | Phase 9 Critical Lineage; lineage working pack |
| **MDM** | MDM | DG-KPI-008; DG-KPI-016 | Phase 10 logical golden record; duplicate review |
| **Lifecycle** | Lifecycle | DG-KPI-009; DG-KPI-017; DG-KPI-WP-005 | Phase 11 retention occupancy (no invented periods) |
| **Governance Issues** | Issue / Exception | DG-KPI-006; DG-KPI-011; DG-KPI-012; DG-KPI-019; DG-KPI-WP-006 | Phase 6 issue and exception procedures |

Related Phase 12 slices **not** on the eight-area scorecard face:

| Related slice | KPIs | Why kept |
| --- | --- | --- |
| Access / Sharing | DG-KPI-010; DG-KPI-018 | Dual-A privacy review remains a locked executive KPI |
| Governance operating model | DG-KPI-013 | Forum action closure — not attendance |
| Measurement / Improvement | DG-KPI-020 | Evidence-pack completeness for the executive set |

---

## 5. How CV-style examples map (no duplicate catalogue)

| Example indicator | How this pack treats it |
| --- | --- |
| Critical Data Element Quality Score | **DG-KPI-005** CDE Quality Composite (per-CDE unweighted; no enterprise index) |
| Data Quality Rule Pass Rate | **DG-KPI-WP-002** supporting; Phase 7 rules are designed, not executed as a live pass rate |
| Critical Data Element Completeness | **DG-KPI-WP-001** supporting Completeness dimension; input to DG-KPI-005, not a replacement |
| Percentage of Critical Data Assets with Assigned Owner | **DG-KPI-WP-003** MVP catalog Owner occupancy; **DG-KPI-001** remains domain-title coverage |
| Percentage of Domains with Assigned Steward | **DG-KPI-002** |
| Percentage of Catalog Assets Classified | **DG-KPI-003** (in-scope Datasets) |
| Restricted / Confidential classification occupancy | **Qualitative DMC note** only. Phase 12 forbids a Restricted-volume vanity KPI |
| Metadata Completeness Rate | **DG-KPI-004** |
| Percentage of Priority Assets Registered | **DG-KPI-014** Year-1 catalog publication coverage (MVP cut) |
| Percentage of Critical Assets with Required Lineage | **DG-KPI-007** |
| Percentage of Critical Lineage Records Reviewed | **DG-KPI-WP-004** (forum-cycle review occupancy, not an invented day SLA) |
| Master Data Coverage | **DG-KPI-016** Master Entity Registry occupancy |
| Duplicate / Match Exception Rate | **DG-KPI-008** duplicate **review-case** resolution. **No match-score KPI** |
| Percentage of Priority Assets with Lifecycle Status | **DG-KPI-WP-005** catalog Lifecycle Status occupancy |
| Assets reviewed within required cycle | **DG-KPI-WP-004** for Critical lineage; catalog Last Reviewed is a source field, not a new executive KPI |
| Open Governance Issues | **DG-KPI-011** (exceptions) and **DG-KPI-WP-006** (open DQ issues) |
| Overdue / aging issues | **DG-KPI-012** cycle-based Critical aging. **No invented “close in n days” SLA** |

---

## 6. Calculation pattern `[A][B]`

Keep formulas understandable. Do not invent production volumes.

| Pattern | Example |
| --- | --- |
| Coverage | (Items meeting the control ÷ items in the stated denominator) × 100 |
| Completeness | (Completed required fields ÷ total required fields) × 100 — or (assets with required occupancy ÷ in-scope assets) × 100 |
| Closure | (Closed items in cohort ÷ items in cohort) × 100 — cohort must be stated |
| Stock | Count of open items at period end |
| Aging | Count and age described against **existing Phase 3 forum cycles**, not a fabricated day-count target |

If the denominator is undefined, the KPI is **not evidenced**. It is not reported as 0% and not reported as 100%.

---

## 7. Owners and frequency (summary)

Existing roles only. Full rows: [`kpi-definitions.csv`](kpi-definitions.csv).

| Role | Reporting duty |
| --- | --- |
| **DMO** | Catalogue method, Evidence Register, pack assembly, **R** for assignment-coverage KPIs |
| **CDO** | Oversight; presents executive pack to DMC |
| **Data Owner A** | Domain interpretation, quality rules, classification, catalog content, issue closure, lifecycle occupancy |
| **Business Data Steward R** | Occupancy, validation, domain huddle pack |
| **PDPO A** | Privacy-review completeness for personal-data shares (DG-KPI-010 / 018) — not the business Owner |
| **DMC** | Existing exception **A**; quarterly executive pack oversight. **No new decision right** |
| **IT / Data Custodian** | Technical extracts when a live process exists — **not claimed here** |

Frequency reuses Phase 3: weekly DMO triage; monthly Steward Forum; quarterly DMC.

---

## 8. Targets and thresholds

Locked rule ([`../../16-target-methodology.md`](../../16-target-methodology.md)):

**To be established after baseline measurement.**

| Label | Use |
| --- | --- |
| Future measurement target | Default target type in the CSV |
| Proposed portfolio threshold | Teaching interpretation only — not an organizational target |
| `[A] Illustrative Rafid target` | Any numeric teaching example |

Phase 7 Target / Warning / Breach examples remain **`[A] Illustrative Rafid target`**. This pack does not convert them into claimed Rafid performance.

---

## 9. Evidence state rule

| Condition | Evidence State |
| --- | --- |
| Definition and formula documented | **Designed** |
| Synthetic working register exists as a **source** (catalog inventory, lineage register) | Source may be Operational (project); the **KPI remains Designed** until a repeatable measurement cycle exists |
| Repeatable result with method, date, and Owner | **Measured** — **not assigned** |

Illustrative Phase 7 scorecard cells and `assets/practical-evidence/01-data-quality-example.md` do **not** qualify as Measured.

---

## 10. MVP working examples

When a KPI is interpreted on working records, prioritize:

1. Patient / Person Master Data — Patient Access & Experience Director  
2. Clinical / Medical Records Data — Chief Medical Officer (CMO)  
3. Financial / Billing & Claims Data — Chief Financial Officer (CFO)  

Enterprise assignment KPIs (DG-KPI-001 / 002) still count the **eight** Phase 4 domains. That is the locked catalogue. This pack does not shrink those denominators to the catalog MVP.

---

## 11. What this framework is not

- Not a second Data Quality Framework  
- Not an enterprise-wide single quality index  
- Not a match-algorithm scorecard  
- Not legal retention compliance  
- Not NDMO `DG.7` implemented  
- Not live Rafid performance  

---

## 12. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Applied eight-area face; WP supporting IDs | Entire document |
| Phase 12 locked files | Formulas, executive set, cadence | Sections 3–8 |
| `[C]` | `DG.7` Performance Management **name** as Phase 2 pointer | Context only |
| `[NDMO verification required]` | Official NDMO KPI types and formulas | Not claimed |
