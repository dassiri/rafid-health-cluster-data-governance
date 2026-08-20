# Interview Preparation

**INTERNAL / INTERVIEW PREPARATION**

This file is **not** an organizational policy, Standard, or NDMO artifact.

**Document ID:** RHC-DG-DOC-001  
**Audience:** Candidate using this repository in a Data Governance interview  
**Status:** Phases 0–14: Designed / Documented. Operational implementation = Not claimed. Measured performance = Not claimed. NDMO compliance = Not claimed. Phase 14 is the final alignment/evidence phase.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

Phase-specific interview notes remain **in their phase folders** (not moved) so existing links stay valid. They are internal preparation, not policy.

| Phase | Internal notes |
| --- | --- |
| 3 | [`../03-operating-model/08-interview-defensibility-notes.md`](../03-operating-model/08-interview-defensibility-notes.md) |
| 4 | [`../04-ownership-stewardship/09-interview-defensibility.md`](../04-ownership-stewardship/09-interview-defensibility.md) |
| 5 | [`../05-data-classification/11-interview-defensibility.md`](../05-data-classification/11-interview-defensibility.md) |
| 6 | [`../06-policies-standards-procedures/interview-preparation.md`](../06-policies-standards-procedures/interview-preparation.md) |
| 7 | [`../07-data-quality/16-interview-defensibility.md`](../07-data-quality/16-interview-defensibility.md) |
| 8 | [`../08-metadata-catalog/16-interview-defensibility.md`](../08-metadata-catalog/16-interview-defensibility.md) |
| 9 | [`../09-data-lineage/17-interview-defensibility.md`](../09-data-lineage/17-interview-defensibility.md) |
| 10 | [`../10-master-data-management/18-interview-defensibility.md`](../10-master-data-management/18-interview-defensibility.md) |
| 11 | [`../11-data-lifecycle/23-interview-defensibility.md`](../11-data-lifecycle/23-interview-defensibility.md) |
| 12 | [`../12-kpis-maturity/27-interview-defensibility.md`](../12-kpis-maturity/27-interview-defensibility.md) |
| 13 | [`../13-implementation-roadmap/22-interview-defensibility.md`](../13-implementation-roadmap/22-interview-defensibility.md) |
| 14 | [`../14-ndmo-alignment/19-interview-defensibility.md`](../14-ndmo-alignment/19-interview-defensibility.md) |

Synthetic worked examples: [`../assets/practical-evidence/`](../assets/practical-evidence/).

---

## 1. How to introduce the project (30 seconds)

> “This is an enterprise data governance **framework** for a fictional Saudi MOH health cluster, Rafid Health Cluster. It is not a software build. I documented Phases 0–14: foundation through policy, quality, catalog, lineage, conceptual MDM, lifecycle, KPIs/maturity, an illustrative roadmap, and NDMO alignment. I label assumptions versus NDMO. I do not claim compliance, I do not invent control numbers or retention periods, and I do not present KPI values or maturity levels as real Rafid data.”

---

## 2. What you can defend

| Question | Answer to give |
| --- | --- |
| What is the organization? | Fictional public healthcare cluster `[A]`; modeled as holding government and personal health data. |
| What did you deliver? | Through Phase 14: Policy stack, ownership, classification, quality, conceptual catalog, conceptual lineage, conceptual MDM, conceptual data lifecycle, conceptual KPIs/maturity, an `[A]` illustrative roadmap, and an NDMO alignment/evidence pack. `DG-KPI-00n` is not an NDMO ID. |
| What did you refuse to fake? | Compliance scores, NDMO national classification names, catalog/MDM/lineage/archive/dashboard tools, invented NDMO IDs, match-score thresholds, one physical MDM database, automatic classification inheritance, invented retention periods or healthcare legal clocks, live KPI values, and a claimed Rafid maturity level. |
| What are Rafid classification tiers? | Public, Internal, Confidential, Restricted `[A][B]` — **not** NDMO national tiers `[NDMO verification required]`. |
| What is the operating model? | Federated **by data domain** `[B]`. CDO reports to CEO; CIO is a peer. Eight domain Owners are assigned in Phase 4 (titles, not people). |
| Which NDMO version? | *Data Management and Personal Data Protection Standards* v1.5, January 2021 `[C]`. |
| What is NDMO’s shape? | 15 domains, 77 controls, 191 specifications; Domain → Control → Specification `[C]`. |
| What is Domain 1? | Data Governance (`DG`), 8 controls / 28 specifications `[C]`. |
| Who owns security controls? | NDMO Domain 15 is under NCA mandate `[C]`. |
| What are the four classification levels? | NDMO four-level **concept** `[C]`; official **names** unresolved `[NDMO verification required]`. Rafid uses Public / Internal / Confidential / Restricted `[A][B]`. |

