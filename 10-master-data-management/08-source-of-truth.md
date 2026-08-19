# Source of Truth

**Document ID:** RHC-DG-P10-008  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for which system is authoritative **for an attribute** in that domain  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — SoR vs SoRef vs Master Representation; no universal SoT.

**Phase:** 10 — Master data management  
**Does not decide:** A single cluster-wide source system

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document distinguishes **three** related ideas `[B]`.

**Do not create a universal source-of-truth rule.**

A system may be authoritative for a **specific attribute** without being the universal source for the **entire entity**.

---

## 2. Three terms (locked)

| Term | Meaning |
| --- | --- |
| **System of Record** | The operational system where the **business process** creates or first maintains that fact |
| **System of Reference** | A system others **look up** for a copy or list (may not be where the fact is created) |
| **Master Representation** | The **governed trusted identity** (logical golden record) after match/survivorship |

Copies in warehouses or billing are not automatically Systems of Record.

---

## 3. Illustrative healthcare examples `[A]`

| Entity / attribute `[A]` | Illustrative authority idea (not a universal rule) |
| --- | --- |
| Patient / National ID | Registration/EMR class as System of Record for capture; MPI class may be System of Reference for lookup |
| Provider / licence expiry | Credentialing class as System of Record for the attribute; EMR provider file may display a copy |
| Facility / department code | Org-reference lists as System of Record for the **code**; EMR may be System of Reference for users |
| Claim / claim identifier | Billing class is System of Record for the **transaction** — claims are **not** Core MDM |

These examples do not appoint a vendor and do not override Phase 4 Owners.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative attribute authorities | Section 3 |
| `[B]` | Three-term distinction | Sections 1–2 |
| `[C]` | MDM domain **name** | Context |
| `[NDMO verification required]` | Official NDMO SoT mandates | Not claimed |
