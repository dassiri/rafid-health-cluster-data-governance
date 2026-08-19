# Master Data vs Reference Data vs Transaction Data

**Document ID:** RHC-DG-P10-002  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (definitions method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Three-way distinction; candidate criteria not NDMO controls.

**Phase:** 10 — Master data management  
**Does not decide:** Recategorizing encounters or claims as master entities

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the **three-way distinction** used in Rafid MDM `[A][B]`.

Do **not** classify every frequently reused dataset as Master Data.

These definitions are industry-practice guidance `[B]` applied as Rafid design `[A]`. They are **not** NDMO control requirements `[NDMO verification required]`.

---

## 2. Three classes (locked)

| Class | Meaning `[B]` | Healthcare examples `[A]` |
| --- | --- | --- |
| **Master Data** | Relatively persistent **business identities** shared across processes; duplication causes cross-process harm | Patient / Person; Provider / Clinician; Facility; Organization / Department |
| **Reference Data** | **Controlled value lists** used to classify or constrain other data | Country codes; Gender codes; Encounter types; Diagnosis code sets; Claim status codes |
| **Transaction Data** | **Events or transactions** that happen in time; they *use* masters and reference codes | Encounter; Claim; Payment; Appointment |

Encounter is **transaction** data (Clinical domain, CMO). It is **not** Core MDM even though it is reused constantly.

Claim is **transaction** data (Financial domain, CFO). It is **not** Core MDM at this maturity.

---

## 3. Master-data candidate criteria `[B]` / `[A]`

A candidate is considered when **several** of the following hold (qualitative — **no score**):

- Shared across multiple business processes  
- Relatively persistent entity  
- Used as a common business identity  
- Requires consistency across systems  
- Has clear business ownership  
- Creates downstream impact when duplicated or inconsistent  

Meeting one criterion does **not** automatically make the object Core MDM (same two-step spirit as CDE/lineage: candidacy then confirmation of MDM treatment). Confirmation for Year-1 Core MDM is recorded in [`03-master-domain-assessment.md`](03-master-domain-assessment.md).

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Healthcare examples | Section 2 |
| `[B]` | Three-way distinction; candidate criteria | Sections 2–3 |
| `[C]` | Reference and Master Data Management domain **name** | Context |
| `[NDMO verification required]` | Official NDMO master/reference definitions as control text | Not claimed |
