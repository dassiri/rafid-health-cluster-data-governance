# End-to-End Lineage Example `[A]`

**Label:** `[A]` Fictional / illustrative Rafid assumption  
**Does not claim:** A production pipeline, scanner, ETL architecture, or real MOH/NPHIES design

---

## Purpose

One **business / conceptual** lineage story. Technical lineage remains conceptual (Phase 9). Field-level lineage is **not** enterprise-wide.

This example is **illustrative**. It does not represent real Rafid, MOH, or national-interchange architecture.

Classification is **Owner-assessed** with the Phase 5 method. Downstream data does **not** automatically inherit the highest upstream tier.

---

## Flow

```text
Patient Registration
    → EHR / Source System (conceptual)
    → Transformation / Integration (conceptual)
    → Data Warehouse (conceptual)
    → Analytics Dataset
    → BI Dashboard (conceptual consumer)
```

---

## Nodes

| Step | Asset (sample ID) | Owner | Steward | Classification `[A][B]` | CDE | Quality control (illustrative) | Transformation concept |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1. Patient Registration | CAT-A01 | Patient Access & Experience Director | Business Data Steward | Restricted | CDE-001, CDE-002 | DQ-001 / DQ-003 on identity | Capture identity at registration |
| 2. EHR / Source System | CAT-A02 / CAT-A04 | Patient Access & Experience Director (person); CMO (encounter) | Business Data Steward | Restricted | CDE-001–004 | Completeness/validity on identity and diagnosis | Persist identity; create encounter |
| 3. Transformation / Integration | CAT-A10 | CMO (encounter link); Patient Access Owner **C** on identity keys | Business Data Steward | Restricted | CDE-002 | Key consistency (MRN) | Conceptual join; no claimed ETL tool |
| 4. Data Warehouse | CAT-A09 (claims slice) / identity keys | CFO (claims facts); Patient Access Owner **A** for person keys used | Business Data Steward | Confidential (claims fact grain — Owner-assessed, not auto-inherited) | CDE-007, CDE-002 | DQ-005 uniqueness on claim ID | Aggregate/conform for reporting — conceptual |
| 5. Analytics Dataset | CAT-A09 | Chief Financial Officer (CFO) | Business Data Steward | Confidential | CDE-007 | Completeness of claim ID in the extract | Derived from warehouse |
| 6. BI Dashboard | CAT-A14 | Chief Financial Officer (CFO) | Business Data Steward | Internal | — | Catalog certification = internal trust only | Display; not a data store |

Restricted registration data does **not** force the dashboard to Restricted. The CFO (or relevant Owner) **reassesses** the consumer asset with Phase 5. Tokenization, aggregation, or removal of identifiers **may** change sensitivity — still Owner **A**.

---

## Lineage types in this example

| Type | Year-1 treatment |
| --- | --- |
| Business lineage | **Shown** — who uses what, for what purpose |
| Conceptual lineage | **Shown** — Source → Transformation → Target → Consumer |
| Technical lineage | **Conceptual only** — no job names, schemas, or scanners |

---

## Why this flow is a lineage candidate (nine criteria — not auto-critical)

Identity (patient safety), financial reporting, cross-domain keys, and Restricted/Confidential handling fire **candidacy**. Critical Lineage confirmation still requires Data Owner, Steward, and DMO (Phase 9). This file does **not** auto-register Critical Lineage.

---

## Related designs

- Phase 9 worked example (registration → claims interchange): [`09-data-lineage/06-worked-example.md`](../../09-data-lineage/06-worked-example.md)  
- Catalog sample: [`02-catalog-sample.md`](02-catalog-sample.md)  
- Quality example: [`01-data-quality-example.md`](01-data-quality-example.md)
