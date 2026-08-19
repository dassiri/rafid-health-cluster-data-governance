# Classification Registry (Proposed)

**Document ID:** RHC-DG-P5-008  
**Phase:** 5 — Data classification  
**Status:** Implemented (schema only)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Labeling

This is a **proposed Rafid governance artifact** `[A][B]`.

**It is not an NDMO-mandated registry.**  
**It must not be given an NDMO control ID.**  
**It is not evidence of NDMO implementation.**

NDMO’s Data Classification domain exists as a knowledge-domain **name** `[C]`. Whether NDMO requires a register with these fields is `[NDMO verification required]`.

DMO maintains the registry (methodology and completeness). Data Owners remain **A** for the **tier** recorded.

---

## 2. Proposed schema `[A][B]`

| Field | Purpose |
| --- | --- |
| Dataset ID | Stable Rafid identifier (assigned by DMO; not an NDMO ID) |
| Dataset name | Human-readable name |
| Domain | One of the eight Phase 4 domains |
| Data Owner | Phase 4 Owner title |
| Steward | Phase 4 Business Data Steward title |
| Classification | One of: Public, Internal, Confidential, Restricted (Rafid labels `[A][B]`) |
| Classification rationale | Qualitative highest-impact narrative; **no numeric score** |
| Approval date | Date the Owner approved the current tier |
| Review date | Date of last periodic reconsideration (not an SLA clock) |
| Review status | For example: current / due for review / change in progress — working values `[B]`, not NDMO codes |
| Exceptions | Documented exceptions (for example Public subset; de-identified extract) |
| Related systems | Systems or stores that hold the dataset (Custodian context) |

Optional operating notes (still not NDMO fields): personal-data flag (yes/no) to trigger PDPO consult; link to Ownership Change Record if Owner title changed.

---

## 3. What is not stored here

- Encryption algorithms or tool names
- NCA control catalogues
- NDMO national tier names presented as the Rafid Classification field
- Named patient or employee records (the registry is metadata about datasets)

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 5 registry field list | Section 2 |
| `[C]` | Data Classification domain **name** | Why a register is plausible, not mandated here |
| `[NDMO verification required]` | Whether NDMO mandates this schema | Section 1 |
