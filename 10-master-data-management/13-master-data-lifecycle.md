# Master Data Lifecycle

**Document ID:** RHC-DG-P10-013  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for definition/domain rules; DMO (lifecycle method) `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — MDM-entity lifecycle only; DMC not routine approver.

**Phase:** 10 — Master data management  
**Does not decide:** Retention/archive/disposal (Phase 11)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This lifecycle applies **only to MDM entities**. It is **not** the enterprise data-lifecycle framework. Enterprise Create→Dispose governance is Phase 11 (`11-data-lifecycle/`). This file is **not** redesigned.

---

## 2. Locked lifecycle

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

---

## 3. Approval rule (locked)

> Approve (Data Owner approves the business definition and domain rules; DMC handles escalation within its existing Phase 3 governance authority and decision-right framework).

This must **not** be read as DMC routinely approving every master entity.

**No new DMC decision right.**

| Step | A / R |
| --- | --- |
| Propose / Define | Steward **R**; Owner **A** |
| **Approve** | **Data Owner** for business definition and domain rules |
| Create / Match / Merge | Steward **R**; Custodian technical; Owner **A** for merge **intent** |
| Publish | Steward / DMO (catalog Master Data Entity) |
| Maintain / Change | Owner **A** for meaning; Steward **R** |
| Deactivate / Retire | Owner **A**; DMO record-keeping |

DMC appears only for **escalation** already in Phase 3 (policy, material exception, Owner non-participation, residual sharing risk) — not a “sign every Patient create” queue.

---

## 4. Duplicate resolution (conceptual)

Match → manual review → Owner merge/split **intent** → Custodian implements in existing systems. No matching engine. False positive/negative handling as in [`06-matching-duplicate-management.md`](06-matching-duplicate-management.md).

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | MDM-only lifecycle; approval split | Sections 2–3 |
| `[C]` | Role **names** | Context |
| `[NDMO verification required]` | Official NDMO master-lifecycle specifications | Not claimed |
