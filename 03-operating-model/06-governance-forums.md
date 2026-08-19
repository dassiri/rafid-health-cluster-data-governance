# Governance Forums

**Document ID:** RHC-DG-P3-006  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Per-hospital boards or architecture boards. Year-1 DMC standing membership is the Phase 4 finalized list `[A]`.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **minimum forums** needed to operate the federated model without excessive bureaucracy `[B]`.

**Approved set: four cadences**

1. Data Management Committee (formal)
2. Steward Forum (formal)
3. Domain huddles (operating cadence, not a second Council)
4. DMO operations huddle (triage only)

There is **no** per-hospital Data Governance Board. That would federate by facility and recreate silos `[A]` / `[B]`.

Diagram: [`diagrams/forum-cadence.mmd`](diagrams/forum-cadence.mmd).

The Data Management Committee uses the NDMO name Entity Data Management Committee `[C]`. Forum procedures in the Organizational Manual are `[NDMO verification required]`.

---

## 2. Data Management Committee

| Element | Design |
| --- | --- |
| **Purpose** | Strategic oversight of the cluster data agenda |
| **Participants** | **Year-1 composition finalized in Phase 4** `[A]`. **Chair:** Cluster CEO. **Standing members:** CDO; CIO; PDPO; Compliance Officer; Patient/Person Master Data Owner; Clinical/Medical Records Data Owner; Financial/Billing & Claims Data Owner. **By invitation when relevant:** Provider/Clinician, HR/Workforce, Supply Chain & Asset, Quality & Patient Safety, and Reference/Organizational Master Data Owners. **Secretariat (non-member):** Data Governance Officer. Title map: [`../04-ownership-stewardship/02-enterprise-ownership-matrix.md`](../04-ownership-stewardship/02-enterprise-ownership-matrix.md). |
| **Decisions** | Strategy; L3 policy; material exceptions; residual sharing risk; Owner non-participation |
| **Frequency** | Quarterly + extraordinary session for material regulatory or patient-safety data incidents |
| **Inputs** | KPI pack; issue themes; exception papers; alignment status |
| **Outputs** | Decisions; actions; risk acceptances |

The CDO does **not** chair this forum `[B]`.

---

## 3. Steward Forum

| Element | Design |
| --- | --- |
| **Purpose** | Cross-domain tactical coordination |
| **Participants** | Data Governance Officer (chair); Business Data Stewards; Custodian leads; PDPO as needed |
| **Decisions** | Standard **proposals**; clash detection; catalog/lineage practice; training needs — **not** L3 policy |
| **Frequency** | Monthly |
| **Inputs** | Issue statistics; draft standards; Owner papers |
| **Outputs** | Recommendations to CDO / Data Owners |

---

## 4. Domain huddles

| Element | Design |
| --- | --- |
| **Purpose** | Run one data domain across facilities |
| **Participants** | Data Owner; Business Data Steward(s); Custodian for that domain; invited consumers |
| **Decisions** | Definitions; data-quality rules; in-policy access/sharing; issue closure |
| **Frequency** | Biweekly or monthly by domain risk |
| **Inputs** | Issues; definition drafts; quality metrics |
| **Outputs** | Domain decisions (logged) |

Domain huddles use the Phase 4 Owner/Steward titles. This file defines the cadence. Live huddles are not claimed.

---

## 5. DMO operations huddle

| Element | Design |
| --- | --- |
| **Purpose** | Intake triage only — not a governance board |
| **Participants** | CDO and/or Data Governance Officer; coordinator |
| **Decisions** | Routing; SLA-breach list — **no** policy |
| **Frequency** | Weekly |
| **Inputs** | Intake queue |
| **Outputs** | Agenda items for Steward Forum or Data Management Committee |

---

## 6. What is not a Phase 3 forum

- Hospital-level Data Governance Committee
- Data architecture board (NDMO Data Architecture and Modeling domain is a later workstream)
- Open Data / FOI working group as a standing extra board (ODIA is not a Year-1 standing DMC member; consult when that agenda applies; operating procedures `[NDMO verification required]`)

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 Implementation Brief | Four cadences, no hospital boards |
| `[C]` | NDMO Standards v1.5 — Entity Data Management Committee **name** | Committee naming |
| `[A]` | Multi-facility footprint | Why not per-hospital boards |
| `[NDMO verification required]` | Organizational Manual forum duties | Not retrieved |