---

## 3. Answers that must not be given

| Do not say | Say instead |
| --- | --- |
| “We are NDMO compliant.” | “We documented an alignment approach. No specification has been evidenced as implemented.” |
| “NDMO control DG.4.12 says…” | Only cite IDs that appear in the official Standards text used in this repo. |
| “Open by Default means we publish patient data.” | NDMO Open by Default is adopted `[C]`, with classification and other law determining what can be public. Clinical data is not treated as open. |
| “I appointed a CDO.” | “NDMO names a CDO. Rafid has not appointed anyone in this case study. Reporting line is a `[B]` design: CDO to Cluster CEO.” |
| “Our maturity is level 3.” | Maturity is Phase 12; not assessed. |
| “PDPL article X requires…” | PDPL is on the watchlist `[NDMO verification required]` unless you have independently verified the article. |

---

## 4. Suggested walkthrough order

1. [`../README.md`](../README.md) — purpose, labels, status.
2. [`../01-project-foundation/organization-profile.md`](../01-project-foundation/organization-profile.md) — fictional as-is.
3. [`../01-project-foundation/data-landscape.md`](../01-project-foundation/data-landscape.md) — why governance is needed.
4. [`../02-governance-strategy/governance-principles.md`](../02-governance-strategy/governance-principles.md) — adopted NDMO principles vs candidate healthcare principles.
5. [`../02-governance-strategy/decision-rights.md`](../02-governance-strategy/decision-rights.md) — classes vs RACI.
6. [`../02-governance-strategy/ndmo-alignment-approach.md`](../02-governance-strategy/ndmo-alignment-approach.md) — method, domain map, what is still open.
7. [`../03-operating-model/README.md`](../03-operating-model/README.md) — operating model.
8. [`../04-ownership-stewardship/README.md`](../04-ownership-stewardship/README.md) — eight domains.
9. [`../05-data-classification/README.md`](../05-data-classification/README.md) — Rafid tiers (not NDMO names).
10. [`../06-policies-standards-procedures/README.md`](../06-policies-standards-procedures/README.md) — 1 Policy + 5 Standards + 6 Procedures. Use [`../06-policies-standards-procedures/interview-preparation.md`](../06-policies-standards-procedures/interview-preparation.md) as **internal** notes.
11. [`../07-data-quality/README.md`](../07-data-quality/README.md) — quality framework. Use [`../07-data-quality/16-interview-defensibility.md`](../07-data-quality/16-interview-defensibility.md) as **internal** notes.
12. [`../08-metadata-catalog/README.md`](../08-metadata-catalog/README.md) — conceptual catalog. Use [`../08-metadata-catalog/16-interview-defensibility.md`](../08-metadata-catalog/16-interview-defensibility.md) as **internal** notes.
13. [`../09-data-lineage/README.md`](../09-data-lineage/README.md) — lineage framework. Use [`../09-data-lineage/17-interview-defensibility.md`](../09-data-lineage/17-interview-defensibility.md) as **internal** notes.
14. [`../10-master-data-management/README.md`](../10-master-data-management/README.md) — conceptual MDM. Use [`../10-master-data-management/18-interview-defensibility.md`](../10-master-data-management/18-interview-defensibility.md) as **internal** notes.
15. [`../11-data-lifecycle/README.md`](../11-data-lifecycle/README.md) — conceptual lifecycle. Use [`../11-data-lifecycle/23-interview-defensibility.md`](../11-data-lifecycle/23-interview-defensibility.md) as **internal** notes.
16. [`../12-kpis-maturity/README.md`](../12-kpis-maturity/README.md) — conceptual KPIs/maturity. Use [`../12-kpis-maturity/27-interview-defensibility.md`](../12-kpis-maturity/27-interview-defensibility.md) as **internal** notes.
17. [`../13-implementation-roadmap/README.md`](../13-implementation-roadmap/README.md) — `[A]` illustrative roadmap. Use [`../13-implementation-roadmap/22-interview-defensibility.md`](../13-implementation-roadmap/22-interview-defensibility.md) as **internal** notes.
18. [`../14-ndmo-alignment/README.md`](../14-ndmo-alignment/README.md) — alignment pack. Use [`../14-ndmo-alignment/19-interview-defensibility.md`](../14-ndmo-alignment/19-interview-defensibility.md) as **internal** notes.
19. [`../assets/practical-evidence/`](../assets/practical-evidence/) — synthetic examples only (`[A]`).

