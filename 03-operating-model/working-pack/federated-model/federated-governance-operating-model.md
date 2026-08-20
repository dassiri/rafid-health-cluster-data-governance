# Federated Governance Operating Model (Applied Working Pack)

**Document ID:** RHC-DG-P3-WP-011  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** A new operating model, hospital-level boards, or hybrid-as-headline-model

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Locked sources:** [`../../01-operating-model-overview.md`](../../01-operating-model-overview.md) · [`../../03-role-catalogue.md`](../../03-role-catalogue.md) · [`../../../04-ownership-stewardship/02-enterprise-ownership-matrix.md`](../../../04-ownership-stewardship/02-enterprise-ownership-matrix.md)

---

## 1. Purpose

Show how the **already approved** federated-by-domain model operates in practice: what stays central, what sits with domain Owners and Stewards, and what IT implements.

This file does **not** replace Phase 3. The approved headline remains:

**Federated, by data domain — not by hospital.** `[B]`

Hospitals and PHCs participate **through domains**. They do not each run a separate governance programme.

---

## 2. Operating shape (applied)

```text
Enterprise Governance
(DMC · CDO · DMO)
        ↓
Policies / Standards / Decision Rights
(POL-001 · STD-001–005 · PRC-001–006 · Phase 3 RACI)
        ↓
Domain Data Owners
(eight Phase 4 titles; one A per domain)
        ↓
Business Data Stewards
        ↓
Operational Governance
(domain huddles · issue / classification / catalog / lineage packs)
        ↓
IT / Data Custodian
        ↓
Technical Implementation
(systems · access provisioning · technical metadata / lineage · platform controls)
```

A “strong centre” is **not** Centralized: the DMO does **not** become Data Owner of laboratory results, encounter notes, or claims.

---

## 3. Why this shape (locked rationale, applied)

| Alternative | Why it is not the Rafid headline |
| --- | --- |
| Centralized | Clinical and corporate meaning would sit in a central office; IT becomes de facto owner — contradicts Phase 2/3 |
| Decentralized (by hospital) | Recreates duplicate patients, split codes, conflicting dictionaries; cannot serve an entity DMO and DMC `[C]` names |
| Hybrid as headline | Useful later as an **MDM pattern** (Phase 10), not as the enterprise model — too vague on “what is central?” |
| **Federated-by-domain (approved)** | One cluster rulebook; business ownership preserved; facilities join through domains |

NDMO names a Data Management Office **and** Business Data Executives / Stewards `[C]`. That is a federated shape: centre + domains. Specification-level mapping remains `[NDMO verification required]`.

---

## 4. Federated boundaries

### 4.1 Enterprise / central responsibilities

Held by **DMC / CDO / DMO** (and aligned PDPO, Compliance Officer, Legal, ODIA where the locked RACI already consults them).

| Responsibility | Accountable seat (locked) | What central does **not** do |
| --- | --- | --- |
| Governance framework and strategy | DMC **A**; CDO **R** | Rewrite domain definitions |
| L3 Policy | DMC **A** | Operate as Data Owner of a domain |
| Enterprise standards and methods | CDO **A** unless the standard changes Policy intent | Override Owner on business meaning |
| Catalog **programme** / metadata **standards** | CDO **A** | Own domain catalog **content** |
| Lineage **programme** | CDO **A** | Own business correctness of a domain flow |
| Issue / exception **process** and registers | DMO operates; DMC **A** for Policy exceptions | Close domain quality issues as Owner |
| Cross-domain escalation and mediation | DGO / CDO process; DMC if residual | Pick a clinical definition in place of Owners |
| KPI reporting and alignment evidence design | CDO **A**; CO **R** on self-assessment work | Invent measured Rafid KPI results |
| NDMO coordination / verification register (project) | CDO **A** | Claim NDMO compliance |
| Training design | DMO | Replace Owner participation |

### 4.2 Domain responsibilities

