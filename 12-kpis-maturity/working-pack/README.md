# Reporting & Analytics — Working Pack

**Document ID:** RHC-DG-P12-WP-000  
**Phase:** 12 — KPIs and maturity (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

This folder is the **applied Reporting & Analytics working pack** inside the existing Rafid Health Cluster Data Governance project. It sits under Phase 12 so the repository numbering stays intact. Locked Phase 12 design files (`01`–`28`) are **not** rewritten.

**No live organizational measurement is claimed unless explicitly supported.**  
**No production Power BI dashboard, live dataset, or automated refresh is claimed.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

Show how Data Governance performance can be:

1. defined through governance KPIs;
2. categorized across the relevant governance areas;
3. assigned owners and measurement frequency;
4. defined with calculation logic and evidence sources;
5. represented through a governance scorecard;
6. evaluated through the existing five-level maturity model;
7. presented through a conceptual governance dashboard structure;
8. prepared for future measurement and review.

This pack **connects** existing Rafid artifacts. It does **not** rebuild Data Quality, ownership, classification, metadata, catalog, lineage, MDM, lifecycle, or NDMO evidence.

```text
Existing Governance Artifacts
          ↓
KPI Definitions
          ↓
Evidence Sources
          ↓
Scorecard
          ↓
Dashboard
          ↓
Governance Review
```

---

## 2. Relationship to existing Phase 12

Phase 12 is the locked **KPI and maturity measurement framework**:

- measurement principles and KPI hierarchy
- twelve measurement domains
- twelve executive KPIs (`DG-KPI-001`–`012`) and eight supporting KPIs (`DG-KPI-013`–`020`)
- five-level maturity model (Initial → Developing → Defined → Managed → Optimized)
- conceptual dashboard specification (four views)
- reporting through existing Phase 3 forums
- target methodology (baseline-first)

This pack is **applied evidence** of how those designs would be used for Reporting & Analytics: definition sheets, evidence-source pointers, a governance scorecard face, dashboard governance, and a reporting workflow.

Locked files remain authoritative for:

- executive KPI IDs and formulas
- the five level **names**
- ten maturity assessment areas
- Phase 3 reporting cadence
- “To be established after baseline measurement.”
- **KPIs inform maturity; they do not automatically determine maturity.**

This pack does **not** replace `01`–`28` in the parent folder. It does **not** invent a new Phase. It does **not** introduce new governance roles or DMC decision rights.

`DG-KPI-00n` identifiers remain fictional Rafid IDs `[A]`. They are **not** NDMO control IDs.

---

## 3. KPI Framework

[`kpi-framework/data-governance-kpi-framework.md`](kpi-framework/data-governance-kpi-framework.md) maps the locked catalogue to eight scorecard areas:

1. Data Quality  
2. Ownership  
3. Classification  
4. Metadata  
5. Lineage  
6. MDM  
7. Lifecycle  
8. Governance Issues / Exceptions  

Related Phase 12 slices (Access / Sharing, Governance operating model, Measurement / Improvement) remain in the definition sheet. They are **not** new operating domains.

The framework reuses Phase 12 formulas. It does **not** create a second KPI catalogue.

---

## 4. KPI Definitions

[`kpi-framework/kpi-definitions.csv`](kpi-framework/kpi-definitions.csv) is the applied definition sheet.

| Set | Count | IDs |
| --- | --- | --- |
| Executive (locked) | 12 | `DG-KPI-001`–`012` |
| Supporting (locked) | 8 | `DG-KPI-013`–`020` |
| Working-pack supporting | 6 | `DG-KPI-WP-001`–`006` |

**26** KPI rows in total. The six working-pack IDs are catalogue-only supporting indicators. They do **not** enter the DMC cover sheet and do **not** swap the locked twelve.

Each row includes: KPI ID, name, governance area, objective, definition, calculation logic, unit, target type, evidence source, owner, frequency, reporting audience, threshold / interpretation, evidence state, status, plus leading/lagging, criticality, and scope where useful.

A formula is **not** a measured result.

---

## 5. Evidence Sources

[`kpi-framework/kpi-evidence-sources.md`](kpi-framework/kpi-evidence-sources.md) points each KPI at existing project artifacts. It does **not** invent source systems.

Examples:

| Area | Evidence source (existing) |
| --- | --- |
| Data Quality | Phase 7 framework and scorecard **structure**; practical-evidence teaching extract |
| Ownership | Phase 4 ownership / stewardship design |
| Classification | Phase 5 classification framework; catalog classification occupancy |
| Metadata | `08-metadata-catalog/working-pack/` |
| Lineage | `09-data-lineage/working-pack/` |
| MDM | Phase 10 MDM design; golden-record teaching example |
| Lifecycle | Phase 11 lifecycle design; catalog lifecycle occupancy |
| Governance Issues | Phase 6 issue / exception procedures; Phase 7 issue path |

---

## 6. Evidence States

This pack uses the same three names as Phase 14 [`05-evidence-status-model.md`](../../14-ndmo-alignment/05-evidence-status-model.md). They are **project evidence states**. They are **not** official NDMO maturity or compliance statuses.

| Project evidence state | Meaning in this pack | Organizational claim |
| --- | --- | --- |
| **Designed** | The KPI, scorecard, maturity model, or dashboard is documented | **Yes** for Phase 12 |
| **Operational** | The artifact has been **applied** inside this synthetic portfolio (working records) | **Not claimed** for a real operating organization |
| **Measured** | Repeatable performance evidence exists (KPI value, quality trend, maturity score) | **Not claimed** |

**KPI definitions in this pack are Designed.** A formula does **not** promote a KPI to Measured.

Metadata and lineage **source** working records may be Operational (project) in the Phase 14 evidence audit. That occupancy is **not** a Rafid KPI result.

**Measured:** not assigned to any KPI, scorecard cell, dashboard tile, or maturity area.

---

## 7. Governance Scorecard

[`scorecard/governance-scorecard.md`](scorecard/governance-scorecard.md) and [`scorecard/scorecard-structure.csv`](scorecard/scorecard-structure.csv) summarize the eight scorecard areas.

This is **not** a second Data Quality Framework. The Phase 7 Data Quality scorecard remains the CDE / dimension monitoring surface ([`../../07-data-quality/11-scorecard-monitoring.md`](../../07-data-quality/11-scorecard-monitoring.md)). This pack **links** to it for the Data Quality row.

Current status for every area: **Not evidenced** (organizational). Measurement readiness: definition complete; baseline not taken. No organizational performance scores are published.

---

## 8. Five-Level Maturity Model

[`maturity/five-level-maturity-model.md`](maturity/five-level-maturity-model.md) applies the **locked** Phase 12 names:

**Level 1 Initial → Level 2 Developing → Level 3 Defined → Level 4 Managed → Level 5 Optimized.**

Ten assessment areas are unchanged. Characteristics are described across Governance, Ownership, Data Quality, Metadata, Lineage, Classification, MDM, Lifecycle, and Measurement / KPIs.

**No Rafid overall maturity score is assigned.**

[`maturity/maturity-assessment-guidance.md`](maturity/maturity-assessment-guidance.md) reuses the six qualitative lenses and the locked statement: KPIs inform maturity; they do not automatically determine it.

Any worked example is labeled **Illustrative assessment only.**

---

## 9. Dashboard Structure

[`dashboard/governance-dashboard-structure.md`](dashboard/governance-dashboard-structure.md) extends the locked four views (Executive, Management, Domain, Operational) with applied sections:

- Executive Summary  
- Data Quality  
- Metadata & Catalog  
- Lineage  
- Ownership  
- Classification  
- MDM  
- Lifecycle  
- Governance Issues  

Tiles that lack evidence display **Not evidenced**. This repository does **not** populate tiles with fake Rafid percentages.

An **illustrative Power BI mapping** is included as a possible presentation layer only. **Power BI is not deployed.** No live dataset is connected. Automated refresh is **not** configured.

---

## 10. Dashboard Governance

[`dashboard/dashboard-governance.md`](dashboard/dashboard-governance.md) defines dashboard owner, KPI owners, data sources, refresh / review frequency, audience, escalation, KPI-input quality checks, and KPI definition change control.

Roles are reused from Phase 3–4. **No new governance roles.** Escalation reuses the existing DMO → CDO → DMC path. KPI changes reuse [`../25-kpi-change-management.md`](../25-kpi-change-management.md).

---

## 11. Reporting Workflow

[`reporting/reporting-workflow.md`](reporting/reporting-workflow.md) records the applied path:

```text
Define KPI
→ Assign Owner
→ Identify Evidence Source
→ Validate Definition
→ Collect / Refresh Data
→ Calculate KPI
→ Quality Check
→ Review
→ Publish Dashboard
→ Escalate Issues
→ Archive / Retain Evidence
```

Cadence reuses Phase 3 forums (weekly DMO huddle; monthly Steward Forum; quarterly DMC). It is **proposed / illustrative** as an operating rhythm for a fictional cluster. It is **not** claimed as operational in a real organization.

---

## 12. KPI Data Quality

The reporting workflow includes a **KPI / reporting quality** section. Governance reporting depends on trustworthy KPI inputs.

Checks: Completeness, Accuracy, Timeliness, Consistency, Validity.

A KPI should **not** be reported as a result if:

- its denominator is undefined;
- source data is missing;
- ownership is unclear;
- calculation logic changed without governance;
- refresh is overdue.

This is **not** a second Data Quality Framework.

---

## 13. MVP Scope

Working examples prioritize the same three domains as the Phase 8 / 9 catalog and lineage MVP:

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Financial / Billing & Claims Data  

The KPI framework may **reference** enterprise governance areas (eight Owner titles; thirteen illustrative CDEs). This pack does **not** expand the Catalog / Lineage MVP. Provider and Facility remain outside Year-1 catalog operating scope except where Encounter depends on them.

---

## 14. Power BI conceptual mapping

See [`dashboard/governance-dashboard-structure.md`](dashboard/governance-dashboard-structure.md) § Power BI.

Wording used: **Conceptual dashboard structure** · **Illustrative Power BI mapping**.

Wording **not** used: production Power BI dashboard; live dataset; automated refresh; measured organizational KPIs.

---

## 15. Limitations

- Synthetic / illustrative / non-production.
- Does not rewrite locked Phase 12 files.
- Does not produce KPI results, baselines, or a Rafid maturity score.
- Does not replace the Phase 7 Data Quality scorecard.
- Does not expand catalog or lineage MVP scope.
- Does not invent retention periods, match-score thresholds, or numeric SLAs.
- Does not deploy Power BI, a semantic model, or a data pipeline.
- Specific NDMO KPI types, formulas, and targets remain `[NDMO verification required]`.

---

## 16. Portfolio disclaimer

This is a fictional portfolio project.

It does **not** claim live organizational measurement, a production BI implementation, a Power BI deployment, real KPI results, a completed maturity assessment, NDMO `DG.7` implementation, NDMO or PDPL compliance, or a real healthcare implementation.

Rafid Health Cluster is fictional.

**Synthetic / Illustrative / Non-production portfolio project.**  
**No live organizational measurement is claimed unless explicitly supported.**

---

## File structure

```text
12-kpis-maturity/working-pack/
├── README.md
├── kpi-framework/
│   ├── data-governance-kpi-framework.md
│   ├── kpi-definitions.csv
│   └── kpi-evidence-sources.md
├── scorecard/
│   ├── governance-scorecard.md
│   └── scorecard-structure.csv
├── maturity/
│   ├── five-level-maturity-model.md
│   └── maturity-assessment-guidance.md
├── dashboard/
│   ├── governance-dashboard-structure.md
│   └── dashboard-governance.md
└── reporting/
    └── reporting-workflow.md
```

---

## Ownership (existing roles only)

No new roles. Responsible / Review / Approval use the Phase 3 catalogue.

| Working-pack artifact | Responsible | Review | Approval (existing rights only) |
| --- | --- | --- | --- |
| Pack method, definition sheet, scorecard, dashboard spec | DMO | CDO | CDO for method; DMC only if an existing policy/exception class is invoked |
| Domain interpretation of a KPI | Data Owner **A** | Business Data Steward **R** | Data Owner **A** (in-policy) |
| Privacy-review occupancy (DG-KPI-010 / 018) | PDPO **A** for the privacy review | DMO (record completeness) | Dual-A unchanged |
| Policy-level exception count (DG-KPI-011) | DMC remains **A** (existing) | DMO register **R** | No new DMC class |

IT / Data Custodian remains technical implementation only. Governance Forum names reused: Data Management Committee, Steward Forum, Domain huddles, DMO operations huddle. Secretariat remains DGO (non-member).
