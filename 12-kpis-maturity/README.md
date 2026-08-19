# Phase 12 — KPIs and Maturity

**Document ID:** RHC-DG-P12-000  
**Phase:** 12 — KPIs and maturity  
**Status:** Implemented  
**Does not decide:** Live Rafid performance, NDMO assessment scores, dashboard software, BI tooling, data pipelines, technical architecture, or the implementation roadmap (Phase 13)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## Status

**Implemented** — conceptual **KPI and maturity measurement framework** for the fictional Rafid Health Cluster `[A]`. No KPI value, target, maturity level, or performance result is presented as real Rafid data. No NDMO or legal compliance is claimed.

This is **not** a dashboard product, a BI implementation, an NDMO annual assessment, or a live scorecard.

**KPI IDs such as `DG-KPI-001` are fictional Rafid identifiers `[A]`. They are not NDMO control IDs.** They must never be briefed as `DG.7` specifications.

---

## Purpose

Phase 12 defines **how data governance is measured and how maturity is assessed** — without inventing performance, without new DMC decision rights, and without redesigning Phases 3–11.

It consumes Phase 1 objectives (direction only), Phase 3 forums and authority, Phase 4 ownership, Phase 5 classification, Phase 6 sharing/exception procedures, Phase 7 quality dimensions and conceptual scoring, Phase 8 mandatory metadata, Phase 9 Critical Lineage, Phase 10 conceptual MDM, and Phase 11 lifecycle registers. It does **not** redesign those phases.

NDMO names Performance Management as a Data Governance control **theme** in the Phase 2 map `[C]` (`DG.7` as already recorded). That **name** is not a verified KPI catalogue. Specific NDMO KPI types, formulas, and targets remain `[NDMO verification required]`. Phase 12 **does not** claim `DG.7` is implemented.

---

## Measurement principles `[A][B]`

Outcome-focused · Evidence-based · Proportionate · Owner-accountable · No vanity metrics · No invented live results · KPIs inform maturity; they do **not** automatically determine maturity

---

## KPI hierarchy (locked)

```text
Strategic Objective
→ Governance Outcome
→ KPI
→ Metric Definition
→ Evidence Source
→ Reporting
→ Decision/Action
```

---

## KPI domains (12) `[A]`

Mapped to existing Phases 3–11 (plus this measurement layer). Not new operating domains and **not** a ninth Data Owner.

1. Governance operating model (Phase 3)  
2. Ownership (Phase 4)  
3. Stewardship (Phase 4)  
4. Classification (Phase 5)  
5. Access / Sharing (Phase 4 / 6)  
6. Issue / Exception (Phase 6 / 7)  
7. Data Quality (Phase 7)  
8. Metadata / Catalog (Phase 8)  
9. Lineage (Phase 9)  
10. MDM (Phase 10)  
11. Lifecycle (Phase 11)  
12. Measurement / Improvement (this phase)

---

## Executive KPI set (locked — 12)

| ID | Name |
| --- | --- |
| DG-KPI-001 | Data Owner Assignment Coverage |
| DG-KPI-002 | Business Data Steward Assignment Coverage |
| DG-KPI-003 | Classification Coverage Rate |
| DG-KPI-004 | Mandatory Metadata Completeness |
| DG-KPI-005 | CDE Quality Composite |
| DG-KPI-006 | Data Quality Issue Closure Rate |
| DG-KPI-007 | Critical Lineage Coverage |
| DG-KPI-008 | Master Data Duplicate Resolution Rate |
| DG-KPI-009 | Retention Schedule Coverage |
| DG-KPI-010 | Sharing Requests with Completed Privacy Review |
| DG-KPI-011 | Open Governance Exceptions |
| DG-KPI-012 | Critical Issue Aging |

All twelve are fictional Rafid IDs `[A]`. **Not** NDMO control IDs.

---

## Targets

Where no baseline exists, use exactly:

**To be established after baseline measurement.**

Any illustrative numerical target is labeled **`[A] Illustrative Rafid target`** and is **not** real Rafid performance and **not** an NDMO mandate.

---

## Reporting cadence

Reuse Phase 3 forums only:

