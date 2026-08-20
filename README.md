# Rafid Health Cluster — Data Governance Framework

A portfolio-grade Data Governance and Data Management framework designed for a fictional Saudi healthcare cluster, covering governance strategy, operating model, ownership, classification, data quality, metadata, lineage, MDM, lifecycle management, KPIs, implementation roadmap, and NDMO alignment.

Rafid Health Cluster is **fictional**. This is a **portfolio design exercise**, not a software product, not a live implementation, and **not an NDMO compliance claim**.

---

## Portfolio Quick View

Use this if you are reviewing as a recruiter or hiring manager.

### 5-Minute Review

1. [Governance Strategy](02-governance-strategy/)
2. [Operating Model](03-operating-model/)
3. [Data Quality](07-data-quality/)
4. [Metadata & Data Catalog](08-metadata-catalog/)
5. [NDMO Alignment](14-ndmo-alignment/)

Optional: [Practical evidence samples](assets/practical-evidence/) (synthetic examples only).

### 15-Minute Review

1. [Project Foundation](01-project-foundation/)
2. [Governance Strategy](02-governance-strategy/)
3. [Operating Model](03-operating-model/)
4. [Ownership & Stewardship](04-ownership-stewardship/)
5. [Classification](05-data-classification/)
6. [Data Quality](07-data-quality/)
7. [Metadata & Catalog](08-metadata-catalog/)
8. [Lineage](09-data-lineage/)
9. [MDM](10-master-data-management/)
10. [NDMO Alignment](14-ndmo-alignment/)

### Deep Dive

The complete framework is organized across **Phases 0–14** (folders `01`–`14`). Interview notes are **internal** and are indexed in [`docs/interview-preparation.md`](docs/interview-preparation.md).

---

## Project Overview

This repository documents how an enterprise Data Governance function **could be designed** for a fictional Saudi healthcare cluster. It demonstrates connected decisions across operating model, ownership, classification, quality, metadata, lineage, MDM, lifecycle, measurement, and implementation planning.

Healthcare is used because it supplies realistic examples of sensitive data, master identity, lineage, quality, lifecycle, and regulatory overlay — without treating Rafid as a real organization.

The work product is **governed operating design** (strategy, RACI, policies, and capability frameworks). It is **not** a platform build and **not** production evidence.

---

## What This Project Demonstrates

- Data Governance Operating Model Design
- Data Ownership & Stewardship
- Data Classification
- Policy & Standards Architecture
- Data Quality Governance
- Metadata Management
- Business Glossary Design
- Data Catalog Design
- Data Lineage Governance
- Master Data Management
- Data Lifecycle Governance
- Governance KPIs
- Data Maturity Assessment (method only; no Rafid score)
- Implementation Planning (illustrative)
- NDMO Alignment & Evidence Design
- Compliance & Risk mapping (conceptual NDMO/PDPL inputs; no compliance claim)

---

## Objectives

- Design a complete enterprise Data Governance operating model.
- Define ownership, stewardship, decision rights, and escalation.
- Establish a practical data classification model.
- Define Data Quality governance and CDE management.
- Design metadata/catalog and conceptual lineage governance.
- Define a conceptual MDM approach.
- Establish enterprise data lifecycle governance.
- Define KPIs and a maturity model.
- Produce an illustrative implementation roadmap.
- Map governance artifacts to NDMO domains without claiming compliance.

---

## Framework Coverage

| Area | Coverage |
| --- | --- |
| Governance Strategy | Vision, objectives, principles, scope, decision rights |
| Operating Model | Roles, reporting lines, RACI, forums, escalation |
| Ownership & Stewardship | Data Owners, Stewards, ownership lifecycle |
| Data Classification | Four-tier Rafid classification proposal |
| Policies & Standards | 1 Policy + 5 Standards + 6 Procedures |
| Data Quality | 7 dimensions, CDE methodology, rules, issues, monitoring |
| Metadata & Catalog | Metadata model, minimum metadata, glossary, catalog MVP, plus an applied [working pack](08-metadata-catalog/working-pack/) (inventory, field model, sample catalog pages) |
| Data Lineage | Business/conceptual lineage and selective technical lineage, plus an applied [working pack](09-data-lineage/working-pack/) (register, examples, quality checks) |
| Master Data Management | Master/reference/transaction model, golden record, matching, survivorship |
| Data Lifecycle | Retention governance, archiving, disposal, legal holds |
| KPIs & Maturity | KPI framework and five-level maturity model |
| Implementation Roadmap | Illustrative three-year implementation roadmap |
| NDMO Alignment | Domain mapping, evidence design, verification/gap register, plus an applied [Compliance & Risk working pack](14-ndmo-alignment/working-pack/) (project evidence states, PDPL governance considerations, governance risk register) |

