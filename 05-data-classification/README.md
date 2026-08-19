# Phase 5 — Data Classification Framework

**Document ID:** RHC-DG-P5-000  
**Phase:** 5 — Data classification  
**Status:** Implemented  
**Does not decide:** L3–L5 policy text (Phase 6), NCA technical control design, or live dataset inventory

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Purpose

Phase 5 defines the **data classification framework** for the fictional Rafid Health Cluster `[A]`: a proposed four-tier enterprise scheme, dataset-level application, ownership of classification decisions, process, change handling, a proposed registry, and access/sharing consequences.

This is a governance framework artifact, not a software application and not a cybersecurity architecture. It does **not** claim NDMO compliance. Rafid’s four tiers are **not** NDMO’s official classification scheme.

---

## Scope

**In scope**

- NDMO baseline **as unresolved** (tier-name conflict preserved)
- Rafid proposed tiers: Public, Internal, Confidential, Restricted `[A][B]`
- Qualitative “highest applicable impact” rule (no numeric scoring)
- Domain-level **typical** guidance for the eight Phase 4 domains (not blanket rules)
- Classification responsibilities and process
- Proposed Classification Registry schema `[A][B]`
- Access/sharing consequences at a high level
- Illustrative fictional examples `[A]`

**Out of scope**

- Phase 6 policy / standard / procedure text
- Classifying a live inventory of Rafid datasets
- Encryption algorithms, security products, or NCA control catalogues
- Invented NDMO control IDs
- Resolving official NDMO tier names
- Numeric SLAs

---

## Classification model

Rafid’s proposed enterprise scheme `[A][B]`:

1. Public  
2. Internal  
3. Confidential  
4. Restricted  

These names are **Rafid working labels**. They must not be briefed as NDMO’s national tiers. See [`01-ndmo-baseline.md`](01-ndmo-baseline.md) and [`02-classification-model.md`](02-classification-model.md).

---

## Dataset-level classification principle

Classification is applied at the **dataset** level, not automatically at the domain level `[B]`.

A domain may contain datasets at more than one Rafid tier. Domain rows in this phase are **typical patterns** only.

The decision rule is qualitative **highest applicable impact** (privacy, patient safety, financial, legal/regulatory, security, reputational, operational; plus unauthorized disclosure, modification, and access). **No numeric scoring.**

---

## Ownership responsibilities

Aligned with Phase 4 (Owner **A** for dataset classification application):

| Role | Classification role |
| --- | --- |
| Data Owner | **Accountable**; approves initial classification and reclassification |
| Business Data Steward | Proposes, applies, maintains registry information, flags misclassification |
| IT Data Steward / Custodian | Implements technical controls; **does not decide** classification |
| DMO | Owns methodology; maintains Classification Registry; consistency oversight |
| PDPO | Reviews privacy implications for personal data |
| Compliance Officer | Independent oversight / audit |

---

## Relationship to Phase 4

Phase 4 named the eight domains and one Data Owner per domain. Phase 5 uses those Owners as classification **approvers**. It does not change Owner titles, stewardship, or the two sharing RACI rows.

Sharing still splits **business approval** (Owner **A**) from **privacy compliance review** (PDPO **A**) where personal data is involved.

---

## Relationship to Phase 6

Phase 6 holds L3–L5 policy and procedure text that may bind this framework. This phase does **not** write those documents. Phase 6 is Designed / Documented; operational implementation and measured performance are not claimed.

---

## NDMO verification limitations

- Data Classification exists as an NDMO knowledge domain `[C]`.
- Official NDMO **tier names and definitions** remain `[NDMO verification required]`. Two candidate name-sets are recorded and **not** selected.
- Rafid’s scheme is an entity proposal `[A][B]`, not a mapping declared equal to NDMO.
- No specification-level control IDs are used in this folder.
- No compliance claim is made.

---

## Files included

| File | Content |
| --- | --- |
| [01-ndmo-baseline.md](01-ndmo-baseline.md) | Verified vs unresolved NDMO classification information |
| [02-classification-model.md](02-classification-model.md) | Four Rafid tiers `[A][B]` |
| [03-classification-criteria.md](03-classification-criteria.md) | Dataset-level, highest-impact, qualitative |
| [04-domain-application.md](04-domain-application.md) | Typical patterns and exceptions for eight domains |
| [05-classification-ownership.md](05-classification-ownership.md) | Who decides vs who implements |
| [06-classification-process.md](06-classification-process.md) | End-to-end and data-state handling |
| [07-change-management.md](07-change-management.md) | Reclassification triggers; Owner approval only |
| [08-classification-registry.md](08-classification-registry.md) | Proposed Rafid registry schema |
| [09-access-sharing-consequences.md](09-access-sharing-consequences.md) | Access/sharing table |
| [10-illustrative-examples.md](10-illustrative-examples.md) | Fictional dataset examples `[A]` |
| [11-interview-defensibility.md](11-interview-defensibility.md) | **INTERNAL / INTERVIEW PREPARATION** |
| [12-ndmo-alignment.md](12-ndmo-alignment.md) | Verified / unverified / Rafid design |

---

## Status

**Implemented** — documentation only. No live datasets are classified. Phase 6 is Designed / Documented; operational implementation and measured performance are not claimed.
