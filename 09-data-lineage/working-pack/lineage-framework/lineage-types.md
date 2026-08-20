# Lineage Types (Working Pack)

**Document ID:** RHC-DG-P9-WP-002  
**Version:** 1.0  
**Status:** Implemented (applied examples only)  
**Owner:** DMO `[B]` (type method)  
**Parent design:** [`../../02-lineage-types.md`](../../02-lineage-types.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

This file **applies** the four locked Phase 9 lineage types to working records. It does not rename the types and does not claim they are NDMO-required names `[NDMO verification required]`.

Year-1 priorities remain locked: Business and Conceptual are **priority**; Technical is **conceptual / selective only**; End-to-End is **one worked example**.

---

## 2. Business lineage (Year-1 priority)

Business lineage shows the **business flow and meaning** of data: process → business data asset → business outcome.

```text
Patient Registration
        ↓
Patient Master Record
        ↓
Clinical Encounter
        ↓
Healthcare / claims reporting
```

Focus: business processes, business assets, business purpose, ownership, and governance meaning.

Working records: [`../business-lineage/business-lineage-examples.md`](../business-lineage/business-lineage-examples.md)  
Locked teaching example: [`../../07-business-lineage-example.md`](../../07-business-lineage-example.md) (Patient Claim Rejection Rate).

---

## 3. Conceptual lineage (Year-1 priority)

Conceptual lineage shows movement between **major logical data structures** at asset / system-class level, without job code.

```text
Patient source (registration / MPI)
      ↓
Patient Master
      ↓
Clinical data domain (encounter)
      ↓
Billing / claims extract
      ↓
Consumer (external interchange or reporting)
```

Focus: domains, major assets, conceptual transformations, flows, and consumers.

Pattern remains:

```text
Source → Transformation → Target → Consumer
```

Working records: [`../conceptual-lineage/conceptual-lineage-maps.md`](../conceptual-lineage/conceptual-lineage-maps.md)  
Locked E2E chain: [`../../06-worked-example.md`](../../06-worked-example.md).

---

## 4. Selective technical / field-level lineage (conceptual only)

Technical lineage in Year-1 is a **description pattern**, not a scanner.

Granularity (locked):

| Level | Name | Year-1 |
| --- | --- | --- |
| Level 1 | Business | Priority-domain KPIs |
| Level 2 | Dataset / Asset | MVP assets |
| Level 3 | Structure / Object | Only when a CDE or governance issue requires it |
| Level 4 | Data Element / Field | **Selective only** |

Field-level lineage is **not** enterprise-wide. It is used here only where a confirmed CDE or a reporting count requires it.

```text
SYN-REG.patient_master.patient_id
        ↓
Patient (META-PAT-001 / CDE-002)
        ↓
emr.clinical.encounter_documentation.patient_id
```

Working records: [`../technical-lineage/selective-technical-lineage.md`](../technical-lineage/selective-technical-lineage.md)

These examples are **synthetic / illustrative / non-production**. They do not claim an ETL engine, Purview scan, or production column graph.

---

## 5. End-to-end lineage (one worked example)

The single detailed end-to-end example remains:

```text
Patient Registration
→ Patient Master
→ Clinical Encounter
→ Billing / Claims
→ External Claims Interchange
```

This pack **instantiates** that chain as register hops `LIN-001`–`LIN-004`. It does not add a second E2E architecture. External Claims Interchange remains **generic**. It is not NPHIES or a named national product.

---

## 6. How the register uses types

| Lineage type | Register rows (illustrative) |
| --- | --- |
| Business | LIN-001, LIN-005, LIN-010, LIN-012 |
| Conceptual | LIN-001, LIN-002, LIN-003, LIN-004, LIN-011, LIN-012 |
| Technical (selective Level 4) | LIN-006, LIN-007, LIN-008, LIN-009, LIN-013 |
| End-to-end (chain, not a fifth type on every row) | LIN-001 → LIN-004 instantiate the locked E2E example |

A row may carry Business **and** Conceptual where the same hop is both a business process step and an asset-level flow. That does not create a new type.

---

## 7. What this file does not do

- Does not build enterprise-wide technical lineage
- Does not invent a fifth lineage type
- Does not treat Purview or Collibra screenshots as evidence
