# Phase 3 — Data Governance Operating Model

**Document ID:** RHC-DG-P3-000  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Named incumbents, policy text, or Phase 5 classification. Domain-to-title assignments are in [`../04-ownership-stewardship/`](../04-ownership-stewardship/).

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Phase purpose

Phase 3 defines **how data governance operates** inside the fictional Rafid Health Cluster `[A]`: the federated operating model, reporting lines, role catalogue, enterprise RACI, decision and escalation paths, forums, and end-to-end workflow.

It consumes Phase 2 decision-right **classes** (strategic / tactical / operational) and NDMO **role names**. Domain Owner titles are in Phase 4. This phase does not issue policies (Phase 6).

This is a governance framework artifact, not a software application.

---

## Status

**Approved / Implemented** — documentation only. No officers are appointed, no forums have met, and no NDMO compliance is claimed.

---

## Scope

**In scope**

- Federated-by-data-domain operating model `[B]`
- Governance structure and forums (titles only; no named people)
- Reporting lines for CDO, CIO, PDPO, and Compliance Officer
- Enterprise RACI for the approved activity set
- Decision and escalation paths
- Minimum forum cadences
- Operating workflow
- NDMO **name** mapping with verification limits

**Out of scope**

- Data Owner / domain assignment (documented in Phase 4, not in this folder’s design origin)
- Policy, standard, or SOP text (Phase 6)
- Dataset classification (Phase 5)
- KPI targets and maturity scores (Phase 12)
- Invented NDMO control numbers
- A CDO–CIO dotted “tooling” reporting line (rejected)

---

## Operating model summary

**Federated by data domain — not by hospital** `[B]`.

The centre (Data Management Office, CDO, Data Management Committee) sets one cluster rulebook. **Data Owners** are accountable for business meaning and quality in their domain. **Business Data Stewards** execute operational governance. **Data Custodians (IT)** implement systems. Hospitals and PHCs do not each run a separate governance programme.

NDMO names a Data Management Office, an Entity Data Management Committee, a Chief Data Officer, and related roles `[C]`. How those names map to specification-level control IDs is `[NDMO verification required]`. This phase does **not** claim that NDMO organization specifications are implemented, and it does **not** claim NDMO compliance.

---

## Files included

| File | Content |
| --- | --- |
| [01-operating-model-overview.md](01-operating-model-overview.md) | Model comparison and federated design |
| [02-reporting-lines.md](02-reporting-lines.md) | CDO, CIO, PDPO, Compliance Officer placement |
| [03-role-catalogue.md](03-role-catalogue.md) | Roles and forums (purpose, authority, rights) |
| [04-enterprise-raci.md](04-enterprise-raci.md) | Enterprise RACI (one Accountable per row) |
| [05-decision-escalation-model.md](05-decision-escalation-model.md) | Normal, conflict, exception, quality, regulatory paths |
| [06-governance-forums.md](06-governance-forums.md) | Four approved cadences |
| [07-operating-workflow.md](07-operating-workflow.md) | End-to-end issue/request flow |
| [08-interview-defensibility-notes.md](08-interview-defensibility-notes.md) | **INTERNAL / INTERVIEW PREPARATION** — not policy |
| [09-ndmo-role-mapping.md](09-ndmo-role-mapping.md) | Working title ↔ NDMO name; verification limits |
| [diagrams/org-reporting-lines.mmd](diagrams/org-reporting-lines.mmd) | Solid vs dotted reporting |
| [diagrams/escalation-flow.mmd](diagrams/escalation-flow.mmd) | Escalation hierarchy |
| [diagrams/forum-cadence.mmd](diagrams/forum-cadence.mmd) | Forum cadence |

---

## Relationship to Phase 4

Phase 3 defines **that** domain governance exists. Phase 4 documents the eight domains, one Owner per domain, stewards, and the domain decision RACI. See [`../04-ownership-stewardship/`](../04-ownership-stewardship/). This folder does not duplicate that map. Year-1 DMC standing membership in the role catalogue matches Phase 4 `[A]`.

---

## NDMO verification limitations

- Role **names** used here (CDO, Data Management Office, Business Data Executive, and others) are NDMO terminology `[C]`.
- **Control-level** identifiers are **not** treated as verified in Phase 3. Any control-level NDMO reference is `[NDMO verification required]`.
- NDMO *Organizational Manual* duty text was not retrieved `[NDMO verification required]`.
- PDPO versus PDPL DPO equivalence is `[NDMO verification required]`.
- ODIA / open data / FOI operating procedures for a healthcare cluster are `[NDMO verification required]`.
- This folder is **not** evidence that any NDMO specification is implemented. No compliance claim is made.
