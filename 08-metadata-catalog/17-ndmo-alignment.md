# NDMO Alignment — Metadata and Catalog

**Document ID:** RHC-DG-P8-017  
**Phase:** 8 — Metadata and catalog  
**Status:** Implemented (alignment notes only)  
**Does not claim:** Implementation, evidence, scores, specification completion, or catalog automation

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

Phase 8 alignment is **domain-name and narrative-concept only** where that is defensible against NDMO Standards v1.5 as used in this repository.

**Not used in this file:** invented specification-level Data Catalog and Metadata control IDs (do not invent numbers under `MCM`).

**No NDMO compliance is claimed.**

---

## 2. Three-way distinction (mandatory)

| Bucket | What it includes in Phase 8 |
| --- | --- |
| **Verified NDMO-supported information** `[C]` | Data Catalog and Metadata is a knowledge-domain **name**; domain ID `MCM` as recorded in Phase 2 from the retrieved Standards text; Section 8.1 **counts** 6 controls / 20 specifications (counts only); NDMO cites an automated catalog as a **national concept** in domain narrative used in Phase 0; Trusted Data principle **name** includes catalog/metadata among mapped families; DAMA DMBOK is a key reference **name** |
| **Unverified NDMO information** `[NDMO verification required]` | Official mandatory **metadata fields**; official metadata **categories**; control- and specification-level **catalog** requirements; whether an entity seven-category model is acceptable; whether certification states are national; Organizational Manual catalog duties; whether Year-1 asset types match national taxonomy |
| **Rafid’s proposed design** `[A][B]` | Lifecycle; seven categories with mandatory vs capability-dependent split; asset hierarchy and Year-1 types; minimum field occupancy including System / Primary System rule; glossary; conceptual catalog; five internal trust statuses; MVP cut |

**Do not mix the three buckets.**  
**Do not invent NDMO control IDs.**  
**Do not claim compliance.**

---

## 3. Statements that remain explicitly unverified

The following require verification against official NDMO text before anyone briefs them as national requirements:

- Specific NDMO **metadata fields**
- Specific NDMO metadata **categories**
- Control-level **catalog** requirements

Until verified, Rafid uses the `[A][B]` design and labels it as such.

`MCM` as a **domain ID** may be used as `[C]` because it was copied in Phase 2 from the retrieved text. That is **not** a licence to invent specification IDs under that domain.

---

## 4. What Phase 8 is not

- Not a completed NDMO Data Catalog and Metadata domain implementation
- Not an automated catalog in production
- Not Phase 9 lineage alignment
- Not an annual specification-level assessment pack (Phase 14)

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5 — Catalog and Metadata domain **name**; `MCM`; Section 8.1 counts; automated catalog **concept** as already used in this repo; Trusted Data mapping **name** | Verified column |
| `[NDMO verification required]` | Fields, categories, specification IDs, certification mandates | Unverified column |
| `[A][B]` | Approved Phase 8 framework | Rafid column |
