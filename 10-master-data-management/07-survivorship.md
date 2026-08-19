# Survivorship

**Document ID:** RHC-DG-P10-007  
**Version:** 1.0  
**Status:** Implemented (conceptual only)  
**Owner:** Data Owner **A** and Steward **R** for domain/attribute rules  
**Approver:** CDO `[B]` (principles as framework)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Per-domain/per-attribute survivorship; no universal order.

**Phase:** 10 — Master data management  
**Does not decide:** A coded survivorship engine

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **conceptual survivorship principles** `[A][B]`.

**Do not create an arbitrary universal priority order.**

Locked rule:

> Survivorship rules are established per master domain and attribute by the Data Owner and Steward.

---

## 2. Considerations (not a ranked enterprise list)

When Owner and Steward **set a rule for one attribute**, they may consider:

- Source authority  
- Attribute-level trust  
- Recency  
- Completeness  
- Verification status  
- Business ownership  

These are **inputs to a local rule**, not a cluster-wide stack-rank of systems.

---

## 3. Illustrative examples `[A]`

All examples are `[A]` illustrative. They are **not** production rules and **not** a universal order.

| Master / attribute `[A]` | Illustrative Owner-set idea |
| --- | --- |
| Patient / National ID | Prefer the value captured at registration when verified; do not silently overwrite from a billing extract |
| Patient / contact phone | Prefer more recently verified contact **if** the Owner so decides — recency is not automatically global |
| Provider / licence expiry | Prefer credentialing system attribute authority over EMR display copy |
| Facility / facility code | Prefer Domain 8 org-reference list (integrity) — **MVP supporting alignment**, not a Facility survivorship **program** |

If two sources conflict, Steward documents the clash; Owner **A** decides; Custodian implements in **existing** systems.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative attribute examples | Section 3 |
| `[B]` | Per-domain/per-attribute rule | Sections 1–2 |
| `[C]` | MDM domain **name** | Context |
| `[NDMO verification required]` | Official NDMO survivorship mandates | Not claimed |
