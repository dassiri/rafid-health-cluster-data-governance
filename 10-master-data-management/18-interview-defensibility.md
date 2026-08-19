# Interview Defensibility — MDM

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P10-018  
**Phase:** 10 — Master data management  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## What is MDM?

MDM is **governance of shared business identities** so Patient, Provider, and (lightly) Facility mean the same thing across systems `[B]`. In this repo it is **conceptual**. It is not SAP MDG, Reltio, or a hub.

NDMO names Reference and Master Data Management as a domain **name** `[C]`. Specific requirements remain `[NDMO verification required]`.

---

## Difference between Master Data and Reference Data?

**Master** = persistent identity (who/what the party or place **is**). **Reference** = allowed **codes** (diagnosis set, claim status, gender). Both need governance. **MDM ≠ RDM.** Item-type remains **reference** at this maturity.

---

## Difference between Master Data and Transaction Data?

**Master** persists (Patient). **Transaction** happens (Encounter, Claim, Payment, Appointment). Reuse alone does not make a claim into Core MDM.

---

## What is a golden record?

A **trusted master representation** after match and survivorship `[B]`. In Rafid it is **logical/governed**, not a mandatory physical table.

---

## Does golden record mean one physical database?

**No.** Not one database, not one platform, not one universal source system.

---

## How do you identify duplicates?

Conceptual **deterministic** match on strong identifiers, **conceptual** fuzzy as a hint, then **manual review**. Duplicates are quality **issues**. Owner oversees merge **intent**.

---

## Deterministic vs probabilistic matching?

Deterministic: same strong key (conceptually). Probabilistic/fuzzy: similarity **in principle only** — **no** weights, **no** numeric threshold, **no** ML matcher.

---

## What is survivorship?

Choosing which **attribute value** wins when sources disagree. **Per domain and attribute**, set by Owner and Steward. **No** universal system ranking.

---

## How do you determine the source of truth?

Distinguish System of Record, System of Reference, and Master Representation. Authority can be **per attribute**. There is **no** universal SoT rule.

---

## Who owns master data?

Phase 4 titles only: Patient Access & Experience Director; Medical Affairs Officer; Strategy & Planning Director. Steward = **Business Data Steward**. IT is not Owner. DMC is **not** routine approver of every entity.

---

## How does MDM improve data quality?

It attacks **uniqueness and cross-system consistency** of shared identities using Phase 7 dimensions and the existing issue path — not a second quality framework.

---

## Why start with Patient and Provider?

They are the identities on the care-to-claim chain (Phase 9 illustrative flow). Highest shared-process harm if duplicated `[A][B]`.

---

## Why is Facility only supporting scope?

Needed for **code consistency and context**, not a third matching/golden-record factory. Domain 8 already owns org reference. No extra MDM workstream.

---

## How would you implement MDM without buying a tool immediately?

Govern definitions, attribute authority, duplicate review, catalogs, and Owner-approved survivorship **principles** on **existing** systems. Buy a hub later if (and only if) operating evidence says copies cannot be governed logically. Naming Reltio is not implementation.

---

## Must-nots

| Do not say | Say instead |
| --- | --- |
| “We implemented Informatica MDM.” | Conceptual framework; no product. |
| “Golden record = one database.” | Logical governed representation. |
| “Match if score ≥ 90%.” | No numeric thresholds. |
| “DMC approves every Patient.” | Owner approves definition/rules; DMC existing escalation only. |
| “HR is Core MDM.” | Non-MDM at this maturity. |
| “Item master is Core MDM.” | Reference data at this maturity. |
| “We are NDMO-compliant on MDM.” | Domain **name** `[C]`; specifications unverified. |
