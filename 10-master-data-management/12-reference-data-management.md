# Reference Data Management

**Document ID:** RHC-DG-P10-012  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for each governed code set in that domain; DMO (method) `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — MDM ≠ RDM; no separate Reference Data phase.

**Phase:** 10 — Master data management  
**Does not decide:** A Phase “10b” reference-data programme; moving item master to Core MDM

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the relationship between **MDM** and **Reference Data Management**.

**MDM ≠ Reference Data Management.**  
**Both require governance.**  
**Do not create a separate Reference Data phase.**

NDMO names “Reference and Master Data Management” as one knowledge-domain **name** `[C]`. That **name** does not force Rafid to treat every code list as Core MDM `[NDMO verification required]`.

---

## 2. Reference data (examples) `[A]`

Controlled code sets such as:

- Country  
- Gender  
- Encounter type  
- Claim status  
- Diagnosis codes  

These **classify or constrain** transactions and masters. They are not Patient or Provider **identities**.

---

## 3. Supply Chain / Item-type at this maturity

**Supply Chain / Item-type data remains Reference Data at this maturity** unless a future **approved** decision changes it.

It is **not** Core MDM. Item codes still have a Phase 4 Owner (Supply Chain Director) and Phase 7 CDE-010/CDE-011 quality concerns — as **reference/item** governance, not a fourth golden-record program.

---

## 4. How both are governed (existing paths)

| Object | Path |
| --- | --- |
| Master entity definition | Data Owner **A** (this phase + STD-005) |
| Code-list meaning | Data Owner **A** of the owning domain (Phase 4) |
| Registration in catalog | Phase 8 / Metadata Registration Procedure |
| Quality defects | Phase 6/7 issue path |
| Policy exceptions | Phase 6 exception procedure (**DMC = A**) |

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Example code sets; item-type cut | Sections 2–3 |
| `[B]` | MDM ≠ RDM; both governed | Section 1 |
| `[C]` | Reference and Master Data Management domain **name** | Context |
| `[NDMO verification required]` | Official NDMO RDM specifications | Not claimed |
