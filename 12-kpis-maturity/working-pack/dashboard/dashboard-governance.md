# Dashboard Governance (Working Pack)

**Document ID:** RHC-DG-P12-WP-009  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (documentation only)

**Does not decide:** A new dashboard Owner role; BI admin rights; a new DMC class

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Responsible:** DMO (dashboard method) · **Review:** CDO · **Approval:** CDO (method)

**Parent design:** [`../../18-kpi-reporting.md`](../../18-kpi-reporting.md) · [`../../24-governance-review.md`](../../24-governance-review.md) · [`../../25-kpi-change-management.md`](../../25-kpi-change-management.md) · Phase 3 role catalogue

---

## 1. Purpose

Govern the **conceptual** governance dashboard the same way other Rafid artifacts are governed: owner, sources, cadence, audience, quality checks, and change control.

**No new governance roles.**  
**No new DMC decision right.**  
The dashboard is not software in this drop.

---

## 2. Dashboard Owner

| Element | Existing role |
| --- | --- |
| **Dashboard Owner (method / specification)** | DMO **R**; CDO oversight (**A** for KPI reporting method — Phase 3 RACI: KPI reporting CDO **A**, DMO **R**) |
| **Does not own domain meaning** | Data Owner remains **A** for domain interpretation of domain tiles |
| **Does not chair DMC** | Cluster CEO chairs; CDO presents the pack |

There is no “Dashboard Product Owner” title. Do not invent one.

---

## 3. KPI Owners

Reuse the definition sheet. Summary:

| KPI class | Accountable / Responsible |
| --- | --- |
| Assignment coverage (DG-KPI-001 / 002) | DMO **R**; CDO oversight |
| Domain content (quality, classification, catalog, lineage, MDM, lifecycle, DQ issues) | Data Owner **A**; Business Data Steward **R** |
| Privacy-review occupancy (DG-KPI-010 / 018) | PDPO **A** for the review; Data Owner **A** for business approval; DMO record completeness |
| Policy exceptions (DG-KPI-011 / 019) | DMC remains **A** for Policy-level exceptions (existing); DMO register **R** |
| Evidence-pack completeness (DG-KPI-020) | DMO **R** |

IT / Data Custodian supplies technical extracts **if** a live process exists — **not claimed**.

---

## 4. Data sources

Sources are the existing registers listed in [`../kpi-framework/kpi-evidence-sources.md`](../kpi-framework/kpi-evidence-sources.md). The dashboard does **not** become a second system of record.

| Rule | Application |
| --- | --- |
| Catalogue is the definition | Tile calculation must match `kpi-definitions.csv` |
| Empty source ⇒ Not evidenced | Never display 0% or 100% as a substitute |
| Illustrative cells stay labelled | Phase 7 teaching numbers are not executive tiles |

---

## 5. Refresh frequency `[A]` Proposed / illustrative cadence

Not operational in a real organization. Reuses Phase 3 intensity; does not invent a KPI committee.

| Layer | Proposed refresh (design) | Claim |
| --- | --- | --- |
| Operational lists (Critical aging, issue stock) | Align to **weekly** DMO operations huddle | Not live |
| Domain / Steward pack | Align to **monthly** Steward Forum (domain huddles biweekly or monthly by risk) | Not live |
| Executive tiles | Align to **quarterly** DMC pack | Not live |

If refresh is overdue, tiles display **Not evidenced** (or last evidenced period with an overdue flag) — they are not silently reused as current.

---

## 6. Review frequency

Reuse [`../../24-governance-review.md`](../../24-governance-review.md):

| Item | Forum | Frequency |
| --- | --- | --- |
| Executive 12-KPI pack | DMC | Quarterly + extraordinary |
| Operational / supporting pack | Steward Forum | Monthly |
| Domain slice | Domain huddles | Biweekly or monthly by domain risk |
| Critical aging list | DMO operations huddle | Weekly |
| Maturity narrative | DMC when CDO tables it | Within quarterly pack |
| Dashboard specification change | CDO (method); Data Owner **A** if domain meaning changes | With the KPI change process |

---

## 7. Audience

```text
Executive / DMC
→ Governance Management (CDO / DMO)
→ Domain Owners / Stewards
→ Operational Teams
```

Year-1 DMC standing members who see the executive page remain those in Phase 3–4 (including Patient, Clinical, and Financial Owners). Other Owners by invitation when relevant.

---

## 8. Escalation path (existing)

```text
DMO operations huddle (routing — no policy)
→ Domain huddle / Steward Forum (Owner A / recommendations)
→ CDO
→ Data Management Committee (existing classes only)
→ Cluster CEO as DMC Chair (unresolved strategic / material risk)
```

Material patient-safety or regulatory data incidents already have an extraordinary DMC path. This dashboard does not add a class.

Policy conflicts use the existing **Data Governance Exception Procedure**.

---

## 9. Data quality checks (KPI inputs)

Before a tile is published as **Evidenced**, DMO (method) and the Business Data Steward **R** confirm the checks in [`../reporting/reporting-workflow.md`](../reporting/reporting-workflow.md) § KPI data quality.

Minimum: denominator defined; source present; owner clear; formula unchanged (or changed under governance); refresh not overdue.

Failed check ⇒ **Not evidenced**, plus an issue or exception on the existing path if warranted.

---

## 10. Change control and KPI definition change process

Reuse the locked chain in [`../../25-kpi-change-management.md`](../../25-kpi-change-management.md):

```text
Proposed → Defined → Validated → Approved under existing authority
→ Implemented → Reviewed → Retired
```

| Change type | Who |
| --- | --- |
| Tile layout / section order (no formula change) | DMO **R**; CDO accepts method |
| KPI formula, denominator, or ID | Full KPI change process; CDO for catalogue/method; Data Owner **A** for domain interpretation |
| Executive set swap | Keep cover sheet between 10 and 15; CDO; DMC **I** |
| Out-of-Policy measurement | Existing exception **A** (DMC) — no new A |
| Tool mapping (e.g. illustrative Power BI page names) | DMO method; **not** a production deployment approval |

Record occupancy on the proposed **KPI Change Record** (Phase 12 artifact). Working-pack IDs `DG-KPI-WP-*` stay off the DMC cover sheet unless swapped under that process.

---

## 11. What dashboard governance is not

- A BI Centre of Excellence as a new Rafid role  
- An NDMO-mandated dashboard control `[NDMO verification required]`  
- Approval of fake results to fill empty tiles  

---

## 12. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Applied dashboard RACI on existing roles | Entire document |
| Phase 3 RACI / forums | Owner, cadence, escalation | Sections 2, 5–8 |
| Phase 12 change management | KPI definition changes | Section 10 |
