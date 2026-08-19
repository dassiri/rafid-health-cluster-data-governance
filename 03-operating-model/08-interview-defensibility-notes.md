# Interview Defensibility Notes

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P3-008  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented (documentation)  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not appoint anyone and does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## How to introduce Phase 3 (30 seconds)

> “Phase 3 is the operating model for a fictional Saudi health cluster. I chose federated by data domain, not by hospital, because the cluster already shares one EMR and the same patient across sites. The CDO reports to the CEO; the CIO is a peer. The CEO chairs the Data Management Committee so the CDO does not oversee themselves. Data Owners own meaning and quality; stewards execute; IT implements. I do not claim NDMO compliance, and I do not invent control numbers.”

---

## Decision log (defend these, not a policy)

| # | Decision | Why | Alternative considered | Reason rejected |
| --- | --- | --- | --- | --- |
| 1 | **Federated by data domain, not by hospital** `[B]` | Cluster EMR + shared patients `[A]`; NDMO names a centre **and** Business Data Executives / Stewards `[C]` | Centralized | Clinical meaning cannot sit in a central office; IT becomes owner |
| | | | Decentralized by hospital | Rebuilds silos; no entity DMO/Committee |
| | | | Hybrid as headline | Vague; keep hybrid only later for selected MDM objects (Phase 10) |
| 2 | **CDO reports to Cluster CEO; CIO is a peer** `[B]` | Entity-wide agenda; NDMO describes CDO-led annual assessment `[C]`; CIO remains custodian executive | Report to CIO | Governance becomes an IT project; contradicts business ownership |
| | | | Report to CMO only | Misses finance/HR/revenue |
| | | | CDO–CIO dotted “tooling” line | Rejected; blurs peer relationship |
| 3 | **CEO chairs the Data Management Committee; CDO does not chair own oversight** `[B]` | Separation of run vs oversee | CDO chairs the Committee | Self-oversight; weak in interview |
| 4 | **Local titles mapped to NDMO role names** | Phase 2 rule; interview can say both working title and NDMO name `[C]` | Invent titles that replace CDO / BDE | Silent second hierarchy |
| 5 | **One A per row; Owner A for meaning, quality, dataset classification, in-policy access/sharing** `[B]` | Business ownership; NDMO sharing process includes Business Data Executive approval `[C]` | CIO A for classification or quality | IT owning business data |
| 6 | **Committee A for strategy/policy/material exceptions; CDO R** `[B]` | NDMO requires senior-executive / committee strategy approval `[C]` | CDO A for policy | CDO writing and approving own policy |
| 7 | **Four cadences only** (Committee, Steward Forum, domain huddles, DMO huddle) `[B]` | 4 hospitals + 18 PHCs `[A]` cannot each have a board | Hospital DG committees | Bureaucracy; federated-by-facility |
| 8 | **Catalog A = CDO; tool R = Custodian** `[B]` | Programme vs platform | CIO A for catalog | Catalog becomes an IT inventory |
| 9 | **Lineage A = CDO; R = Custodian** `[B]` | Technical capture is IT work; the standard is enterprise | Owner A for all lineage | Owners cannot implement pipelines; they remain **C** for completeness |
| 10 | **Material regulatory A = CEO; R = CDO** `[B]` | Entity risk; CDO still leads the work as NDMO describes for the assessment `[C]` | CDO A for all regulator-facing incidents | Under-powered if CEO is not accountable |
| 11 | **ODIA seat kept; year-1 operating model thin** | NDMO names the role `[C]`; hospital FOI/open data not designed | Drop ODIA | Inventing a gap in the named role set |
| 12 | **PDPO solid to CEO, dotted to CDO** `[B]` | Privacy vs infrastructure | PDPO under CIO only | Conflicts with protection-by-design as a data agenda `[C]` principle |
| 13 | **Compliance Officer solid to Legal/Internal Control, dotted to CDO** `[B]` | CDO should not mark their own homework | CO solid to CDO | Weak challenge |

---

## Answers that must not be given

| Do not say | Say instead |
| --- | --- |
| “We are NDMO compliant.” | “Phase 3 is an operating design. No specification has been evidenced as implemented.” |
| “This org chart is a verified NDMO control.” | “NDMO **names** a CDO. Control-level IDs are `[NDMO verification required]` in this phase. The CEO reporting line is `[B]`.” |
| “I appointed a CDO named …” | “Titles only. No incumbents. Data Owner **titles** are in Phase 4; no people are appointed.” |
| “Each hospital has its own Data Governance Board.” | “That was rejected. Federation is by **domain**, not facility.” |
| “IT owns patient data quality.” | “The Data Owner is Accountable; IT is Responsible for system fixes.” |
| “Open by Default means we publish clinical records.” | NDMO Open by Default is adopted `[C]`; classification and other law constrain what can be public. Dataset decisions are Phase 5. |

---

## Suggested walkthrough

1. [`01-operating-model-overview.md`](01-operating-model-overview.md) — federated-by-domain
2. [`02-reporting-lines.md`](02-reporting-lines.md) — CEO / CDO / CIO / PDPO / CO
3. [`04-enterprise-raci.md`](04-enterprise-raci.md) — one A per row
4. [`05-decision-escalation-model.md`](05-decision-escalation-model.md) — five paths
5. [`09-ndmo-role-mapping.md`](09-ndmo-role-mapping.md) — names vs unverified control IDs

---

## Known limits

- Rafid is fictional `[A]`.
- Organizational Manual not retrieved `[NDMO verification required]`.
- Phase 4 ownership is Designed / Documented; operational implementation and measured performance are not claimed.
- No compliance score.
