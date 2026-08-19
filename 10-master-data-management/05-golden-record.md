# Golden Record / Trusted Master Representation

**Document ID:** RHC-DG-P10-005  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for accepting the trusted representation of that master  
**Approver:** CDO `[B]` (concept as framework)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Logical/governed golden record; no physical hub required.

**Phase:** 10 — Master data management  
**Does not decide:** Physical MDM database or vendor hub

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records what Rafid means by a **golden record**: a **trusted master representation** that is **logical and governed** `[B]`.

STD-005 already stated golden record means **governed authority**, not a physical hub. This file does not change that.

---

## 2. Critical rule (locked)

The golden record **does not require**:

- One physical database  
- One physical MDM platform  
- One universal source system  

Existing EMR, credentialing, and org-reference systems may continue to **store** copies. Governance decides **which representation is trusted for which use**, not that IT must build a new store.

---

## 3. Logical chain (locked)

```text
Source records
→ Matching / reconciliation
→ Survivorship
→ Trusted master representation
→ Downstream consumption
```

| Step | Governance meaning |
| --- | --- |
| **Source records** | System-local person/provider/facility rows |
| **Matching / reconciliation** | Conceptual match + manual review ([`06-matching-duplicate-management.md`](06-matching-duplicate-management.md)) |
| **Survivorship** | Per-domain, per-attribute Owner rules ([`07-survivorship.md`](07-survivorship.md)) |
| **Trusted master representation** | The Owner-accepted identity (logical) |
| **Downstream consumption** | Encounter, claim, catalog, reports **use** that identity — via lineage (Phase 9), not a new bus architecture |

The trusted representation can be **logically governed across existing systems** (for example: registration is authoritative for National ID capture; credentialing for licence expiry) without collapsing into one table.

Facility / Organization in MVP does **not** get a separate golden-record **program** ([`16-mdm-mvp.md`](16-mdm-mvp.md)).

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Logical golden-record concept | Sections 2–3 |
| `[C]` | MDM domain **name** | Context |
| `[NDMO verification required]` | Official NDMO golden-record mandates | Not claimed |
