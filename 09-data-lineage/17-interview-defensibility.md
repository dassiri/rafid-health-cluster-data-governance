# Interview Defensibility — Data Lineage

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P9-017  
**Phase:** 9 — Data lineage  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## What is data lineage?

Lineage is a **governed description of how data moves**: Source → Transformation → Target → Consumer `[B]`. In Rafid Year-1 it is mainly **business** and **conceptual** lineage `[A][B]`. It is not a scanner, not a graph database, and not the data itself.

---

## Difference between lineage and metadata?

**Metadata** is the description of an asset (name, Owner, classification, definition). **Lineage** is the description of **relationships between** assets (and, selectively, fields). Lineage is stored as Phase 8 **Lineage Metadata** fields. Lineage is a kind of metadata; metadata is not only lineage.

---

## Difference between lineage and data catalog?

The **catalog** is the inventory of assets. **Lineage** is the movement story those assets participate in. The catalog may show Source → Target → Consumer at asset level. It does not become a technical lineage platform.

---

## Why is lineage important?

It supports impact analysis, ownership clarity, sharing context, quality root-cause, and a prompt to **reassess** classification `[B]`. That is a **governance benefit**. It is **not** claimed as satisfaction of a specific NDMO or sector specification `[NDMO verification required]`.

---

## How do you prioritize lineage?

Two steps `[A][B]`: a candidate appears when one or more of **nine** criteria fire; then Owner, Steward, and DMO **confirm** whether prioritized coverage is warranted. No numeric score. One criterion does **not** auto-make Critical Lineage.

---

## Why not build column-level lineage everywhere?

Cost, noise, and no Owner capacity `[B]`. Year-1 is Levels 1–2 on three domains. Level 4 is **selective** (CDE RCA, classification reassessment, investigation). Enterprise-wide field-level lineage is out of scope.

---

## Who owns lineage?

**Data Owner = Accountable** for business lineage correctness. **Business Data Steward = Responsible** for maintaining lineage metadata. **Custodian** supplies technical facts where applicable. **DMO** = methodology, registry, lineage-record quality. **DMC** uses **existing** Phase 3 rights only.

---

## How does lineage support impact analysis?

Quality failure in a source field → downstream dataset → process/report → KPI `[B]`. Example: invalid diagnosis → claims extract → rejections → illustrative Claim Rejection Rate `[A]`. Still use the Phase 6 quality issue path; prefer fix-the-source (Phase 7).

---

## How does lineage interact with classification?

Ask: does the downstream asset still contain the same sensitive elements? If so, the **Data Owner assesses** it with the **Phase 5** framework. Lineage **does not** auto-inherit the highest tier. Transformation, tokenization, field removal, aggregation, and de-identification **may** change sensitivity — still Owner **A**.

---

## How does lineage improve data quality?

It does not replace Phase 7. It shows **where a defect travels** so remediation hits the source and downstream Stewards are informed.

---

## How would you start lineage in healthcare?

MVP: three domains (Person, Clinical, Billing). Two use cases: registration→clinical→claims, and Claim Rejection Rate business lineage. Three assets. Focus the **Critical Lineage Register**. Generic “national claims interchange” — **not** NPHIES architecture. Do not buy Purview first.

---

## Must-nots

| Do not say | Say instead |
| --- | --- |
| “Downstream always inherits Restricted.” | Owner reassesses with Phase 5. |
| “We implemented automated lineage.” | Conceptual / business lineage; no scanner. |
| “This is the NPHIES map.” | Illustrative generic interchange `[A]`; national specs `[NDMO verification required]`. |
| “We are NDMO-compliant on lineage.” | No specification evidenced. |
| “DMC signs every flow.” | Existing exception/policy rights only. |
