# Rafid Health Cluster — Enterprise Data Governance Framework

**Document type:** Program overview  
**Organization:** Rafid Health Cluster `[A]`  
**Program type:** Enterprise data governance framework (documentation and operating design)  
**Not in scope:** Application development, platform build, or tool implementation  
**Current status:** Phases 0–14: Designed / Documented. Operational implementation = Not claimed. Measured performance = Not claimed. NDMO compliance = Not claimed. Phase 14 is the final alignment/evidence phase.

---

## 1. Purpose

This repository holds the **enterprise Data Governance Framework** for Rafid Health Cluster, a fictional Saudi healthcare delivery organization.

The work product is a **governed operating design**: strategy, operating model, policies, standards, and implementation artifacts. It is **not** a software product.

The program exists to:

- Treat cluster data as a managed organizational asset.
- Establish authority, accountability, and decision rights for data.
- Prepare the cluster to **align** with the Kingdom’s National Data Management and Personal Data Protection Standards issued by the National Data Management Office (NDMO).
- Remain interview-ready: every material statement is labeled by source, and regulatory claims are not invented.

This repository **does not claim** that Rafid Health Cluster is NDMO-compliant, PDPL-certified, or NCA-compliant.

---

## 2. Organization

| Item | Statement | Label |
| --- | --- | --- |
| Legal name | Rafid Health Cluster (مجمع رافد الصحي) | `[A]` |
| Nature | Fictional Ministry of Health (MOH) health cluster | `[A]` |
| Sector | Public healthcare delivery — Kingdom of Saudi Arabia | `[A]` |
| Assumed regulatory posture | Modeled as a **Public Entity** holding government and personal health data | `[A]` + `[NDMO verification required]` |
| Delivery footprint | Multi-hospital cluster with primary care and selected specialty services | `[A]` |

Organization detail is in [`01-project-foundation/organization-profile.md`](01-project-foundation/organization-profile.md).

---

## 3. Project scope

**In scope for the overall program**

- Enterprise data governance strategy and operating design.
- Ownership and stewardship model.
- Classification, quality, metadata, lineage, master data, and lifecycle **frameworks**.
- Policy / standard / procedure hierarchy.
- KPI and maturity approach.
- NDMO **alignment** documentation (mapping and evidence approach — not a compliance attestation).

**Out of scope for the overall program**

- Building or configuring EMR, integration, catalog, or MDM software.
- Legal opinions, official regulator submissions, or audit letters.
- Invented NDMO control numbers or fabricated compliance scores.
- Redesign of later-phase artifacts ahead of their approved design.

**In scope for this repository drop**

- Phase 0 — Project foundation.
- Phase 1 — Governance direction (vision, mission, objectives, principles).
- Phase 2 — Governance design boundaries (scope, decision-rights classes, policy hierarchy, NDMO alignment approach).
- Phase 3 — Operating model (federated-by-domain structure, reporting lines, RACI, forums, workflow).
- Phase 4 — Data ownership and stewardship (eight domains, one Owner each, decision RACI, stewardship model).
- Phase 5 — Data classification framework (Rafid proposed four-tier scheme; dataset-level; NDMO names unresolved).
- Phase 6 — Policies, standards, and procedures (1 Policy + 5 Standards + 6 Procedures).
- Phase 7 — Data quality framework (dimensions, CDEs, representative rules, monitoring; illustrative only).
- Phase 8 — Metadata management and conceptual data catalog (no catalog product).
- Phase 9 — Data lineage framework (conceptual/business lineage; one illustrative E2E example).
- Phase 10 — Master data management (conceptual MDM; Patient and Provider primary; Facility supporting only).
- Phase 11 — Data lifecycle management (conceptual Create→Dispose governance; no invented retention periods).
- Phase 12 — KPIs and maturity (conceptual measurement; 12 executive KPIs; five-level maturity; no live Rafid results).
- Phase 13 — Implementation roadmap (`[A]` Illustrative; not a real plan; not NDMO-required sequencing; not implementation or compliance evidence).
- Phase 14 — NDMO alignment and evidence pack (consolidation only; not a compliance certification).

