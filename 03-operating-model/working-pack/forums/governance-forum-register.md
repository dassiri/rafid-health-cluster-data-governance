# Governance Forum Register

**Document ID:** RHC-DG-P3-WP-008  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** New forums, hospital boards, architecture boards, or a change to Year-1 DMC membership

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Locked source:** [`../../06-governance-forums.md`](../../06-governance-forums.md)

---

## 1. Purpose

Register the **four approved cadences** as a practical forum operating record: purpose, participants, decision types, inputs, outputs, frequency, escalation role, and evidence.

This file does **not** create a fifth forum. It does **not** invent a Privacy Committee, Data Council, or per-hospital Data Governance Board.

Frequency is the Phase 3 designed cadence. As a live operating rhythm it is **Proposed / Illustrative**. Live meetings are not claimed.

---

## 2. Approved set (unchanged)

1. Data Management Committee (formal)
2. Steward Forum (formal)
3. Domain huddles (operating cadence, not a second Council)
4. DMO operations huddle (triage only)

There is **no** per-hospital Data Governance Board. That would federate by facility and recreate silos `[A]` / `[B]`.

---

## 3. Forum records

### 3.1 Data Management Committee

| Element | Applied record |
| --- | --- |
| **Forum name** | Data Management Committee (working name: Data Governance Council) |
| **NDMO name** `[C]` | Entity Data Management Committee |
| **Purpose** | Strategic oversight of the cluster data agenda |
| **Participants** | **Chair:** Cluster CEO. **Standing members (Phase 4 Year-1):** CDO; CIO; PDPO; Compliance Officer; Patient/Person Master Data Owner; Clinical/Medical Records Data Owner; Financial/Billing & Claims Data Owner. **By invitation:** Provider/Clinician, HR/Workforce, Supply Chain & Asset, Quality & Patient Safety, Reference/Organizational Master Data Owners. **Secretariat (non-member):** Data Governance Officer. CDO does **not** chair. |
| **Decision types** | Strategy; L3 policy; material exceptions; residual sharing/openness risk; Owner non-participation. Tactical standards **endorsed** only when they change risk appetite or conflict with policy. **No new DMC class.** |
| **Inputs** | KPI pack; issue themes; exception papers; alignment / verification status |
| **Outputs** | Decisions; actions; risk acceptances |
| **Frequency** | Quarterly + extraordinary session for material regulatory or patient-safety data incidents. **Proposed / Illustrative.** |
| **Escalation role** | Receives policy, residual-risk, and unresolved cross-domain cases from CDO. Escalates unresolved / entity risk to Cluster CEO as Chair. Regulatory material risk → CEO + Legal + PDPO in parallel (Committee is **informed**; it does not delay incident notification). |
| **Evidence / records** | DMC decision; exception register update; strategy/policy approval record (designed — not live minutes) |

### 3.2 Steward Forum

| Element | Applied record |
| --- | --- |
| **Forum name** | Steward Forum |
| **Purpose** | Cross-domain tactical coordination |
| **Participants** | Data Governance Officer (chair); Business Data Stewards; Custodian leads; PDPO as needed |
| **Decision types** | Standard **proposals**; clash detection; catalog/lineage practice; training needs. **Not** L3 policy. **Not** ownership reassignment. |
| **Inputs** | Issue statistics; draft standards; Owner papers; lineage/catalog completeness themes |
| **Outputs** | Recommendations to CDO / Data Owners |
| **Frequency** | Monthly. **Proposed / Illustrative.** |
| **Escalation role** | Surfaces ageing and cross-domain clashes to DGO/CDO. Does not settle residual policy risk. |
| **Evidence / records** | Forum notes; recommendation log; items routed to domain huddle or DMC pack |

### 3.3 Domain huddles

| Element | Applied record |
| --- | --- |
| **Forum name** | Domain huddle |
| **Purpose** | Run one data domain across facilities |
| **Participants** | Data Owner; Business Data Steward(s); Custodian for that domain; invited Consumers |
| **Decision types** | Definitions; data-quality rules; in-policy access/sharing; classification application; issue closure; CDE confirmation; lineage business correctness; in-policy residual quality |
| **Inputs** | Issues; definition drafts; quality metrics; classification packs; catalog/lineage drafts |
| **Outputs** | Domain decisions (logged) |
| **Frequency** | Biweekly or monthly by domain risk. **Proposed / Illustrative.** |
| **Escalation role** | Owner decides in-policy. Cross-domain, Owner conflict, or Owner silence → DGO. Policy exception or residual → DMC. |
| **Evidence / records** | Domain decision log; Issue Record; Classification Registry; catalog/lineage row; CDE confirmation |

Illustrative Year-1 huddles used in this pack’s examples `[A]`: Patient / Person Master; Clinical / Medical Records; Financial / Billing & Claims.

### 3.4 DMO operations huddle

| Element | Applied record |
| --- | --- |
| **Forum name** | DMO operations huddle |
| **Purpose** | Intake triage only — **not** a governance board |
| **Participants** | CDO and/or Data Governance Officer; coordinator |
| **Decision types** | Routing; qualitative SLA-breach list. **No** policy. **No** domain meaning. |
| **Inputs** | Intake queue; incomplete packs; ageing list |
| **Outputs** | Agenda items for Steward Forum or Data Management Committee; routed Steward/Owner actions |
| **Frequency** | Weekly. **Proposed / Illustrative.** |
| **Escalation role** | First tactical hop after Owner-level failure: DGO → CDO. Material regulatory items are parallel-notified; they do not wait for this huddle. |
| **Evidence / records** | Intake/routing log (designed artifact; no ticketing product is claimed) |

---

## 4. What is not a Phase 3 forum (unchanged)

- Hospital-level Data Governance Committee
- Data architecture board
- Open Data / FOI working group as a standing extra board
- Privacy Committee / Data Council / domain committees other than the domain huddle

ODIA is consulted when that agenda applies. ODIA is **not** a Year-1 standing DMC member. Operating procedures remain `[NDMO verification required]`.

---

## 5. Forum-to-decision map (working)

| If the decision is… | It lands in… |
| --- | --- |
| In-policy domain meaning, classification, quality close, catalog content | Domain huddle |
| Cross-domain clash, standard proposal, practice | Steward Forum (recommend) → Owner or CDO |
| Routing / ageing list | DMO operations huddle |
| Strategy, L3 policy, material exception, residual sharing risk, Owner non-participation | Data Management Committee |
| Residual the Committee cannot settle; material regulatory **A** | Cluster CEO (not a fifth forum) |

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Phase 3 four cadences | Register |
| `[A]` | Year-1 DMC composition; example domains | Participants |
| `[C]` | Entity Data Management Committee **name** | Naming |
| `[NDMO verification required]` | Organizational Manual forum duties | Not retrieved |
