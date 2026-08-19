# NDMO Alignment — Classification

**Document ID:** RHC-DG-P5-012  
**Phase:** 5 — Data classification  
**Status:** Implemented (alignment notes only)  
**Does not claim:** Implementation, evidence, or national-tier equivalence

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Three-way distinction (mandatory)

| Bucket | What it includes in Phase 5 |
| --- | --- |
| **Verified NDMO information** `[C]` | Data Classification is a knowledge domain; classification supports use and protection; impact assessment is part of the **concept**; four **levels** exist as a national **concept**; Personal Data Protection is a separate domain; Data Security and Protection is under NCA; Open by Default is a national guiding principle **name** |
| **Unverified NDMO information** `[NDMO verification required]` | Exact official **tier names**; official **definitions** of those names; which of the two candidate name-sets is correct; classification regulation text; specification-level IDs; whether Internal exists nationally; handling tables per national tier; whether an entity scheme may differ in labels |
| **Rafid’s proposed design** `[A][B]` | Tiers Public, Internal, Confidential, Restricted; dataset-level rule; highest applicable impact (qualitative); typical domain guidance; Owner approval; proposed registry; access/sharing consequences table |

**Do not mix the three buckets.**  
**Do not resolve the NDMO classification-tier conflict.**  
**Do not present Rafid’s scheme as equivalent to NDMO’s national scheme.**  
**Do not introduce NDMO control IDs.**

---

## 2. Unresolved name conflict (repeated on purpose)

Candidate set A `[NDMO verification required]`: Top Secret, Secret, Restricted, Public  

Candidate set B `[NDMO verification required]`: Top Secret, Secret, Confidential, Public  

No selection is made in this phase.

---

## 3. What Phase 5 is not

- Not a completed NDMO Data Classification domain implementation
- Not a crosswalk of Rafid Restricted → any NDMO name
- Not NCA control design
- Not Phase 6 policy

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5 — domain/narrative statements listed in [`01-ndmo-baseline.md`](01-ndmo-baseline.md) | Verified column |
| `[NDMO verification required]` | Official names, definitions, regulation, specification IDs | Unverified column |
| `[A][B]` | Approved Rafid classification framework | Rafid column |