**Explicitly not claimed in this drop:** operational implementation, measured performance, or NDMO compliance.

Detail: [`01-project-foundation/project-scope.md`](01-project-foundation/project-scope.md).

---

## 4. Current project status

| Phase | Focus | Repository location | Status |
| --- | --- | --- | --- |
| 0 | Project foundation | `01-project-foundation/` | **Documented** |
| 1 | Governance direction | `02-governance-strategy/` (vision, objectives, principles) | **Documented** |
| 2 | Governance design boundaries | `02-governance-strategy/` (scope, decision rights, policy hierarchy, NDMO alignment approach) | **Documented** |
| 3 | Operating model | `03-operating-model/` | **Documented** |
| 4 | Ownership and stewardship | `04-ownership-stewardship/` | **Documented** |
| 5 | Data classification | `05-data-classification/` | **Documented** |
| 6 | Policies, standards, procedures | `06-policies-standards-procedures/` | **Documented** |
| 7 | Data quality | `07-data-quality/` | **Documented** |
| 8 | Metadata and catalog | `08-metadata-catalog/` | **Documented** |
| 9 | Data lineage | `09-data-lineage/` | **Documented** |
| 10 | Master data management | `10-master-data-management/` | **Documented** |
| 11 | Data lifecycle | `11-data-lifecycle/` | **Documented** |
| 12 | KPIs and maturity | `12-kpis-maturity/` | **Documented** |
| 13 | Implementation roadmap | `13-implementation-roadmap/` | **Documented** |
| 14 | NDMO alignment pack | `14-ndmo-alignment/` | **Documented** |

**Roles on this program**

- **Governance analysis and design decisions:** Claude (governance designer).
- **Repository structure, documentation, and technical artifacts:** implementation/documentation engineer (this workstream).
- This drop records Phases 0–14 as **Designed** documentation. Phase 13 is an **`[A]` illustrative** roadmap only — not a real transformation plan, not NDMO-required sequencing, and not evidence of implementation or compliance. **Operational implementation is not claimed. Measured performance is not claimed.** It does not appoint named people, implement catalog/MDM/quality/lineage/lifecycle/dashboard tooling, or claim NDMO control implementation or NDMO compliance. Rafid classification labels are not NDMO national tiers. Phase 7 scorecard numbers are illustrative, not measured Rafid performance. Phase 8 is conceptual metadata/catalog design, not a platform. Phase 9 lineage is conceptual/business; the E2E example is not real MOH/NPHIES/Rafid architecture. Phase 10 MDM is conceptual; golden record is logical, not a physical hub. Phase 11 lifecycle is conceptual governance; no invented retention periods, disposal timeframes, or legal/NDMO compliance claims. Phase 12 KPIs (`DG-KPI-00n`) are fictional Rafid identifiers, not NDMO control IDs; no KPI value or maturity level is real Rafid performance. `DG.7` is not claimed implemented. Phase 14 organizes alignment and **designed** evidence only.

---

## 5. Phase structure

```text
Phase 0  Foundation          →  who we are, what data we hold, what the program covers
Phase 1  Direction           →  vision, mission, objectives, principles
Phase 2  Design boundaries   →  governance scope, decision-right classes, policy hierarchy, NDMO alignment method
Phase 3  Operating model     →  federated-by-domain structure, reporting lines, RACI, forums
Phase 4  Ownership           →  eight domains, one Owner each, stewardship, decision RACI
Phase 5  Classification      →  Rafid Public / Internal / Confidential / Restricted (proposed; not NDMO names)
Phase 6  Policy stack        →  1 Policy + 5 Standards + 6 Procedures (MDM standalone)
Phase 7  Data quality        →  dimensions, CDEs, representative rules, issue integration
Phase 8  Metadata / catalog  →  conceptual catalog, minimum metadata, glossary, MVP (no product)
Phase 9  Data lineage        →  business/conceptual lineage; one illustrative E2E example
Phase 10 Master data         →  conceptual MDM; Patient & Provider primary; Facility supporting
Phase 11 Data lifecycle      →  conceptual Create→Dispose; no invented retention periods
Phase 12 KPIs / maturity     →  conceptual 12 executive KPIs; five-level maturity; no live results
Phase 13 Implementation plan →  `[A]` illustrative 3-year shape; no dates/budget/results
Phase 14 NDMO alignment      →  evidence pack; Designed only; not a compliance certification
```

