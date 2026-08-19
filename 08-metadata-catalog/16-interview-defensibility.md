# Interview Defensibility — Metadata and Catalog

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P8-016  
**Phase:** 8 — Metadata and catalog  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## What is metadata?

Metadata is **data about data**: the governed description that says what an asset is, who owns it, how it is classified, and in which system context it lives `[B]`. It is not the patient row, the claim file, or the incident narrative.

Rafid groups metadata into seven categories `[A][B]` (four mandatory, three capability-dependent). Those names are **not** briefed as NDMO-required `[NDMO verification required]`.

---

## Why do we need a data catalog?

So people can **discover governed assets** without relying on shadow spreadsheets `[B]`. The catalog shows name, Owner, classification, definition, and trust status. It does **not** dump Restricted data. NDMO names Data Catalog and Metadata as a domain and an automated catalog as a national **concept** `[C]`; Rafid has a **design**, not a tool, and not a compliance score.

---

## Difference between catalog and glossary?

| Artifact | Holds |
| --- | --- |
| **Glossary** | Business **terms** (Patient, Encounter, …) |
| **Catalog** | Data **assets** (datasets, master entities, …) |

They link: Glossary ↔ Catalog ↔ Assets. Neither is the data store.

---

## Difference between metadata and data quality?

**Data quality:** is the **data** correct? (Phase 7)  
**Metadata quality:** is the **description** correct, complete, current, and governed? (this phase)

Do not build a second quality framework. Reuse dimension **names** only as metadata checks.

---

## Who owns metadata?

**Data Owner = Accountable** for business metadata and definitions (Phase 4 rows 1 and 8). **Business Data Steward = Responsible** for maintenance. **Custodian** supplies technical metadata where applicable. **DMO** owns methodology, catalog oversight, and the registration check — not clinical meaning. **DMC** uses **existing** Phase 3 decision rights only (no new catalog-appeal class). **PDPO** is Consulted on personal/health definitions; PDPO is **A** only on the sharing privacy row.

---

## What makes an asset trustworthy?

Internal catalog statuses: Registered → Reviewed → Certified → Deprecated → Retired `[A][B]`. **Certified** means the **Data Owner** accepts the **description**. It is **not** NDMO certification, not a regulator seal, and not access approval.

---

## How does classification appear in a catalog?

As **Security / Classification metadata**: the Rafid tier (Public / Internal / Confidential / Restricted `[A][B]`). Unlabeled is not Public. The catalog may show the **label**; it must not show Confidential/Restricted **contents**. Access stays Phase 4/5.

---

## How does lineage connect to metadata?

Coarse **Source → Transformation → Target → Consumer** may be stored as lineage metadata. **Phase 9** is Designed / Documented as the lineage framework (documentation/design only; operational implementation and measured performance are not claimed). Do not pretend the catalog is a lineage platform.

---

## How would you start a catalog program?

The approved **MVP**: three domains (Patient/Person, Clinical/Medical Records, Financial/Billing & Claims); asset types Dataset and Master Data Entity; users = Owners, Business Data Stewards, DMO; **mandatory fields only as the publish bar**; full registration workflow; **qualitative** success. Do not start with eight domains and a vendor bake-off.

---

## Why not implement a tool immediately?

A tool without Owner-accepted definitions, classification links, and a registration path becomes another shadow IT list `[B]`. This phase is **governance design**. Purview, Collibra, Atlan, and Informatica are **out of scope**. NDMO’s automated-catalog **concept** `[C]` is not satisfied by naming a product, and is not claimed as implemented.

---

## Must-nots

| Do not say | Say instead |
| --- | --- |
| “We implemented Collibra/Purview.” | Conceptual catalog; no platform. |
| “Certified means NDMO certified.” | Internal Rafid trust only `[A][B]`. |
| “The catalog contains the Restricted dataset.” | It contains **metadata** about it. |
| “DMC approves every asset.” | Owner **A** for content; DMC keeps existing exception/policy rights. |
| “Steward is Head of HIM.” | In Phase 8 domain examples, Steward = **Business Data Steward** only. |
| “We are MCM-compliant.” | Domain **name** `[C]`; specifications `[NDMO verification required]`; no compliance claim. |