---

## 5. Likely deep-dive questions

### “How is this different from DAMA?”

NDMO cites DAMA DMBOK as a key reference `[C]`. DAMA is a body of knowledge `[B]`. NDMO is a national **standards** document with auditable specifications `[C]`. This repo uses DAMA-style structure as `[B]` only when labeled, and uses NDMO names/IDs only when `[C]`.

### “How did you start Phase 3 without redesigning strategy?”

Used Phase 2 decision classes and NDMO **role names**. Proposed office, committee, and reporting lines. Did not change vision/principles. Did not assign Data Owners. Fetch the NDMO Organizational Manual before writing job descriptions `[NDMO verification required]`. Control-level organization IDs remain `[NDMO verification required]`.

### “How do you handle conflicting clinical confidentiality and Open by Default?”

Policy hierarchy: law (L0) and classification constrain openness. Open by Default is not a licence to publish Restricted or Confidential Rafid datasets. Dataset decisions follow Phase 5 / POL-001 / PRC-005.

### “What would an annual NDMO assessment look like?”

NDMO describes entity-led annual assessment at **specification** level, binary 100% vs 0% if partial, with evidence, led by the CDO, reported in Q3 as stated in the Standards `[C]`. Rafid has no score. A real assessment would not mark Phase 0–2 documents as `DG.1` complete, because budget, 3-year plan, and approval are missing.

### “How does Phase 7 data quality work?”

Seven Rafid dimensions `[A][B]`: Accuracy, Completeness, Validity on every CDE; the other four only when material. Thirteen illustrative CDEs; no numeric CDE score. Two-step confirmation (candidate, then Owner/Steward warrant). Issues follow the Phase 6 Data Quality Issue Management Procedure. Example percentages are **illustrative**. NDMO quality dimensions/thresholds/CDE/scoring remain `[NDMO verification required]`. Detail: [`../07-data-quality/16-interview-defensibility.md`](../07-data-quality/16-interview-defensibility.md) (**internal**).

### “Did you implement a data catalog tool?”

No. Phase 8 is **governance and conceptual design**. Seven metadata categories `[A][B]`; mandatory vs capability-dependent; Year-1 asset types excluding API/Data Product; MVP = three domains. Certification is **internal trust**, not NDMO certification. Coarse lineage metadata is Phase 8; the lineage **framework** is Phase 9. Detail: [`../08-metadata-catalog/16-interview-defensibility.md`](../08-metadata-catalog/16-interview-defensibility.md) (**internal**).

### “Did you build automated data lineage?”

No. Phase 9 is **governance and conceptual design**. Year-1 priorities are business and conceptual lineage. Technical lineage is conceptual only. One illustrative E2E example (not MOH/NPHIES/Rafid architecture). Downstream data does **not** auto-inherit the highest classification tier. Detail: [`../09-data-lineage/17-interview-defensibility.md`](../09-data-lineage/17-interview-defensibility.md) (**internal**).

### “Did you implement an MDM tool?”

No. Phase 10 is **conceptual MDM**. Core masters are Patient, Provider, and Facility (Facility is **supporting only**). Golden record is logical, not one database. No match scores. HR, Finance transactions, and Quality are Non-MDM at this maturity. Detail: [`../10-master-data-management/18-interview-defensibility.md`](../10-master-data-management/18-interview-defensibility.md) (**internal**).

### “Did you implement retention, archive, or records management?”

No. Phase 11 is **conceptual Data Lifecycle Management**. Archive ≠ Backup. Records Management is referenced as distinct and **not built**. Retention Period fields are `[NDMO verification required]` / `[Legal / regulatory verification required]`. Classification does **not** automatically determine duration. MVP = Patient / Person Master, Clinical / Medical Records, Financial / Billing & Claims. Detail: [`../11-data-lifecycle/23-interview-defensibility.md`](../11-data-lifecycle/23-interview-defensibility.md) (**internal**).

### “Did you implement a governance dashboard or score Rafid’s maturity?”

