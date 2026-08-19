# Stewardship Operating Model

**Document ID:** RHC-DG-P4-005  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented  
**Does not decide:** Numeric SLAs, headcount formulas, or named incumbents

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document describes how Business Data Stewards **operate** under Data Owners in the fictional Rafid Health Cluster `[A]`. NDMO name: Business Data Steward `[C]`. Specification-level duties `[NDMO verification required]`.

**Capacity is qualitative.** This file does **not** introduce numeric SLAs.

---

## 2. Steward appointment `[B]`

- The **Data Owner** nominates the Business Data Steward for that domain.
- The **DMO** confirms the nomination is complete (one steward seat recorded, Owner named, domain named) and records it in the Steward Registry.
- The **CDO** does not become the Owner by accepting the registration.
- IT Data Stewards / Custodians are appointed on the **technical** side; they are not a substitute for the Business Data Steward.

---

## 3. DMO Steward Registry `[B]`

The Data Management Office keeps a **Steward Registry** (design control — **not** an NDMO control ID):

| Field (minimum) | Purpose |
| --- | --- |
| Domain name | Which of the eight domains |
| Data Owner title | Accountable role |
| Business Data Steward title | Executing role |
| Custodian function (system class) | Technical contact — not Owner |
| Date registered / last reviewed | Lifecycle |
| Status | Active / pending reassignment |

The registry is an operating artifact. Creating it in live operations is not claimed here.

---

## 4. Steward responsibilities `[B]`

Aligned to Phase 3 operational class and the Phase 4 decision matrix:

- Draft data definitions for Owner approval
- Propose and monitor data-quality rules (Owner remains **A**)
- Prepare classification packs for Owner approval (Phase 5 will define the method’s application; not started here)
- Prepare in-policy access and business-sharing packs
- Maintain domain catalog/metadata content for Owner approval
- Investigate data issues and coordinate Custodian fixes
- Coach Data Consumers
- Escalate to the Data Owner when a decision exceeds steward authority

Stewards **do not**: approve L3 policy; act as a second Data Owner; mark their own domain’s privacy review (**A = PDPO** on sharing privacy review).

---

## 5. Competencies `[B]`

Qualitative expectations for a Business Data Steward:

- Domain literacy (can explain what “good” looks like in that domain)
- Ability to work with HIM, clinical, financial, or HR language as applicable `[A]`
- Process discipline (packs, registries, issue notes)
- Working knowledge of the cluster policy hierarchy (Phase 2) — not a substitute for Legal or PDPO
- Ability to distinguish business meaning (Owner) from system behaviour (Custodian)

IT Data Stewards / Custodians need system and integration competence; they are not required to own business definitions.

---

## 6. Capacity considerations (qualitative only)

Steward time must be **visible and protected** relative to the domain’s operational load `[B]`. Signals that capacity is insufficient (no numeric thresholds):

- Recurring issues ageing without Owner decision
- Catalog/definition backlog called out in Steward Forum
- Owner unavailable so packs stall
- One person covering steward work for multiple high-conflict domains without DMO visibility

Response is **escalation and Owner/DMO discussion**, not a hidden SLA number. Numeric SLAs were considered in Phase 4 and **rejected**.

Reference / Organizational Master Data uses a DMO-based analyst as Steward. That is a **staffing location**, not DMO ownership. If that analyst’s DMO coordination work crowds out steward work, the Owner (Strategy & Planning Director) and CDO address capacity — they do not transfer **A** to the CDO.

---

## 7. Steward Forum interaction

Phase 3 Steward Forum (monthly, DGO chairs) `[B]`:

- Stewards bring cross-domain clashes, standard **proposals**, and ageing-issue themes
- The Forum does **not** reassign ownership
- The Forum does **not** approve L3 policy
- Outputs are recommendations to Owners and/or CDO

Domain huddles (Owner + Steward + Custodian) remain the place for in-policy domain decisions. Huddles start when Owners and Stewards are appointed in live operations (not claimed here).

---

## 8. Escalation to Data Owner

Steward → Data Owner when:

- A definition, quality rule, classification application, in-policy access, business share, catalog entry, issue closure, or retention **decision** is required
- The steward cannot complete a pack (missing evidence, conflicting SMEs)
- A consumer disputes an operational application of an approved rule

The Owner remains **A** on those rows (except access **exception** and sharing **privacy review**).

---

## 9. Escalation through governance forums

If the Owner does not decide, or domains conflict, Phase 3 paths apply `[B]`:

```text
Business Data Steward
  → Data Owner
    → Data Governance Officer (mediate / SLA-breach list — qualitative ageing, not a numeric SLA)
      → CDO
        → Data Management Committee
          → Cluster CEO (residual / material regulatory)
```

Privacy incidents still **parallel-notify** PDPO (Phase 3). Cybersecurity incidents remain on the CISO / NCA path `[C]` Domain 15 mandate; governance coordinates.

---

## 10. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 4 stewardship model; Phase 3 forums | Operating design |
| `[A]` | Rafid titles and DMO-hosted reference steward | Examples |
| `[C]` | Business Data Steward **name**; Domain 15 NCA note | Terminology; cyber parallel path |
| `[NDMO verification required]` | Specification-level steward duties | Not cited as IDs |