Phase 0–2 produce **strategy artifacts**. Phase 3 produces the **operating model**. Phase 4 produces **domain ownership**. Phase 5 produces a **proposed Rafid classification framework**. Phase 6 produces **1 Policy + 5 Standards + 6 Procedures**. Phase 7 produces the **data quality framework**. Phase 8 produces **metadata and conceptual catalog design**. Phase 9 produces a **conceptual lineage framework**. Phase 10 produces a **conceptual MDM framework**. Phase 11 produces a **conceptual data lifecycle framework**. Phase 12 produces a **conceptual KPI and maturity framework**. Phase 13 produces an **`[A]` illustrative implementation roadmap**. Phase 14 produces an **NDMO alignment and designed-evidence pack**. Together they do not implement NDMO specifications, appoint named officers, or equate Rafid tiers with official NDMO tier names. **Phases 0–14 = Designed. Operational implementation = Not claimed. Measured performance = Not claimed.**

NDMO’s own Data Governance domain (`DG`) requires a Data Management and Personal Data Protection Strategy, including vision, mission, goals, and guiding principles (`[C]` — NDMO Standards v1.5, control `DG.1`). This program uses that official requirement as the **reason Phase 1–2 exist**. It does not treat the existence of these documents as proof of compliance. Phase 3 does **not** re-assert specification-level organization control IDs as verified; those remain `[NDMO verification required]`.

---

## 6. Source and assumption labeling convention

Every material statement in this repository is tagged. Labels are not optional.

| Label | Meaning | How it is used |
| --- | --- | --- |
| `[A]` | **Fictional assumption** | Cluster facts invented for the portfolio (name, facilities, systems, current-state pain). Not a real organization. |
| `[B]` | **Industry best practice** | Common data-governance practice (for example DAMA-DMBOK-style strategy structure, policy hierarchy layers, decision classes). Not presented as an NDMO mandate. |
| `[C]` | **NDMO-supported** | Content that can be traced to the official NDMO *Data Management and Personal Data Protection Standards* (Version 1.5, January 2021) or another cited official NDMO/SDAIA publication. Control IDs are used **only** when they appear in that source. |
| `[NDMO verification required]` | **Not confirmed against the official text for this use** | Applicability, role-manual detail, sector overlays, later regulations, or any mapping that has not been checked in the official document. Must not be briefed as a requirement. |
| `[Legal / regulatory verification required]` | **Not confirmed against applicable law for this use** | Used in Phase 11 for healthcare and other retention/hold/disposal clocks that have not been legally verified. Must not be briefed as a statutory period. |

### Rules of use

1. Do **not** invent NDMO requirements.
2. Do **not** create fake NDMO control or specification numbers.
3. Do **not** claim regulatory compliance, certification, or completed audits.
4. If a statement is both a cluster assumption and an NDMO theme, apply **both** labels.
5. Official NDMO control IDs cited in this repo (for example `DG.1`, `DG.2`, `DC.3`) are taken from NDMO Standards v1.5. They are **reference pointers**, not evidence that Rafid has implemented the control.
6. NDMO’s *Organizational Manual* and several NDMO **regulations** (classification, sharing, FOI, and others) are referenced by the Standards but were **not retrieved for this drop**. Role-duty detail and regulation-level procedures remain `[NDMO verification required]`.

Primary official source for `[C]` labels in Phase 0–2:

