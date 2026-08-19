# Asset Registration Workflow

**Document ID:** RHC-DG-P8-007  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (workflow method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Operating workflow consistent with Phase 6; procedure not redesigned.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Ticket tool; numeric SLAs; a second registration procedure

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **catalog operating workflow** for asset registration `[A][B]`.

It is **consistent with** Phase 6. It does **not** redesign the Phase 6 procedure. It does **not** invent a document ID for that procedure.

---

## 2. Phase 6 procedure (mandatory reference)

Registration **shall** follow:

**Metadata Registration Procedure**

`06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`

Phase 6 steps (unchanged):

```text
Identify dataset
  → Document business definition
  → Register metadata
  → Link classification
  → Maintain
```

---

## 3. Phase 8 operating workflow (locked)

```text
Identify
→ Submit metadata
→ Steward validation
→ Owner approval where required
→ DMO governance check
→ Publish
→ Maintain
```

| Step | Who | Action | Phase 6 alignment |
| --- | --- | --- | --- |
| **Identify** | Business Data Steward; Custodian **C** | Same unit as classification/registration | Identify dataset |
| **Submit metadata** | Steward **R** | Mandatory fields completed; classification linked or PRC-002 completed first | Document definition + Register + Link classification |
| **Steward validation** | Business Data Steward | Completeness of mandatory categories; definition readable; no Restricted **data** pasted into the record | Register |
| **Owner approval where required** | Data Owner **A** | Required for business definition / catalog content (Phase 4 rows 1 and 8) and for **Certified** status | Document business definition (Owner **A**) |
| **DMO governance check** | DMO | Method completeness, domain/Owner consistency, classification present — DMO does **not** rewrite clinical or finance meaning | DMO completeness |
| **Publish** | Steward / DMO | Metadata discoverable; status at least Registered | (result of Register) |
| **Maintain** | Steward **R** | Update on definition, system context, Owner, or classification change | Maintain |

**Unlabeled is not Public.** If classification is missing, complete the Data Classification Procedure before publish.

No numeric SLA.

---

## 4. Escalation (existing paths only)

| Situation | Path |
| --- | --- |
| Definition dispute | Data Owner |
| Cross-domain clash | DMO / CDO; DMC only under **existing** Phase 3 classes (not a new catalog-appeal right) |
| Out-of-policy metadata/catalog exception | **Data Governance Exception Procedure** — `06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md` (**DMC = A**) |

DMO cannot rewrite meaning to “complete” the register (Phase 6).

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Operating workflow mapping | Section 3 |
| `[C]` | Data Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Official NDMO registration procedure | Not claimed |
