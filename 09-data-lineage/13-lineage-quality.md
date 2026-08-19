# Lineage Quality

**Document ID:** RHC-DG-P9-013  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (lineage-quality method); Data Owner **A** for accepting residual risk on domain flows  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Five lineage-quality attributes; no enterprise numeric targets.

**Phase:** 9 — Data lineage  
**Does not decide:** A lineage scorecard with cluster-wide percentages

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document defines **quality of the lineage description**, not quality of the data (Phase 7).

No **enterprise numeric targets** are set. Any example check that used a number would have to be `[A] Illustrative`; **none is set as a target here**.

---

## 2. Five attributes (locked) — defined for lineage

| Attribute | Meaning for lineage |
| --- | --- |
| **Completeness** | Agreed Source, Transformation, Target, and Consumer are recorded at the intended granularity for that flow. |
| **Accuracy** | The described path matches Owner-accepted business movement (the data actually goes that way as understood). |
| **Timeliness** | The lineage record is updated when an approved change trigger fires (qualitative — **no numeric SLA**). |
| **Consistency** | The same asset is not given contradictory upstream/downstream statements across registry and catalog. |
| **Traceability** | A reader can follow Source → Target → Consumer and see Owner/Steward on each asset. |

These names overlap Phase 7 **data**-quality names on purpose as vocabulary reuse. They are **applied to lineage records**, not to CDEs. This is **not** a second Data Quality Framework.

---

## 3. Illustrative checks `[A][B]` (non-numeric)

| Check | Pass when |
| --- | --- |
| Completeness | MVP Critical Lineage records have upstream, downstream, and transformation reference populated or explicitly “not yet known” |
| Accuracy | Owner has validated business lineage where required |
| Timeliness | Change Record exists after a listed trigger (process evidence, not a clock) |
| Consistency | Catalog Lineage Metadata matches the Lineage Record |
| Traceability | Each hop names a catalog asset (or documented gap) |

Do not convert these into cluster percentages in this phase.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Five attributes and checks | Sections 2–3 |
| `[C]` | Trusted Data principle **name** (transparency) | Context |
| `[NDMO verification required]` | Official NDMO lineage-quality metrics | Not claimed |
