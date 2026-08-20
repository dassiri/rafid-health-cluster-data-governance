# Governance Dashboard Structure (Working Pack)

**Document ID:** RHC-DG-P12-WP-008  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (conceptual specification only)

**Does not decide:** Tool vendor, cloud BI, refresh pipelines, UX, or live tiles

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Responsible:** DMO (specification) · **Review:** CDO · **Approval:** CDO (method)

**Parent design:** [`../../19-governance-dashboard-spec.md`](../../19-governance-dashboard-spec.md)

---

## 1. Purpose

This document is a **conceptual dashboard structure** `[A][B]` for future measurement and review.

**Not software. Not a production Power BI dashboard. Not a live dataset. Not automated refresh.**

It extends the locked four views (Executive, Management, Domain, Operational) with applied sections that match the eight scorecard areas.

**Synthetic / Illustrative / Non-production portfolio project.**

---

## 2. Locked views (reused)

| View | Audience | Content |
| --- | --- | --- |
| **Executive** | DMC (quarterly) | DG-KPI-001–012 as status tiles **when evidenced**; narrative for not-evidenced; exception count; Critical aging theme |
| **Management** | CDO / DMO | Executive set plus DG-KPI-013–020 and WP supporting IDs; evidence pointers |
| **Domain** | Data Owner + Business Data Steward | Domain filter for quality, catalog, issues, classification; eight Owner titles only |
| **Operational** | Custodian / Steward | Issue lists; duplicate review queue; metadata gaps |

No view publishes a **cluster-wide quality index**. No view treats backup jobs as retention.

---

## 3. Tile behaviour (locked — reused)

| State | Display |
| --- | --- |
| Evidenced | Value + period + source (when a live process exists — **not claimed in this drop**) |
| Not evidenced | Explicit **Not evidenced** |
| Illustrative only | Label **`[A] Illustrative Rafid target`** if a teaching number is shown |

This repository **does not** populate tiles with fake Rafid percentages.

---

## 4. Applied sections `[A]`

Each section below is a **layout specification**. Tiles default to **Not evidenced**.

### 4.1 Executive Summary

| Component | Intent | Typical KPIs / inputs |
| --- | --- | --- |
| Overall governance status | Qualitative: Designed / not evidenced — **not** a composite score | DG-KPI-020; scorecard Current Status |
| Key governance risks | Residual risks visible to DMC | DG-KPI-011; DG-KPI-012; Phase 14 risk pointers as context only |
| Priority gaps | Measurement readiness vs occupancy | Scorecard Key Risk / Gap |
| Major trends | Improving / stable / worsening **when a time series exists** | Not claimed. Do not invent a trend |

### 4.2 Data Quality

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Quality KPIs | CDE status distribution — not “Rafid quality = n%” | DG-KPI-005 |
| CDE coverage | Completeness and rule pass **when evidenced** | DG-KPI-WP-001; DG-KPI-WP-002 |
| Quality exceptions | Open stock, closure, Critical aging | DG-KPI-WP-006; DG-KPI-006; DG-KPI-012 |

Drill-through: Phase 7 CDE / dimension scorecard structure. Do not copy illustrative cells as live tiles.

Working examples (MVP): CDE-001 National ID; CDE-002 Patient ID; CDE-003 Diagnosis code; CDE-007 Claim identifier.

### 4.3 Metadata & Catalog

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Registration coverage | Year-1 publication in MVP cut | DG-KPI-014 |
| Metadata completeness | Mandatory field occupancy | DG-KPI-004 |
| Certification / review status | Catalog approval / last reviewed as **qualitative** until measured | Phase 8 catalog status fields — not a new executive KPI |

MVP domains only. Do not expand catalog MVP.

### 4.4 Lineage

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Critical lineage coverage | Confirmed Critical items registered | DG-KPI-007 |
| Review status | Forum-cycle Last Reviewed occupancy | DG-KPI-WP-004 |
| High-priority lineage gaps | Incomplete coarse fields | DG-KPI-015 |

Do not show “% interfaces scanned.”

### 4.5 Ownership

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Asset ownership coverage | MVP catalog Owner occupancy | DG-KPI-WP-003 |
| Stewardship coverage | Domain Steward assignment | DG-KPI-002 |
| Domain Owner assignment | Eight titles | DG-KPI-001 |

### 4.6 Classification

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Classification coverage | In-scope Datasets with Owner-approved tier | DG-KPI-003 |
| Unclassified priority assets | Qualitative list / count of unlabeled in-scope assets | Supporting view of the DG-KPI-003 denominator — **not** a Restricted-volume vanity KPI |

Distribution by tier may appear as a **qualitative** DMC note.

### 4.7 MDM

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Master data coverage | Patient / Provider registry occupancy | DG-KPI-016 |
| Exceptions | Duplicate review-case resolution | DG-KPI-008 |

No match-score tile. Facility remains supporting-only.

### 4.8 Lifecycle

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Lifecycle coverage | Catalog Lifecycle Status occupancy; Retention Rule registration | DG-KPI-WP-005; DG-KPI-009 |
| Review / retirement status | Disposal evidence completeness; qualitative hold note | DG-KPI-017 |

Do not tile “years retained” as compliance.

### 4.9 Governance Issues

| Component | Intent | Typical KPIs |
| --- | --- | --- |
| Open issues | DQ stock; policy exception stock | DG-KPI-WP-006; DG-KPI-011 |
| Aging | Critical forum-cycle aging | DG-KPI-012 |
| Closure status | DQ issue closure; exception review occupancy | DG-KPI-006; DG-KPI-019 |

---

## 5. Illustrative Power BI mapping

**Illustrative Power BI mapping. Power BI is not deployed.**  
No live dataset is connected. Automated refresh is **not** configured. Real organizational KPIs are **not** measured.

| Power BI object (illustrative) | Maps to | Claim |
| --- | --- | --- |
| Workspace “Rafid Data Governance” `[A]` | Conceptual container | Not created |
| Semantic model / dataset | KPI Evidence Register + source registers | Not connected |
| Page: Executive | §4.1 | Conceptual dashboard structure |
| Page: Data Quality | §4.2 | Conceptual |
| Page: Metadata & Catalog | §4.3 | Conceptual |
| Page: Lineage | §4.4 | Conceptual |
| Page: Ownership | §4.5 | Conceptual |
| Page: Classification | §4.6 | Conceptual |
| Page: MDM | §4.7 | Conceptual |
| Page: Lifecycle | §4.8 | Conceptual |
| Page: Governance Issues | §4.9 | Conceptual |
| Row-level security | Domain filter by Data Owner title | Not implemented |
| Scheduled refresh | Dashboard governance refresh frequency | **Not configured** |

If a future teaching screenshot is added, it must show **Not evidenced** tiles or be labelled `[A] Illustrative Rafid target`. It must **not** be briefed as a production dashboard.

Purview / Tableau / Looker mappings are equally illustrative and **not** deployed (same rule as Phase 8–9 tool mappings).

---

## 6. What the dashboard is not

- Not NDMO-mandated  
- Not a data pipeline  
- Not a cluster-wide quality index  
- Not a maturity score visual  
- Not evidence of `DG.7` implementation  

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Applied sections; illustrative Power BI mapping | Sections 4–5 |
| Phase 12 dashboard spec | Four views; tile behaviour | Sections 2–3 |
| `[NDMO verification required]` | Official NDMO dashboard requirements | Not claimed |