| Forum | Frequency (Phase 3) | KPI use |
| --- | --- | --- |
| DMO operations huddle | Weekly | Intake / routing; **no** policy |
| Domain huddles | Biweekly or monthly by domain risk | Domain metrics |
| Steward Forum | Monthly | Cross-domain pack |
| Data Management Committee | Quarterly + extraordinary | Executive pack |

DMC: *Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework.* **No new DMC decision right.**

---

## Maturity model (locked)

Five levels: **Initial → Developing → Defined → Managed → Optimized**.

Ten assessment areas: Governance, Ownership, Classification, Data Quality, Metadata, Lineage, MDM, Lifecycle, Access/Sharing, Measurement/Improvement.

**KPIs inform maturity; they do not automatically determine maturity.**

Any worked score is `[A] Illustrative assessment method` and **not** an actual Rafid maturity result.

---

## NDMO verification limitations

Specific NDMO performance-management, KPI-type, target, and maturity requirements remain `[NDMO verification required]`.  
This framework is **not** the NDMO annual specification-level self-assessment (Phase 14).  
No legal compliance is claimed. No retention periods are invented.

---

## Boundary with Phase 13

Phase 13 is implemented as an `[A]` Illustrative Implementation Roadmap. It is documentation/design only; operational implementation and measured performance are not claimed. This phase sets **no** multi-year initiative calendar and does **not** treat `DG.1.3` as complete.

---

## Files

| Path | ID |
| --- | --- |
| [01-measurement-principles.md](01-measurement-principles.md) | RHC-DG-P12-001 |
| [02-kpi-hierarchy.md](02-kpi-hierarchy.md) | RHC-DG-P12-002 |
| [03-kpi-domains.md](03-kpi-domains.md) | RHC-DG-P12-003 |
| [04-kpi-catalogue.md](04-kpi-catalogue.md) | RHC-DG-P12-004 |
| [05-core-kpi-set.md](05-core-kpi-set.md) | RHC-DG-P12-005 |
| [06-data-quality-kpis.md](06-data-quality-kpis.md) | RHC-DG-P12-006 |
| [07-metadata-catalog-kpis.md](07-metadata-catalog-kpis.md) | RHC-DG-P12-007 |
| [08-lineage-kpis.md](08-lineage-kpis.md) | RHC-DG-P12-008 |
| [09-mdm-kpis.md](09-mdm-kpis.md) | RHC-DG-P12-009 |
| [10-lifecycle-kpis.md](10-lifecycle-kpis.md) | RHC-DG-P12-010 |
| [11-ownership-stewardship-kpis.md](11-ownership-stewardship-kpis.md) | RHC-DG-P12-011 |
| [12-classification-kpis.md](12-classification-kpis.md) | RHC-DG-P12-012 |
| [13-access-sharing-kpis.md](13-access-sharing-kpis.md) | RHC-DG-P12-013 |
| [14-issue-exception-kpis.md](14-issue-exception-kpis.md) | RHC-DG-P12-014 |
| [15-leading-lagging-indicators.md](15-leading-lagging-indicators.md) | RHC-DG-P12-015 |
| [16-target-methodology.md](16-target-methodology.md) | RHC-DG-P12-016 |
| [17-kpi-data-sources.md](17-kpi-data-sources.md) | RHC-DG-P12-017 |
| [18-kpi-reporting.md](18-kpi-reporting.md) | RHC-DG-P12-018 |
| [19-governance-dashboard-spec.md](19-governance-dashboard-spec.md) | RHC-DG-P12-019 |
| [20-maturity-model.md](20-maturity-model.md) | RHC-DG-P12-020 |
| [21-maturity-assessment-method.md](21-maturity-assessment-method.md) | RHC-DG-P12-021 |
| [22-kpi-maturity-link.md](22-kpi-maturity-link.md) | RHC-DG-P12-022 |
| [23-maturity-assessment-output.md](23-maturity-assessment-output.md) | RHC-DG-P12-023 |
| [24-governance-review.md](24-governance-review.md) | RHC-DG-P12-024 |
| [25-kpi-change-management.md](25-kpi-change-management.md) | RHC-DG-P12-025 |
| [26-governance-artifacts.md](26-governance-artifacts.md) | RHC-DG-P12-026 |
| [27-interview-defensibility.md](27-interview-defensibility.md) | RHC-DG-P12-027 |
| [28-ndmo-alignment.md](28-ndmo-alignment.md) | RHC-DG-P12-028 |
