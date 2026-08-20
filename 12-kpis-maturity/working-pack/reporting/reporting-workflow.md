# Reporting Workflow (Working Pack)

**Document ID:** RHC-DG-P12-WP-010  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (documentation only)

**Does not decide:** Ticket tooling; a KPI committee; live refresh; numeric SLAs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Responsible:** DMO (workflow method) · **Review:** CDO · **Approval:** CDO (method)

**Parent design:** [`../../16-target-methodology.md`](../../16-target-methodology.md) · [`../../18-kpi-reporting.md`](../../18-kpi-reporting.md) · [`../../25-kpi-change-management.md`](../../25-kpi-change-management.md) · Phase 3 forums

---

## 1. Purpose

Record a practical Reporting & Analytics workflow using **existing** Rafid roles and forums.

This cadence is **proposed / illustrative** for the fictional cluster. It is **not** claimed as operational in a real organization.

**Synthetic / Illustrative / Non-production portfolio project.**

---

## 2. Workflow

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

| Step | Activity | Actor (existing roles) | Output |
| --- | --- | --- | --- |
| **1. Define KPI** | Name, objective, formula, unit, scope, inclusion/exclusion | DMO method; requestor | Catalogue / definition-sheet row |
| **2. Assign Owner** | Method vs domain **A**; Steward **R** | CDO (method); Data Owner **A** (domain); PDPO **A** where privacy review | Owner fields on the sheet |
| **3. Identify Evidence Source** | Point at an existing register — do not invent a system | DMO; Business Data Steward **R** | Evidence Register pointer |
| **4. Validate Definition** | Formula does not redesign Phases 4–11; ID is Rafid not NDMO; vanity test | DMO; Data Owner **C** if domain KPI | Validated / rejected |
| **5. Collect / Refresh Data** | Occupancy extract for the stated cohort and period | Business Data Steward **R**; Custodian (technical, when a live process exists — not claimed) | Source extract or **not evidenced** |
| **6. Calculate KPI** | Apply locked logic only | DMO method; Steward validates occupancy | Value **or** explicit Not evidenced |
| **7. Quality Check** | KPI-input checks in §4 | DMO; Steward **R**; Owner **A** for domain meaning | Pass / fail (fail ⇒ do not publish as Evidenced) |
| **8. Review** | Existing forums only | Domain huddle; Steward Forum; CDO | Pack comments; actions |
| **9. Publish Dashboard** | Executive / management / domain / operational views | DMO assembles; CDO presents executive pack | Conceptual dashboard / DMC pack. Tiles: Evidenced or Not evidenced |
| **10. Escalate Issues** | Existing path only | DMO huddle → Owner / Steward Forum → CDO → DMC (existing classes) | Issue, exception, or residual-risk note |
| **11. Archive / Retain Evidence** | Keep definition, source pointer, quality-check outcome, pack version | DMO | Evidence pack occupancy (proposed artifact). Retention period **not invented** `[Legal / regulatory verification required]` |

Steps 1–4 may complete while 5–7 remain **not evidenced**. That is the current portfolio state.

---

## 3. Reporting cadence

**Do not invent a new governance cadence.** Reuse Phase 3.

| Review type | Forum | Frequency (Phase 3) | Content |
| --- | --- | --- | --- |
| **Operational / working review** | DMO operations huddle | Weekly | Intake, routing, Critical list — **no** policy |
| **Operational / working review** | Steward Forum | Monthly | Full operational pack including supporting and WP KPIs |
| **Governance / domain review** | Domain huddles | Biweekly or monthly by domain risk | Domain slice; Owner **A** |
| **Governance / executive review** | Data Management Committee | Quarterly + extraordinary | Executive 12-KPI pack; exception and Critical aging themes |

If a shorter label is needed in interviews:

- Operational / Working Review: **Monthly** (Steward Forum) plus weekly DMO triage  
- Governance Review: **Quarterly** (DMC) and domain huddles as Phase 3  
- Executive Review: **Quarterly** DMC, or extraordinary as already defined  

Those labels describe the **existing** Phase 3 design. They are **not** a live operating rhythm.

DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework. **No new DMC decision right.**

---

## 4. KPI data quality

Governance reporting depends on trustworthy **KPI inputs**. This is KPI / reporting quality. It is **not** a second Data Quality Framework.

Reuse Phase 7 dimension **names** only as checks on the metric itself `[A][B]`:

| Check | Meaning for a KPI |
| --- | --- |
| **Completeness** | Numerator and denominator are populated or explicitly not evidenced; required Owner and source pointer exist |
| **Accuracy** | Calculation matches the locked formula; cohort is the one stated on the sheet |
| **Timeliness** | Extract period matches the forum pack; refresh is not overdue |
| **Consistency** | Same denominator rules as the last published period unless a governed change was recorded |
| **Validity** | Unit, scope, and inclusion/exclusion match the catalogue; Rafid ID is not briefed as an NDMO ID |

### Do not report the KPI as Evidenced if

- the denominator is undefined;
- source data is missing;
- ownership is unclear;
- calculation logic changed without governance;
- refresh is overdue.

Failed checks produce **Not evidenced** (and an issue/exception on the existing path if warranted). They do **not** produce a fabricated 0% or 100%.

DG-KPI-005 still must not hide a baseline dimension breach. A “green” composite tile that masks Completeness failure fails this section.

---

## 5. Pack rules (reused)

- No live numbers in this documentation drop.  
- If evidence is missing, say **not evidenced**.  
- Do not present DG-KPI-005 as a single cluster quality index.  
- Do not present DG-KPI-009 as legal retention compliance.  
- Do not present teaching inventory occupancy as a Rafid KPI result.  
- Do not fill empty tiles to make the dashboard look live.

---

## 6. Target handling in the workflow

After a defensible baseline exists (not claimed):

```text
Define KPI
→ Identify evidence source
→ Measure baseline (when data exist)
→ Propose target
→ Owner acceptance for domain KPIs
→ Record on Definition Sheet
→ Review with the KPI (Phase 3 forums)
```

Until then, Target Status remains exactly:

**To be established after baseline measurement.**

---

## 7. What this workflow is not

- A production analytics operating model  
- An NDMO-mandated reporting procedure `[NDMO verification required]`  
- Automatic maturity scoring after publish  

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Eleven-step path; KPI-input quality | Sections 2, 4 |
| Phase 3 | Forums and frequencies | Section 3 |
| Phase 12 target / reporting / change files | Locked rules | Sections 5–6 |
