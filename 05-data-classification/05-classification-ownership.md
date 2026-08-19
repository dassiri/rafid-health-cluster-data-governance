# Classification Ownership

**Document ID:** RHC-DG-P5-005  
**Phase:** 5 — Data classification  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document assigns classification **decision rights** for the fictional cluster `[A]`. It matches Phase 4: Data Owner is **Accountable** for dataset classification application; IT does **not** decide `[B]`.

NDMO names: Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office, PDPO, Compliance Officer `[C]`. Specification-level duties `[NDMO verification required]`.

---

## 2. Responsibilities

### Data Owner

- **Accountable** for the business classification decision
- **Approves initial classification**
- **Approves reclassification**
- Only the Data Owner approves a classification **change** (see [`07-change-management.md`](07-change-management.md))

### Business Data Steward

- **Proposes** classification (impact narrative, no numeric score)
- **Applies and maintains** the approved Rafid tier on the dataset
- **Maintains registry information** for the domain’s datasets
- **Flags** potential misclassification to the Owner

### IT Data Steward / Custodian

- **Implements technical controls** that correspond to the approved tier (high-level; no tool or algorithm specification here)
- **Does NOT decide** classification
- May refuse implementation that cybersecurity flags as unsafe; that is a **security** escalation (CISO path + CDO), not a right to pick a tier

### DMO

- **Owns the methodology** (this framework)
- **Maintains the Classification Registry** (proposed artifact)
- **Provides consistency oversight** (similar datasets should not silently diverge without rationale)

DMO is **not** the business Data Owner and does **not** approve classification in place of the Owner.

### PDPO

- **Reviews privacy implications for personal data**
- Does **not** replace Owner **A** on the classification decision
- Remains **A** on Phase 4 “Data sharing — privacy compliance review (personal data)” — a **sharing** decision, not a substitute classification stamp

### Compliance Officer

- **Performs independent oversight / audit** of whether the process and registry are followed
- Does **not** set the business tier

---

## 3. RACI snapshot `[B]`

| Activity | Owner | Steward | Custodian | DMO | PDPO | CO |
| --- | --- | --- | --- | --- | --- | --- |
| Propose dataset classification | C | **R** | I | C | C* | I |
| Approve initial classification | **A** | R | I | C | C* | I |
| Approve reclassification | **A** | R | I | C | C* | I |
| Record in Classification Registry | C | **R** | I | **A**† | I | I |
| Implement technical handling | C | C | **R** | C | I | I |
| Process/methodology | C | C | I | **A** | C | C |
| Independent process audit | I | I | I | C | C | **A** |

\* PDPO **C** when the dataset involves personal data.  
† DMO is **A** for **registry completeness and methodology**, not for the **tier value**. The **tier value** **A** remains the Data Owner.

Each row has one **A**.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 5 responsibilities; Phase 4 classification **A** = Owner | Sections 2–3 |
| `[A]` | Rafid titles from Phase 4 | Who occupies Owner/Steward seats |
| `[C]` | NDMO role **names** | Mapping |
| `[NDMO verification required]` | Specification-level classification duties | Not cited as IDs |