---

## Phase Structure

| Phase | Focus | Folder |
| --- | --- | --- |
| 0 | Project definition — purpose, scope, and documentation boundaries | [01-project-foundation](01-project-foundation/) |
| 1 | Organization and data landscape — fictional cluster profile and assumed data holdings | [01-project-foundation](01-project-foundation/) |
| 2 | Governance strategy — vision, principles, scope, decision-right classes, and NDMO alignment approach | [02-governance-strategy](02-governance-strategy/) |
| 3 | Operating model — federated-by-domain structure, roles, RACI, forums, and escalation | [03-operating-model](03-operating-model/) |
| 4 | Ownership and stewardship — eight domains, one Data Owner each, and stewardship operating design | [04-ownership-stewardship](04-ownership-stewardship/) |
| 5 | Data classification — Rafid Public / Internal / Confidential / Restricted proposal | [05-data-classification](05-data-classification/) |
| 6 | Policies, standards, and procedures — 1 Policy + 5 Standards + 6 Procedures | [06-policies-standards-procedures](06-policies-standards-procedures/) |
| 7 | Data quality — dimensions, CDEs, rules, issues, and monitoring design | [07-data-quality](07-data-quality/) |
| 8 | Metadata and catalog — conceptual catalog, minimum metadata, glossary, and MVP | [08-metadata-catalog](08-metadata-catalog/) |
| 9 | Data lineage — business/conceptual lineage, criticality, and one illustrative end-to-end example | [09-data-lineage](09-data-lineage/) |
| 10 | Master data management — conceptual MDM; Patient and Provider primary; Facility supporting | [10-master-data-management](10-master-data-management/) |
| 11 | Data lifecycle — Create→Dispose governance; no invented retention periods | [11-data-lifecycle](11-data-lifecycle/) |
| 12 | KPIs and maturity — twelve executive KPIs and a five-level maturity model | [12-kpis-maturity](12-kpis-maturity/) |
| 13 | Implementation roadmap — `[A]` illustrative three-year shape; not a live transformation plan | [13-implementation-roadmap](13-implementation-roadmap/) |
| 14 | NDMO alignment and evidence — designed evidence pack plus applied [Compliance & Risk working pack](14-ndmo-alignment/working-pack/); final phase; not a compliance certification | [14-ndmo-alignment](14-ndmo-alignment/) |

---

## Practical Evidence `[A]`

A small **illustrative** layer shows how selected designs could be applied to **synthetic** data. Recruiter-facing samples sit in [`assets/practical-evidence/`](assets/practical-evidence/). Applied working packs sit under Phase 8 (metadata/catalog), Phase 9 (lineage), and Phase 14 (compliance/risk mapping).

| Example | File |
| --- | --- |
| Data quality (sample → rules → issues → result) | [01-data-quality-example.md](assets/practical-evidence/01-data-quality-example.md) |
| Catalog sample (15 assets) | [02-catalog-sample.md](assets/practical-evidence/02-catalog-sample.md) |
| Business glossary sample (15 terms) | [03-business-glossary-sample.md](assets/practical-evidence/03-business-glossary-sample.md) |
| Metadata Management working pack | [08-metadata-catalog/working-pack/](08-metadata-catalog/working-pack/) |
| Data Catalog & Lineage working pack | [09-data-lineage/working-pack/](09-data-lineage/working-pack/) |
| Compliance & Risk working pack | [14-ndmo-alignment/working-pack/](14-ndmo-alignment/working-pack/) |
| MDM golden record (patient identity) | [04-mdm-golden-record-example.md](assets/practical-evidence/04-mdm-golden-record-example.md) |
| Conceptual lineage (registration → dashboard) | [05-lineage-example.md](assets/practical-evidence/05-lineage-example.md) |

These examples are **not** operational evidence of a live organization, **not** measured Rafid performance, and **not** NDMO compliance evidence. The Phase 14 working pack may label selected repository working records as **Operational (project)**; that label does **not** change this organizational claim.

