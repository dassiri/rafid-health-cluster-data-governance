# Lineage Criticality (Working Pack)

**Document ID:** RHC-DG-P9-WP-003  
**Version:** 1.0  
**Status:** Implemented (applied working labels only)  
**Owner:** Data Owner **A** (confirm coverage in the domain); DMO (method) `[B]`  
**Parent design:** [`../../05-lineage-criticality.md`](../../05-lineage-criticality.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**This is a Rafid illustrative lineage criticality approach.** It is **not** an official NDMO criticality scale `[NDMO verification required]`.

---

## 1. Purpose

Phase 9 already locks **how a flow becomes prioritized lineage**:

> A lineage candidate is identified when one or more criteria indicate material business impact or governance value. The Data Owner, Steward, and DMO then confirm whether prioritized lineage coverage is warranted.

There is **no numeric scoring**. A single criterion does **not** automatically make a flow Critical Lineage.

This working pack adds a **coverage label** after that two-step confirmation so the register can be read in a portfolio review. The nine criteria are unchanged.

---

## 2. Nine candidacy criteria (locked — reused)

1. Critical Data Element (confirmed Phase 7 CDE)  
2. Patient safety  
3. Regulatory impact — only where verified; otherwise `[NDMO verification required]`  
4. Financial impact  
5. Executive reporting  
6. Cross-domain dependency  
7. External data sharing  
8. Data quality history  
9. Master data dependency  

A criterion signals **candidacy**. Confirmation is a separate Owner / Steward / DMO step.

---

## 3. Working coverage labels `[A][B]`

| Label | Meaning in this pack | Relation to Phase 9 |
| --- | --- | --- |
| **Critical** | Lineage is required now. Recorded on the Critical Lineage Register. Typically Levels 1–2; Level 4 only where a CDE or investigation warrants it. | Confirmed **prioritized lineage coverage** |
| **Important** | Lineage is strongly recommended. Documented on the Lineage Registry. Not every Important row is on the Critical Lineage Register in Year-1. | Candidate confirmed as **coverage recommended**, not Year-1 Critical Register focus |
| **Standard** | Lineage is maintained where useful. Same register fields, lower operating priority. | Coarse catalog pointer may exist without Year-1 deep coverage |

These three labels are **Rafid working language**. They are not NDMO national criticality levels.

---

## 4. When Critical is used in this pack

A hop is labelled **Critical** only when:

- one or more of the nine criteria fire, **and**
- Owner, Steward, and DMO are treated as having confirmed Year-1 prioritized coverage (illustrative confirmation, not a live meeting minute).

Typical Critical reasons in the register:

| Reason | Typical assets |
| --- | --- |
| Supports critical reporting / executive use | Patient Claim Rejection Rate |
| CDE on the path | CDE-001, CDE-002, CDE-003, CDE-007 |
| Master-data dependency | Patient Master (META-PAT-001) |
| Cross-domain movement | Patient → Encounter; Encounter → Claims |
| External sharing consumer | Claims → External Claims Interchange |
| Material financial impact | Claims extract hops |

---

## 5. When Important or Standard is used

| Label | Used when |
| --- | --- |
| **Important** | The hop supports important operational processes, has multiple downstream consumers, or has meaningful quality / ownership implications, but Year-1 deep coverage is not the Critical Register focus. Example: Charge_Code (CDE-008) field hop; Encounter_Date operational reporting. |
| **Standard** | Useful operational identity (for example Encounter_ID, which is **not** a catalogue CDE) where lineage is recorded for completeness of the teaching register. |

CDE status **candidacy** does not force every CDE hop onto the Critical Lineage Register. Charge_Code remains a confirmed CDE in Phase 7; this pack treats its **field-level** lineage as Important so Year-1 Level 4 stays selective.

---

## 6. Applied to the register

| Label | Lineage IDs |
| --- | --- |
| Critical | LIN-001, LIN-002, LIN-003, LIN-004, LIN-005, LIN-006, LIN-007, LIN-008 |
| Important | LIN-009, LIN-010, LIN-011, LIN-012 |
| Standard | LIN-013 |

MVP priority mapping is in [`lineage-mvp-scope.md`](lineage-mvp-scope.md). Critical ≈ Priority 1; Important ≈ Priority 2; Standard ≈ Priority 3.

---

## 7. What this file does not do

- Does not replace the nine criteria or the two-step rule
- Does not invent official NDMO criticality levels
- Does not score lineage numerically
- Does not auto-promote a candidate because a CDE is present
