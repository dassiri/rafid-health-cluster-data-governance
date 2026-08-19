# MDM Lifecycle Boundary

**Document ID:** RHC-DG-P11-014  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 10 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 10 entity lifecycle kept distinct; Phase 10 not redesigned.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Matching, survivorship, or golden-record design

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **distinguishes** Phase 10 MDM **entity** lifecycle from Phase 11 **enterprise** data lifecycle.

**Do NOT redesign Phase 10.** Pointer: `10-master-data-management/13-master-data-lifecycle.md`

---

## 2. Phase 10 MDM entity lifecycle (locked — reused, not changed)

Phase 10 records:

```text
Propose entity
→ Define
→ Approve
→ Create
→ Match
→ Merge / Resolve
→ Publish
→ Maintain
→ Change
→ Deactivate
→ Retire
```

The identity-management core of that chain is:

```text
Create → Match → Merge → Publish → Maintain → Deactivate
```

That core is **MDM only**. **Retire** in Phase 10 means the master **entity** is no longer an active identity — **not** an enterprise dispose of all related data.

---

## 3. Phase 11 enterprise data lifecycle (locked)

```text
Create / Acquire
→ Register
→ Classify
→ Store
→ Use
→ Share
→ Retain
→ Archive
→ Dispose
```

---

## 4. Boundary rules `[A][B]`

| Statement | Meaning |
| --- | --- |
| Two lifecycles | MDM governs **shared identity**; Phase 11 governs **data assets/records** from create to dispose |
| Deactivate ≠ Dispose | A deactivated Patient master may still have related clinical/financial data under Retention Schedule |
| No MDM-specific retention rules | Do not invent a Patient-master “keep X” rule. Apply the same retention governance as other assets |
| Golden record remains logical | Phase 10; not a physical store that replaces archive |
| Core MDM cut unchanged | Patient, Provider, Facility (supporting) — not redesigned |

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Two-lifecycle split | Sections 2–4 |
| `[C]` | Reference and Master Data Management domain **name** | Context |
| `[NDMO verification required]` | Official NDMO master-lifecycle vs records specs | Not claimed |