---

## Key Design Decisions

- Federated-by-domain governance model.
- CEO-chaired Data Management Committee.
- Data Owners are business roles; IT/Custodian does not act as Data Owner.
- Business Data Steward is the generic stewardship role.
- Rafid classification uses Public / Internal / Confidential / Restricted as an `[A][B]` entity proposal.
- Rafid classification tiers are **not** presented as NDMO national classification tiers.
- MDM is a standalone Standard in the Phase 6 architecture.
- Patient/Person and Provider/Clinician are the primary MDM MVP domains; Facility/Organization is supporting only.
- Technical lineage remains conceptual.
- Retention periods are not invented and remain verification placeholders where required.
- KPIs and roadmap figures are illustrative rather than measured Rafid performance.
- The Phase 13 roadmap is not a live implementation plan, not an NDMO-required sequence, and not evidence of implementation.

---

## Evidence & Source Discipline

Every material statement in the framework is labeled:

| Label | Meaning |
| --- | --- |
| `[A]` | Fictional / illustrative Rafid assumption |
| `[B]` | Industry best practice |
| `[C]` | NDMO-supported content based on the sources explicitly verified for the project |
| `[NDMO verification required]` | Requires verification against the applicable official NDMO source/version |
| `[Legal / regulatory verification required]` | Requires verification against applicable law/regulation |

These labels are used to prevent fictional design choices from being presented as regulatory requirements.

---

## NDMO Position

The framework is aligned conceptually to relevant NDMO domains and uses NDMO-supported material where explicitly verified. It does not claim NDMO compliance.

Control/specification-level verification remains open where the official source text was not available or independently verified.

---

## Project Status

**Project Status: Designed / Documented**

- Operational implementation: Not claimed
- Measured performance: Not claimed
- NDMO compliance: Not claimed
- Rafid Health Cluster: Fictional portfolio organization

---

## Repository Structure

```text
rafid-health-cluster-data-governance/
├── README.md
├── 01-project-foundation/
├── 02-governance-strategy/
├── 03-operating-model/
├── 04-ownership-stewardship/
├── 05-data-classification/
├── 06-policies-standards-procedures/
├── 07-data-quality/
├── 08-metadata-catalog/
│   └── working-pack/          # applied glossary, inventory, catalog samples
├── 09-data-lineage/
│   └── working-pack/          # applied lineage register, examples, quality checks
├── 10-master-data-management/
├── 11-data-lifecycle/
├── 12-kpis-maturity/
├── 13-implementation-roadmap/
├── 14-ndmo-alignment/
│   └── working-pack/          # applied NDMO/PDPL mapping, evidence states, risk register
├── assets/
│   └── practical-evidence/
└── docs/
```

---

## How to Use This Repository

1. Start with Phase 0–2 for context and strategy.
2. Review Phase 3–5 for governance structure, ownership, and classification.
3. Review Phase 6 for the policy/standard/procedure architecture.
4. Review Phase 7–11 for the core Data Management capabilities.
5. Optionally open [`assets/practical-evidence/`](assets/practical-evidence/) for synthetic worked examples.
6. Review Phase 12–13 for measurement and illustrative implementation planning.
7. Finish with Phase 14 for NDMO alignment and designed evidence.

Interview notes are **Internal Interview Preparation**, not policy. Start at [`docs/interview-preparation.md`](docs/interview-preparation.md).

---

## Portfolio / Interview Context

This project was created as a portfolio exercise to demonstrate practical Data Governance and Data Management thinking in a Saudi organizational context. It is designed to show how governance decisions connect across operating model, ownership, classification, quality, metadata, lineage, MDM, lifecycle, measurement, and implementation planning.

Interviewers should distinguish between the project's designed artifacts and actual organizational implementation.

---

## Limitations

- Rafid Health Cluster is fictional.
- Illustrative metrics, thresholds, classifications, examples, and roadmap assumptions are not live organizational data.
- Practical evidence files use synthetic identifiers only.
- Some NDMO details remain subject to official-source verification.
- Sector-specific legal/regulatory requirements are not presented as verified unless explicitly labeled.
- No production technology platform has been implemented.
- No operational compliance evidence is claimed.

---

## License / Usage

Portfolio project for demonstration and interview purposes.
