# Lifecycle vs Records Management vs Backup

**Document ID:** RHC-DG-P11-003  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Three-way distinction; Records Management not built.

**Phase:** 11 — Data lifecycle  
**Does not decide:** A Records Management programme or backup architecture

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **distinguishes** three concepts that are often collapsed in operations `[B]`.

**Do not create a separate Records Management framework** in this phase.

---

## 2. Three concepts (locked)

| Concept | Meaning |
| --- | --- |
| **Data Lifecycle Management** | Governs **data** from creation / acquisition to disposition (this phase) |
| **Records Management** | Governs **records** that must be retained as **evidence** or **business records** |
| **Backup / Disaster Recovery** | Supports **recovery and continuity** and is **NOT** the same as retention or archival |

A backup copy can exist **after** the business retention rule would have allowed disposal of the **active** instance. Backup expiry is a **continuity** design (out of this phase), not a substitute Retention Schedule.

**Archive ≠ Backup.** Archived data remains in the **lifecycle**. Backup is a **recovery** copy.

NDMO Document and Content Management is a knowledge-domain **name** `[C]`. That name does not implement Records Management here `[NDMO verification required]`.

---

## 3. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Three-way split | Section 2 |
| `[C]` | Document and Content Management domain **name** | Context |
| `[NDMO verification required]` | Official NDMO records/lifecycle overlap | Not claimed |
