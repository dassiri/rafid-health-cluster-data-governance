# NDMO Classification Baseline

**Document ID:** RHC-DG-P5-001  
**Phase:** 5 — Data classification  
**Status:** Implemented (baseline only — conflict **not** resolved)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This file records what this programme treats as **verified at domain/narrative level** versus what remains **unverified** for official NDMO classification **tier names and definitions**.

It does **not**:

- Choose an official NDMO four-tier name-set
- Equate Rafid’s scheme with NDMO’s scheme
- Introduce specification-level control IDs
- Claim compliance

---

## 2. Verified NDMO information used in this phase `[C]`

Drawn from NDMO *Data Management and Personal Data Protection Standards*, Version 1.5, January 2021, at **domain / narrative** level only:

| Statement | Use in Phase 5 |
| --- | --- |
| Data Classification is one of the 15 knowledge domains | Alignment target name; not implemented here |
| Classification categorizes data so it may be used and protected efficiently | Why a framework exists |
| Classification levels are assigned following an impact assessment of potential damage from mishandling or unauthorized access | Rafid uses a **qualitative** impact rule; it does **not** copy an unverified official scoring method |
| NDMO materials refer to **four** classification levels as a national concept | Confirms a four-level *idea*; **does not** confirm the four **names** |
| Open by Default does not mean health records are published; non-disclosure can be justified | Consistent with Phase 1 application note |
| Data Security and Protection is under the National Cybersecurity Authority (NCA) | Security **consequences** stay high-level; no NCA control catalogue is designed here |
| Personal Data Protection is a distinct knowledge domain | PDPO reviews privacy implications of classification where personal data is involved |

---

## 3. Unresolved NDMO tier-name conflict `[NDMO verification required]`

**This conflict is not resolved in Phase 5.** Do not pick a winner in interviews or in later files.

Two candidate official name-sets appear in secondary discussion of NDMO classification. **Exact official tier names and their official definitions are `[NDMO verification required]`.**

**Candidate set A** `[NDMO verification required]`

- Top Secret  
- Secret  
- Restricted  
- Public  

**Candidate set B** `[NDMO verification required]`

- Top Secret  
- Secret  
- Confidential  
- Public  

**Neither set is adopted as Rafid’s enterprise scheme.**  
**Neither set is declared “the” NDMO scheme in this repository.**  
**Definitions of Top Secret, Secret, Restricted (as an NDMO name), Confidential (as an NDMO name), and Public (as an NDMO name) are `[NDMO verification required]`.**

Until the official Standards/regulation text is re-verified for **names**, this programme will not:

- Map Rafid Internal, Confidential, or Restricted **onto** an NDMO name one-for-one
- Treat Rafid “Restricted” as NDMO “Restricted” or as NDMO “Confidential”
- Invent a fifth or sixth NDMO name

Rafid’s four working labels (Public, Internal, Confidential, Restricted) are an **entity proposal** `[A][B]`. See [`02-classification-model.md`](02-classification-model.md).

---

## 4. What else remains `[NDMO verification required]`

- NDMO Data Classification **Regulation** text (named by the Standards; not retrieved as the working source for this phase)
- Official impact categories, impact-level labels, and any lawful exception that reclassifies low-impact data as Public
- Whether an entity may use local labels (such as **Internal**) alongside national labels
- Handling-control tables that NCA or NDMO may require per national tier
- Any specification-level classification control or specification identifier

---

## 5. How Phase 5 proceeds despite the conflict

Rafid documents a **proposed internal scheme** so the cluster can classify **datasets** consistently `[A][B]`. National alignment is deferred to a later verification pack (folder `14-ndmo-alignment/`, not built here) **after** official names are confirmed.

Until then, interview language is:

> “NDMO has a Data Classification domain and a four-level *concept* `[C]`. I have **not** locked official NDMO tier names because Restricted versus Confidential as the third national label is `[NDMO verification required]`. Rafid’s Public / Internal / Confidential / Restricted labels are the cluster’s proposed scheme `[A][B]`, not NDMO’s scheme.”

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5 — Domain 13 **name** and domain narrative; four-levels **concept**; NCA mandate for security domain; Open by Default / Personal Data Protection **names** | Section 2 |
| `[NDMO verification required]` | Official tier **names**, **definitions**, regulation text, specification IDs | Sections 3–4 |
| `[A][B]` | Rafid proposed scheme (other Phase 5 files) | Not mixed into NDMO names |
