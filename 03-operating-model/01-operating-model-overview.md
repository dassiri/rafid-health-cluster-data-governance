# Operating Model Overview

**Document ID:** RHC-DG-P3-001  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Domain list, named Data Owners, or hospital-level governance boards

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved operating model for the fictional Rafid Health Cluster `[A]`: **Federated by data domain**. It compares alternatives briefly and states what is central versus domain-owned versus IT-owned.

It implements Phase 2 decision classes `[B]` (strategic / tactical / operational). See [`../02-governance-strategy/decision-rights.md`](../02-governance-strategy/decision-rights.md).

---

## 2. Approved model

**Recommendation (approved): Federated, by data domain — not by hospital.** `[B]`

The centre sets one cluster rulebook. Named **Data Owners** own meaning and quality in their domain. **Stewards** run day-to-day governance. **IT/Custodians** implement systems. Hospitals and PHCs do **not** each run a separate governance programme.

Illustrative domain names (Patient identity, Laboratory, Pharmacy, and similar) are **examples only** `[A]`. They are not a Phase 4 assignment.

---

## 3. Comparison of alternatives `[B]`

| Model | How it would work at Rafid | Fit |
| --- | --- | --- |
| **Centralized** | DMO/CDO owns definitions, quality, access, and classification for all data | Fast consistency; fails clinically — Medical Affairs, Lab, and Pharmacy will not treat a central office as owner of clinical meaning. IT becomes de facto owner. Contradicts Phase 2: IT is not accountable for business data. |
| **Decentralized** | Each hospital / department sets its own rules | Matches local habit `[A]` as-is; recreates duplicate patients, split lab codes, and conflicting EMR dictionaries. Cannot serve an entity-level Data Management Office and Data Management Committee `[C]`. |
| **Federated (approved)** | Central policy, standards, catalog rules, issue process; domain Owners/Stewards execute; facilities participate **through domains** | Fits cluster-wide EMR plus local operations. Preserves business ownership. Gives NDMO a real centre without pretending the centre owns every data element. |
| **Hybrid** | Some domains fully central (for example Patient ID), others federated | Useful later as an **MDM pattern** (Phase 10), not as the enterprise model. As the headline model it is vague (“what is central?”). |

---

## 4. Why federated-by-domain fits a multi-facility health cluster `[A]` + `[B]`

- Four hospitals, 18 PHCs, specialty centres, and one cluster EMR `[A]`: the **same patient** already crosses sites. Federating by **facility** would rebuild silos. Federating by **domain** matches how care and systems run.
- Clinical safety depends on business meaning sitting with clinical/corporate owners, not the CIO.
- NDMO names a Data Management Office **and** Business Data Executives / Stewards `[C]`. That is a federated shape: centre + domains. Specification-level mapping of those names is `[NDMO verification required]`.
- A “strong centre” is not Centralized: the DMO does not become Data Owner of laboratory results.

---

## 5. What stays central vs domain-owned vs IT `[B]`

| Central (DMO / CDO / Committee) | Domain (Owner + Steward) | IT / Custodian |
| --- | --- | --- |
| Strategy, policy, enterprise standards | Meaning, definitions, quality rules for the domain | Platform, access provisioning, technical lineage |
| Classification **method** | Classification **of datasets** in the domain | Enforcement of handling controls with cybersecurity |
| Catalog standard and catalog programme | Catalog content for the domain | Catalog tool operations |
| Issue/exception process; NDMO coordination | Issue resolution inside the domain | Fixes in systems |
| Training design; KPI pack | Domain metrics input | Technical operational metrics |

NDMO Domain 15 (Data Security and Protection) is under the National Cybersecurity Authority `[C]`. Governance **coordinates** with cybersecurity; it does not replace NCA control design.

---

## 6. Title mapping (no second hierarchy)

Phase 2 requires local titles to map to NDMO names `[A]` / `[C]`. Full catalogue: [`03-role-catalogue.md`](03-role-catalogue.md). Mapping and verification limits: [`09-ndmo-role-mapping.md`](09-ndmo-role-mapping.md).

| Rafid working title `[B]` | NDMO name `[C]` |
| --- | --- |
| Data Management Committee (working name: Data Governance Council) | Entity Data Management Committee |
| Data Management Office (working name: Data Governance Office) | Data Management Office |
| Chief Data Officer | Chief Data Officer |
| Data Governance Officer | Data Governance Officer |
| Data Owner | Business Data Executive |
| Business Data Steward | Business Data Steward |
| Data Custodian | IT Data Steward |
| Personal Data Protection Officer | Personal Data Protection Officer |
| Data Management Compliance Officer | Compliance Officer |
| Open Data and Information Access Officer | Open Data and Information Access Officer |
| Legal Advisor (data) | Legal Advisor |
| Executive Sponsor | Not an NDMO role name; NDMO requires senior-executive strategy approval `[C]` — sponsor title is `[B]` |
| Data Consumer | Not an NDMO-named role in the Standards role list `[B]`; control-level treatment `[NDMO verification required]` |

No named incumbents. Titles only.

---

## 7. Intentionally unresolved

- Which cluster titles are Data Owners — Phase 4
- How many domains exist — Phase 4
- Facility SMEs as stewards — Phase 4
- Year-1 depth of ODIA / FOI / Open Data operations `[NDMO verification required]`

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 Implementation Brief — federated-by-domain choice | Model and split of duties |
| `[C]` | NDMO Standards v1.5 — role and structure **names**; Domain 15 NCA note; senior-executive strategy approval | Terminology only |
| `[A]` | Rafid organization profile and landscape | Multi-facility premise |
| `[NDMO verification required]` | Specification-level control IDs; Organizational Manual duties | Not treated as verified in this phase |