- National Data Management Office, *Data Management and Personal Data Protection Standards*, Version 1.5, January 2021, published via SDAIA.

---

## 7. Repository map

```text
rafid-health-cluster-data-governance/
├── README.md                          ← this file
├── 01-project-foundation/             ← Phase 0
├── 02-governance-strategy/            ← Phase 1–2
├── 03-operating-model/                ← Phase 3 (operating model)
├── 04-ownership-stewardship/          ← Phase 4 (ownership and stewardship)
├── 05-data-classification/            ← Phase 5 (Rafid proposed classification framework)
├── 06-policies-standards-procedures/  ← Phase 6 (1 Policy + 5 Standards + 6 Procedures)
├── 07-data-quality/                   ← Phase 7 (data quality framework)
├── 08-metadata-catalog/               ← Phase 8 (conceptual metadata and catalog)
├── 09-data-lineage/                   ← Phase 9 (conceptual lineage framework)
├── 10-master-data-management/         ← Phase 10 (conceptual MDM)
├── 11-data-lifecycle/                 ← Phase 11 (conceptual data lifecycle)
├── 12-kpis-maturity/                 ← Phase 12 (conceptual KPIs and maturity)
├── 13-implementation-roadmap/         ← Phase 13 (`[A]` illustrative roadmap)
├── 14-ndmo-alignment/                 ← Phase 14 (alignment and designed evidence)
├── assets/
│   ├── diagrams/
│   ├── tables/
│   └── templates/
└── docs/
    └── interview-preparation.md
```

---

## 8. How to read this portfolio

1. Start with this README and [`docs/interview-preparation.md`](docs/interview-preparation.md).
2. Read Phase 0 in order: scope → organization → data landscape.
3. Read Phase 1–2 in `02-governance-strategy/`.
4. Read Phase 3 in `03-operating-model/` (start with that folder’s README). Interview notes in Phase 3 are **internal**, not policy.
5. Read Phase 4 in `04-ownership-stewardship/`. Interview notes there are **internal**, not policy.
6. Read Phase 5 in `05-data-classification/`. Rafid tiers are **not** NDMO national tiers. Interview notes are **internal**, not policy.
7. Read Phase 6 in `06-policies-standards-procedures/` (**1 Policy + 5 Standards + 6 Procedures**). Interview notes there are **internal**, not policy.
8. Read Phase 7 in `07-data-quality/`. Dimension names and thresholds are Rafid design `[A][B]`, not claimed as NDMO-required. Interview notes are **internal**, not policy. Example scores are illustrative, not measured performance.
9. Read Phase 8 in `08-metadata-catalog/`. This is conceptual catalog design, not Purview/Collibra/Atlan. Interview notes are **internal**.
10. Read Phase 9 in `09-data-lineage/`. Business/conceptual lineage; one illustrative E2E example — not real MOH/NPHIES/Rafid architecture. Interview notes are **internal**. Lineage does **not** auto-classify downstream data.
11. Read Phase 10 in `10-master-data-management/`. Conceptual MDM; golden record is logical. Facility is supporting scope only. Interview notes are **internal**.
12. Read Phase 11 in `11-data-lifecycle/`. Conceptual Create→Dispose governance; Archive ≠ Backup; no invented retention periods. Interview notes are **internal**.
13. Read Phase 12 in `12-kpis-maturity/`. Conceptual KPIs and maturity; `DG-KPI-00n` is not an NDMO ID; no live Rafid scores. Interview notes are **internal**.
14. Read Phase 13 in `13-implementation-roadmap/`. **`[A]` Illustrative** roadmap — not a real plan, not NDMO-required sequencing, not implementation or compliance evidence. Interview notes are **internal**.
15. Read Phase 14 in `14-ndmo-alignment/`. Alignment and **designed** evidence only — **not** NDMO compliance. Interview notes are **internal**.
16. If asked in an interview whether the cluster is “NDMO compliant,” the correct answer is: **no compliance claim is made**; this program documents an alignment **approach** and a Designed-only evidence pack.
