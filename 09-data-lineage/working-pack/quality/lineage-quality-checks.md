# Lineage Quality Checks (Working Pack)

**Document ID:** RHC-DG-P9-WP-012  
**Version:** 1.0  
**Status:** Implemented (illustrative checks only — no numeric targets)  
**Owner:** DMO `[B]` (lineage-quality method); Data Owner **A** for accepting residual risk on domain flows  
**Parent design:** [`../../13-lineage-quality.md`](../../13-lineage-quality.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

---

## 1. This is lineage metadata quality — not a second Data Quality Framework

**Data quality (Phase 7)** asks whether the **data** is correct: for example, whether National ID is unique, or whether a diagnosis code is valid.

**Lineage quality (this file)** asks whether the **lineage description** is correct, complete, current, and followable.

| Question | Framework | Example |
| --- | --- | --- |
| Is the National ID on the master unique? | Phase 7 data quality | DQ-001 on CDE-001 |
| Is the hop Registration → Patient Master documented with source, target, Owner, and transformation? | Lineage quality | Completeness of LIN-001 |

A complete lineage record can describe a path that still carries poor-quality **data**. A high-quality CDE can still have an incomplete **lineage** record. The two assessments are related through impact analysis ([`../../08-lineage-and-quality.md`](../../08-lineage-and-quality.md)). They are not the same scorecard.

This is **not** a second Data Quality Framework. Dimension **names** are reused as vocabulary. They are applied to **lineage records**, not to CDEs.

No enterprise numeric targets are set.

---

## 2. Locked lineage-quality attributes (Phase 9)

| Attribute | Meaning for lineage |
| --- | --- |
| **Completeness** | Agreed Source, Transformation, Target, and Consumer are recorded at the intended granularity |
| **Accuracy** | The described path matches Owner-accepted business movement |
| **Timeliness** | The lineage record is updated when an approved change trigger fires (qualitative — **no numeric SLA**) |
| **Consistency** | The same asset is not given contradictory upstream/downstream statements across registry and catalog |
| **Traceability** | A reader can follow Source → Target → Consumer and see Owner/Steward on each asset |

---

## 3. Validity as an applied record check `[A][B]`

Phase 8 metadata quality also uses **Validity** (coded values in an allowed list). This pack applies the same idea to **lineage records**, without replacing Traceability.

**Validity (lineage record):** Lineage Type, Criticality, catalog Asset IDs, and CDE references use allowed project values (the four lineage types; Critical / Important / Standard; existing `META-*` IDs; the 13 catalogue CDEs only).

A lineage record is **invalid** if, for example, it invents a 14th CDE, a fourth MVP domain, or a lineage type that is not Business / Conceptual / Technical / End-to-End.

---

## 4. When a lineage record is incomplete

A lineage record is incomplete if any of the following required items is missing **at the intended granularity**:

- Source is missing  
- Target is missing  
- Owner is missing  
- Transformation is missing where required (or not explicitly “not yet known”)  
- Criticality is missing where required (confirmed coverage rows)  
- Consumer is missing on Year-1 Critical hops  
- Catalog Asset ID is missing where the node is a catalogued asset  

“Not yet known” is a valid completeness pattern when explicitly recorded. Inventing a fake transformation to look complete is **not** allowed.

---

## 5. Illustrative checks applied to this pack `[A]`

| Check | Pass when | Applied result (this pack) |
| --- | --- | --- |
| Completeness | Critical rows have source, target, transformation, consumer, Owner, Steward, criticality | LIN-001–LIN-008 populated in the CSV |
| Accuracy | Owner has validated business lineage where required | Validation Status = Published (illustrative Owner acceptance) |
| Timeliness | Change Record exists after a listed trigger | Last Reviewed = 2026-08-15; no fake clock SLA |
| Consistency | Catalog Lineage Reference matches the Lineage Record | Chain IDs `LIN-REG-PAT-001`, `LIN-ENC-001`, `LIN-CLM-001` reused |
| Traceability | Each hop names a catalog asset **or** a documented consumer gap | Consumer-only KPI/reporting nodes labelled `n/a — business consumer` |
| Validity (applied) | Types, IDs, CDEs, and domains are project-allowed values | No new CDEs; three MVP domains only |

Do not convert these into cluster percentages.

---

## 6. Worked incomplete vs complete (teaching)

| Record | Completeness issue | Treatment |
| --- | --- | --- |
| Hypothetical draft: “Claims → reporting” with no source asset ID and no Owner | Incomplete | Remain Pending Steward Validation |
| LIN-001 | Source META-PAT-002, target META-PAT-001, transformation named, Owner and Steward present, Critical confirmed | Complete at Levels 1–2 |
| LIN-013 | Level 4 hop for a **non-CDE**; Standard priority | Complete **as Standard** — completeness does not promote Encounter_ID to a CDE |

---

## 7. Relationship to data-quality impact analysis

When a Phase 7 defect is logged, lineage supports **impact analysis**:

```text
Quality failure in a source field
→ downstream dataset
→ downstream process/report
→ KPI
```

Example (illustrative, not measured): invalid Diagnosis_Code (DQ-002 / CDE-003) → Claim Submission Dataset (LIN-008 / LIN-003) → interchange rejection risk → Patient Claim Rejection Rate (LIN-005).

Issues still follow the Phase 6 Data Quality Issue Management Procedure. Lineage does not replace it.

---

## 8. What this file does not do

- Does not create a second Data Quality Framework
- Does not add CDEs, dimensions, or thresholds
- Does not set cluster-wide lineage completeness percentages
- Does not claim official NDMO lineage-quality metrics `[NDMO verification required]`
