# Project Scope

**Document ID:** RHC-DG-P0-001  
**Phase:** 0 — Project Foundation  
**Status:** Documented  
**Depends on:** Organization profile, data landscape  
**Does not decide:** Operating model, policies, classification scheme, KPIs, or roadmap dates

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document bounds the **Rafid Health Cluster Data Governance Framework** program: what it covers, what it excludes, and which decisions are deferred.

It is a foundation artifact `[B]`. It is not an NDMO specification and does not constitute a Data Management and Personal Data Protection Plan (`DG.1.3` remains a later-phase deliverable).

---

## 2. Program definition

| Item | Statement | Label |
| --- | --- | --- |
| Program name | Rafid Health Cluster Data Governance Framework | `[A]` |
| Program type | Enterprise data governance **framework** (people, process, policy, and accountability design) | `[B]` |
| Not a | Software application, data platform, or EMR implementation | `[A]` |
| Intended use | Portfolio-quality operating design for a fictional KSA public healthcare cluster | `[A]` |

---

## 3. Why the program exists

Rafid Health Cluster is assumed to hold clinical, administrative, workforce, and financial data across multiple facilities, with fragmented ownership and no formal data office `[A]`.

NDMO states that Data Governance provides authority and control over planning and implementation of data management practices through people, processes, and technologies, in alignment with the entity’s Data Management and Personal Data Protection Strategy `[C]` (NDMO Standards v1.5, Domain 1 — Data Governance).

NDMO Standards are intended to be adopted by Public Entities in the Kingdom, and also extend to business partners handling government data `[C]` (NDMO Standards v1.5, Purpose and Scope). Whether Rafid, as a fictional MOH cluster, is in scope as a Public Entity is an **assumption for this portfolio** `[A]` and remains `[NDMO verification required]` for any real entity.

This program therefore designs governance so the cluster can **align** to that national framework. It does **not** assert that alignment is complete.

---

## 4. In scope

### 4.1 Overall program (all phases, when built)

| Area | Included | Label |
| --- | --- | --- |
| Strategy | Vision, mission, objectives, principles, governance scope | Phase 1–2 |
| Authority | Decision-right **classes**; later, operating model and stewardship | `[B]`; operating detail is later |
| Policy stack | Hierarchy now; policy text later | `[B]` / `[C]` (`DG.2` is the NDMO policy control — not implemented here) |
| Data practices | Classification, quality, catalog/metadata, lineage, MDM, lifecycle — as **frameworks** | `[B]` mapped to NDMO domain names `[C]` |
| Measurement | KPIs and maturity model | later phase; NDMO `DG.7` is a related control `[C]` |
| Alignment | NDMO domain mapping and evidence approach | later pack; method starts in Phase 2 |

### 4.2 This documentation drop (Phase 0–2 only)

- Organization profile and assumed data landscape `[A]`.
- Program and governance scope.
- Vision, mission, objectives, and principles.
- Decision-right **classes** (not a full RACI).
- Policy hierarchy (not policy text).
- NDMO alignment **approach** (not a control-by-control compliance matrix).

---

## 5. Out of scope

| Excluded item | Reason |
| --- | --- |
| Building or configuring EMR, integration, catalog, DQ, or MDM tools | This is a governance framework, not an IT delivery program `[A]` / `[B]` |
| Named appointments of CDO or other officers | NDMO names these roles (`DG.4`) `[C]`; staffing is an operating-model decision (Phase 3+) |
| Full RACI, committee charters, job descriptions | Phase 3–4; NDMO *Organizational Manual* not retrieved `[NDMO verification required]` |
| Data classification of real or fictional datasets | Phase 5; NDMO classification process is `DC.3` `[C]` |
| Written cluster policies, standards, or SOPs | Phase 6; NDMO `DG.2` `[C]` |
| Data quality rules, catalog design, lineage graphs, MDM operating model | Phases 7–10 |
| Retention schedules and legal hold procedures | Phase 11 |
| KPI targets, maturity scores, three-year initiative roadmap | Phases 12–13 |
| Official NDMO compliance audit, evidence pack, or score | Phase 14 and live operations; NDMO describes annual entity self-assessment `[C]` — this repo does not perform it |
| Legal advice on PDPL, MOH circulars, or NCA ECC | Outside this program |
| Invented NDMO controls or fake control IDs | Explicit program rule |

---

## 6. Data and organizational boundary (summary)

Full landscape: [`data-landscape.md`](data-landscape.md). Governance boundary: [`../02-governance-strategy/governance-scope.md`](../02-governance-strategy/governance-scope.md).

| Boundary | Working statement | Label |
| --- | --- | --- |
| Data in program view | All cluster data regardless of form (electronic, paper, image, voice, email, and other recorded forms), consistent with NDMO’s stated scope for government data | `[C]` for NDMO wording; `[A]` that Rafid data is government/cluster data |
| Facilities | All hospitals, primary care centers, and cluster corporate functions listed in the organization profile | `[A]` |
| Partners | Business partners handling cluster/government data are **in the alignment conversation**; partner contracts are not drafted here | `[C]` NDMO Purpose and Scope extends to business partners; `[A]` that Rafid has such partners |
| Personal data | Patient, staff, and other identifiable data are in the governance landscape | `[A]`; PDPL applicability `[NDMO verification required]` for mapping detail |

---

## 7. Success conditions for Phase 0–2 (documentation only)

Phase 0–2 is complete when:

1. The fictional organization and data landscape are written and labeled `[A]`.
2. Program inclusions and exclusions are explicit.
3. Vision, mission, objectives, and principles are recorded without implying implementation.
4. Decision-right **classes** and policy **hierarchy** are recorded without issuing policies or a RACI.
5. NDMO alignment is described as a **method**, with official domain names and only verified control IDs.
6. No Phase 3+ design has been smuggled in.

These are documentation exit criteria `[B]`. They are not NDMO specification completion criteria.

---

## 8. Intentionally unresolved

| Item | Why it is open |
| --- | --- |
| Exact legal status of a real MOH health cluster under NDMO | `[NDMO verification required]` |
| Which NDMO specifications are P1/P2/P3 for each later workstream | Official counts exist `[C]`; initiative mapping is Phase 13 |
| Budget, staffing model, and tool selection | Not a Phase 0–2 decision |
| Sector overlays (MOH, CBAHI, SFDA, NCA) | May apply in a real cluster; not designed here `[NDMO verification required]` |
| Whether additional entity-level principles beyond NDMO’s eight will be formally adopted | NDMO permits entity-level additions (`DG.1.2`) `[C]`; healthcare additions in this repo are **candidates only** |

---

## 9. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO, *Data Management and Personal Data Protection Standards*, v1.5, January 2021 | Purpose and Scope; Domain 1 definition; `DG.1`, `DG.2`, `DG.4`, `DG.7`; business-partner extension |
| `[B]` | Program-scoping practice for governance frameworks (DAMA-style “what is / is not in the program”) | Structure of this document |
| `[A]` | Rafid Health Cluster portfolio assumptions | Entity, exclusions, current-state premise |
