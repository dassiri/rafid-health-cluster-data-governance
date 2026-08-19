# Phase 4 — Data Ownership and Stewardship

**Document ID:** RHC-DG-P4-000  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented  
**Does not decide:** Dataset classification (Phase 5), policy text (Phase 6), or named incumbents

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Purpose

Phase 4 assigns **enterprise data domains** to Data Owners and Business Data Stewards for the fictional Rafid Health Cluster `[A]`. It operationalizes the Phase 3 federated-by-domain model: one accountable Owner per domain, cluster-wide, with stewards executing and IT remaining a custodian.

This is a governance framework artifact, not a software application. It does not claim NDMO compliance.

---

## Scope

**In scope**

- Eight approved data domains and their Owner / Steward titles `[A]`
- Ownership principles and decision RACI `[B]`
- Stewardship operating model (qualitative capacity; no numeric SLAs)
- Ownership lifecycle and governance design controls `[B]`
- Year-1 Data Management Committee composition `[A]` (recorded here; DMC membership cell updated in the Phase 3 role catalogue)
- Domain-level NDMO name alignment only

**Out of scope**

- Phase 5 classification of datasets
- Policy / SOP text
- Numeric steward SLAs
- Shared / dual-Accountable ownership
- Hospital-level ownership boards
- Invented NDMO control IDs

---

## Domain ownership model

Exactly **one** Data Owner per domain. Ownership is **enterprise-wide** (the cluster), not hospital-by-hospital `[B]`. Titles are fictional cluster roles `[A]`. NDMO name for the Owner role is Business Data Executive `[C]`. Specification-level role requirements are `[NDMO verification required]`.

| # | Domain | Data Owner | Business Data Steward |
| --- | --- | --- | --- |
| 1 | Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access |
| 2 | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) |
| 3 | Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator |
| 4 | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager |
| 5 | Human Resources / Workforce Data | HR Director | HR Operations Manager |
| 6 | Supply Chain & Asset Data | Supply Chain Director | Inventory / Procurement Manager |
| 7 | Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) | Quality Improvement Manager |
| 8 | Reference / Organizational Master Data | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO |

IT Data Stewards / Custodians are **not** business Data Owners.

The DMO coordinates the framework. It is **not** the operational Data Owner of a business domain. The Reference / Organizational Master Data **steward** may sit in the DMO; the **Owner** remains the Strategy & Planning Director.

---

## Stewardship model

Business Data Stewards execute day-to-day governance (definitions drafts, quality monitoring, classification packs, catalog content, issue investigation) `[B]`. NDMO name: Business Data Steward `[C]`.

Capacity is **qualitative**. This phase does **not** set numeric SLAs.

Stewards escalate to their Data Owner, then through Phase 3 forums (Steward Forum → CDO → Data Management Committee).

---

## Relationship to Phase 3

Phase 3 defined federated-by-domain structure, decision classes, enterprise RACI, forums, and role **types**. Phase 4 **fills in** Owner and Steward titles and the domain decision matrix. It does not change CDO reporting, the federated model, or IT-as-custodian.

Year-1 DMC standing membership is finalized in this phase `[A]` and copied into [`../03-operating-model/03-role-catalogue.md`](../03-operating-model/03-role-catalogue.md).

---

## Relationship to Phase 5

Phase 5 applies the approved Rafid classification model: Public, Internal, Confidential, and Restricted `[A][B]`. These are Rafid's entity-level classification proposal and are not presented as NDMO national classification tiers. NDMO classification requirements remain subject to `[NDMO verification required]`.

Phase 4 only names **who is Accountable** for classification **decisions** in each domain. No dataset is classified here. Phase 5 is Designed / Documented; operational implementation and measured performance are not claimed.

---

## NDMO verification limitations

- Role **names** (Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office, Entity Data Management Committee) are `[C]`.
- Mapping those names to specification-level control IDs is `[NDMO verification required]`. Phase 4 does **not** cite unverified control IDs.
- Assigning a Rafid title (for example CMO) to a domain is `[A]` / `[B]`, not an NDMO mandate.
- Organizational Manual job content is `[NDMO verification required]`.
- No compliance claim is made.

---

## Files included

| File | Content |
| --- | --- |
| [01-domain-ownership-detail.md](01-domain-ownership-detail.md) | Per-domain Owner, Steward, scope, consulted parties |
| [02-enterprise-ownership-matrix.md](02-enterprise-ownership-matrix.md) | One-page domain × Owner × Steward matrix |
| [03-ownership-decision-matrix.md](03-ownership-decision-matrix.md) | Ten-row ownership decision RACI |
| [04-domain-ownership-raci.md](04-domain-ownership-raci.md) | Same RACI applied to all eight domains |
| [05-stewardship-operating-model.md](05-stewardship-operating-model.md) | Appointment, registry, competencies, capacity, escalation |
| [06-ownership-lifecycle.md](06-ownership-lifecycle.md) | Restructuring, split, systems, transfer, departure, new domain |
| [07-ownership-governance-controls.md](07-ownership-governance-controls.md) | Registries and review controls (`[B]` — not NDMO controls) |
| [08-ndmo-alignment.md](08-ndmo-alignment.md) | Domain-level alignment only |
| [09-interview-defensibility.md](09-interview-defensibility.md) | **INTERNAL / INTERVIEW PREPARATION** |
| [10-unresolved-decisions.md](10-unresolved-decisions.md) | Four Phase 4 items — **closed** |

---

## Status

**Implemented** — documentation only. No people are appointed. No datasets are classified. Phase 5 is Designed / Documented; operational implementation and measured performance are not claimed.