Held by **Data Owner (A)** and **Business Data Steward (R)** for one of the eight Phase 4 domains, cluster-wide.

| Responsibility | Owner | Steward |
| --- | --- | --- |
| Business definitions | **A** | **R** drafts |
| Ownership participation / Steward nomination | **A** (DMC ratifies Owner seats) | Executes |
| Stewardship operating packs | Accepts | **R** |
| Domain data quality rules, CDE confirmation, issue closure | **A** | **R** |
| Dataset classification / reclassification | **A** | **R** packs |
| Domain metadata / catalog **content** | **A** | **R** |
| Domain lineage **business correctness** | **A** | **R** metadata |
| In-policy access and routine business sharing | **A** | **R** |
| Domain lifecycle / retention **business** decision | **A** | **R** |
| MDM meaning for that master domain | **A** | **R** |

Domain list (unchanged) `[A]`:

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Provider / Clinician Data  
4. Financial / Billing & Claims Data  
5. Human Resources / Workforce Data  
6. Supply Chain & Asset Data  
7. Quality & Patient Safety Data  
8. Reference / Organizational Master Data  

DMO may **host** the Domain 8 Steward. DMO is still **not** the Owner. Owner remains Strategy & Planning Director.

### 4.3 Technical responsibilities

Held by **IT / Data Custodian** (IT Data Steward). CIO is the executive for systems and a DMC **peer** of the CDO — not Data Owner.

| Responsibility | Custodian role |
| --- | --- |
| Systems of record operation | **R** technical |
| Access **provisioning** after Owner (or DMC exception) decision | **R** |
| Technical metadata accuracy | **R** (never **A** for meaning) |
| Technical lineage information where applicable | **R** (Year-1 conceptual) |
| Implement quality rules and handling controls in systems | **R** with cybersecurity coordination |
| Platform / backup / operational controls | **R** per policy |
| Security veto | May refuse NCA-aligned violations via **CISO path and CDO** — still not classification or meaning **A** |

NDMO Domain 15 remains under NCA `[C]`. Governance coordinates; it does not replace NCA control design.

---

## 5. Interaction: central × domain × technical

Worked path for a **Patient identifier** used in encounter and claims `[A]`:

| Layer | Who | What they decide or do |
| --- | --- | --- |
| Central | DMO | One issue process, one catalog field standard, one lineage register method, KPI pack |
| Domain (Patient) | Patient Access & Experience Director **A**; Registration Steward **R** | Meaning of Patient ID / National ID; CDE-001/002 confirmation; duplicate-issue close |
| Domain (Clinical) | CMO **A**; HIM Steward **R** | Encounter uses the identifier; clinical documentation quality; classification of encounter notes |
| Domain (Financial) | CFO **A**; Revenue Cycle Manager **R** | Claims use of the identifier; charge-code quality; not a second Patient Owner |
| Technical | MPI / EMR / billing Custodians | Implement match/merge **after** Owner intent; provision access; record technical hops |

Cross-domain clash uses the locked mediation path. Consulted “losers” of contested ownership stay **C** (Phase 4). No shared **A**.

---

## 6. Decision-class mapping (Phase 2 applied)

| Class | Typical landing in the federated model |
| --- | --- |
| Operational | Steward execution; Owner decision in the domain huddle; Custodian implements |
| Tactical | DMO/CDO methods; Owner domain rules; Steward Forum recommendations |
| Strategic | Data Management Committee; CEO for residual / material regulatory |

---

## 7. What this model is not

- Not a live operating organization
- Not federated-by-hospital
- Not a new governance structure
- Not NDMO organization-control implementation
- Not IT ownership of business data

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 federated-by-domain choice | Model and split |
| `[A]` | Eight domains; Patient–Encounter–Claims example | Applied illustration |
| `[C]` | DMO, Committee, BDE/BDS, IT Data Steward **names**; Domain 15 NCA | Terminology; security boundary |
| `[NDMO verification required]` | Specification-level organization controls | Not claimed as implemented |