No. Phase 12 is **conceptual measurement**. Twelve executive KPIs (`DG-KPI-001`–`012`) are **fictional Rafid IDs**, not NDMO controls. Targets: **To be established after baseline measurement.** Five maturity levels; KPIs **inform** maturity and do **not** automatically determine it. No live Rafid KPI values or maturity results. Not `DG.7` complete. Detail: [`../12-kpis-maturity/27-interview-defensibility.md`](../12-kpis-maturity/27-interview-defensibility.md) (**internal**).

---

## 6. Source labels — 15-second explanation

> “`[A]` is fiction I invented for the case. `[B]` is common governance practice. `[C]` is something I can point to in NDMO Standards v1.5. If I am not sure the official text supports the **use** I am making, I tag `[NDMO verification required]` rather than guessing.”

---

## 7. Known limits of this drop

- Phase 6 documents are design text; no live DMC approval or NDMO assessment is claimed.
- Phase 7 Data Quality framework is documented; example thresholds and scorecard cells are **illustrative**, not measured Rafid performance. NDMO quality dimensions, thresholds, CDE mandates, and scoring remain `[NDMO verification required]`.
- Phase 8 Metadata and catalog is documented as **conceptual design**; no Purview/Collibra/Atlan/Informatica implementation. NDMO metadata fields, categories, and control-level catalog requirements remain `[NDMO verification required]`.
- Phase 9 Data lineage is documented as **conceptual/business lineage**; one illustrative E2E example; no scanner. Specific NDMO lineage requirements remain `[NDMO verification required]`.
- Phase 10 Master data management is documented as **conceptual MDM**; no hub/engine. Specific NDMO MDM requirements remain `[NDMO verification required]`.
- Phase 11 Data lifecycle is documented as **conceptual governance**; no invented retention periods, disposal timeframes, or legal/NDMO compliance claims. Specific NDMO lifecycle/retention/archive/disposal requirements remain `[NDMO verification required]`. Healthcare retention remains `[Legal / regulatory verification required]`.
- Phase 12 KPIs and maturity is documented as **conceptual measurement**; no live Rafid KPI values, targets, or maturity results. `DG-KPI-00n` is not an NDMO ID. `DG.7` is not claimed implemented. Specific NDMO KPI types/targets remain `[NDMO verification required]`.
- Phase 13 is implemented as an `[A]` Illustrative Implementation Roadmap. It is documentation/design only; operational implementation and measured performance are not claimed. It is not a real plan; not NDMO-required sequencing; not evidence of implementation or NDMO compliance. No dates, budgets, headcount, KPI results, or maturity results.
- Phase 14 NDMO alignment pack is documented as **Designed** evidence/alignment only; **not** a compliance certification. Operational and measured evidence are **not claimed**.
- NDMO regulations beyond the Standards PDF were not retrieved.
- No Arabic controlled vocabulary yet.
- No diagrams beyond markdown/mermaid support files in `assets/`.
- Healthcare sector overlays (MOH, CBAHI, etc.) are watchlist only.

---

## 8. Phase 14 — Alignment vs compliance (add-on)

Detail: [`../14-ndmo-alignment/19-interview-defensibility.md`](../14-ndmo-alignment/19-interview-defensibility.md) (**internal**).

### Alignment vs compliance

Alignment means the framework is structured to address relevant NDMO **domains** using verified names and a labeled method. Compliance requires verified specification text, approved implementation, **operational** evidence, and assessment. This portfolio is **alignment documentation**. It is **not** NDMO compliance.

**The Rafid framework is a portfolio design exercise. Its artifacts demonstrate how a Data Governance function could be structured; they are not evidence that Rafid Health Cluster has operationally implemented or achieved NDMO compliance.**

### Evidence readiness

All Phase 0–14 artifacts are **Designed**. **Operational = Not claimed. Measured = Not claimed.** Phase 13 is an illustrative roadmap only. A real organization would still need appointments, approvals, live registers, baselines, and an official assessment process `[C]` as described in the Standards — none of which is claimed here.

### Verification discipline

`[C]` only where traced to NDMO Standards v1.5 as already used in Phase 2. Uncopied control/specification IDs stay `[NDMO verification required]`. IDs such as `RHC-EVD-001` and `DG-KPI-001` are **Rafid** identifiers, not NDMO controls. Rafid classification tiers, RACI, DMC composition, KPIs, and the Phase 13 `[A]` illustrative roadmap are **not** briefed as NDMO-mandated.

### How to defend the project

> “I built a labeled governance design for a fictional health cluster, mapped it to NDMO domain **names** I could cite, and refused to invent the rest. I can show what evidence would look like if this were operational. I cannot and do not claim NDMO compliance.”

