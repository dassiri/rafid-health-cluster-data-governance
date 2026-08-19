# Policy Hierarchy

**Document ID:** RHC-DG-P2-003  
**Phase:** 2 — Governance Design Boundaries  
**Status:** Documented  
**Does not decide:** Any Rafid policy text, standard, or SOP

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document defines **how normative documents stack**. It is required before Phase 6 so procedures cannot outrank law, and so cluster standards cannot be mistaken for NDMO specifications.

NDMO control `DG.2` requires a policy and guidelines **gap analysis** and then entity-specific Data Management and Personal Data Protection Policy and Guidelines aligned to national policies and standards `[C]` (NDMO Standards v1.5, `DG.2.1`, `DG.2.2`). **Neither deliverable is produced here.** This file only states the hierarchy those later documents must respect `[B]`.

---

## 2. Hierarchy `[B]` with national layer `[C]`

Higher layers prevail when documents conflict. Layer codes are Rafid documentation labels `[B]`, **not** NDMO IDs.

| Layer | Name | What belongs here | Status in this repo |
| --- | --- | --- | --- |
| **L0** | Kingdom law and Royal instruments | Statutes and implementing regulations (for example PDPL, other applicable laws) | Watchlist only `[NDMO verification required]` for the full applicable set |
| **L1** | National data and cyber regulators | NDMO Standards and NDMO-issued policies/regulations; NCA frameworks for security | Standards v1.5 used as `[C]` source; other NDMO regulations and NCA catalogs not retrieved `[NDMO verification required]` |
| **L2** | Sector / supervisory rules | MOH, accreditation, health-insurance, or medicines rules that apply to a real cluster | Not designed; `[NDMO verification required]` |
| **L3** | Entity policy | Rafid Data Management and Personal Data Protection Policy (and related entity policies) | **Not written** — `DG.2.2` later `[C]` |
| **L4** | Entity standards | Binding cluster rules that make L3 testable (classification handling, quality dimensions, metadata minimums) | **Not written** |
| **L5** | Procedures and work instructions | How a role performs a standard | **Not written** |

```text
L0  Law
L1  NDMO / NCA (national)
L2  Health-sector rules (if applicable)
L3  Rafid policy
L4  Rafid standards
L5  Rafid procedures
```

---

## 3. Rules of the stack `[B]` / `[A]`

1. **No L5 procedure may contradict L0–L4.** If practice must differ, the change is an exception against policy (exception process is later), not a silent SOP.
2. **Do not copy NDMO specification IDs into Rafid SOPs as if Rafid invented them.** Cite the official ID when pointing at NDMO `[C]`.
3. **Do not invent NDMO IDs** to fill gaps. Gaps are labeled `[NDMO verification required]` or handled as `[B]` cluster practice explicitly marked as non-NDMO.
4. **Entity policy (L3) must be aligned to national policies and standards** when `DG.2` is executed `[C]`. Alignment is not claimed now.
5. **Domain 15 security control detail** follows NCA, not a parallel Rafid security standard that pretends to replace NCA `[C]`.
6. **Healthcare candidate principles** in the principles document are not L3 policy until (if ever) issued `[A]`.

---

## 4. Document types that will appear later `[B]`

| Type | Layer | Example (illustrative name only) |
| --- | --- | --- |
| Policy | L3 | Rafid Data Governance Policy |
| Standard | L4 | Rafid Metadata Minimum Standard |
| Procedure | L5 | How to request a data extract |
| Register | Artifact (NDMO `DG.8` later) | Decision log, issue log `[C]` pointer — not created here |
| Plan | Strategy/plan (`DG.1.3`) | Three-year data management plan `[C]` pointer — not created here |

Illustrative names are **placeholders**, not issued titles.

---

## 5. Gap-analysis placeholder (not executed)

When Phase 6 runs `DG.2.1`, NDMO says the gap analysis includes, at minimum `[C]`:

1. Analysis of the national program’s policies, standards, and guidelines.
2. Identification and analysis of data-related standards and policies published by the entity or the regulator of the entity’s sector.
3. Analysis of internal entity-specific requirements.
4. A development plan with implementation timeline.

Rafid has **not** performed this analysis. Sector regulator documents are `[NDMO verification required]`. Internal “policies” today are assumed to be fragmented SOPs `[A]` (organization profile).

---

## 6. Intentionally unresolved

- Actual L0 inventory (PDPL articles, health law, etc.).
- Actual L1 inventory beyond Standards v1.5 (classification regulation, sharing regulation, FOI regulation, Organizational Manual).
- Whether L2 is empty, thin, or dense for an MOH cluster.
- Policy owners and approval path (needs Phase 3).
- Bilingual (Arabic/English) controlled-document rules.

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5, `DG.2.1`, `DG.2.2`, `DG.1.3`, `DG.8`, Domain 15 NCA note | Why entity policy must align nationally; later artifact types |
| `[B]` | Policy–standard–procedure hierarchy | Layer model |
| `[A]` | Rafid as-is (fragmented SOPs) | Gap-analysis starting premise |
