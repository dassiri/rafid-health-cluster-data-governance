# Lineage Registration Workflow

**Document ID:** RHC-DG-P9-012  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (workflow method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Operating workflow; no new Phase 6 procedure; no invented document ID.

**Phase:** 9 — Data lineage  
**Does not decide:** A seventh Phase 6 procedure; ticket SLAs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the **lineage operating workflow** `[A][B]`.

It does **not** create a new Phase 6 procedure. It does **not** invent a document ID.

It **references existing Phase 8 metadata/catalog governance**, including:

**Metadata Registration Procedure**

`06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`

Assets on a lineage path should already be identifiable in the catalog (or registered through that procedure). Lineage metadata then fills Phase 8 Lineage Metadata fields.

---

## 2. Locked workflow

```text
Identify lineage requirement
→ Gather source/target information
→ Document transformation
→ Steward validation
→ Owner validation where required
→ DMO governance check
→ Publish
→ Review/update
```

| Step | Who | Action |
| --- | --- | --- |
| **Identify lineage requirement** | Steward **R**; Owner and DMO on criticality confirm | Candidate vs prioritized coverage ([`05-lineage-criticality.md`](05-lineage-criticality.md)) |
| **Gather source/target information** | Steward **R**; Custodian **C** | Catalog asset IDs, system context |
| **Document transformation** | Steward **R**; Custodian **C** | Conceptual transformation reference — not job code |
| **Steward validation** | Business Data Steward | Completeness of Source → Target → Consumer at the intended granularity |
| **Owner validation where required** | Data Owner **A** | Required when the flow’s **business meaning** is at stake (business lineage correctness) |
| **DMO governance check** | DMO | Method, registry consistency, no rewritten clinical/finance meaning |
| **Publish** | Steward / DMO | Lineage metadata on the catalog asset; Critical Lineage Register if confirmed |
| **Review/update** | Steward **R** | On change triggers ([`14-change-management.md`](14-change-management.md)) |

No numeric SLA.

---

## 3. Exceptions

Out-of-policy lineage handling reuses:

**Data Governance Exception Procedure**

`06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md`

**DMC = A** (existing right). No new exception procedure.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Operating workflow | Section 2 |
| `[C]` | Catalog domain **name** | Context |
| `[NDMO verification required]` | Official NDMO lineage-registration procedure | Not claimed |
