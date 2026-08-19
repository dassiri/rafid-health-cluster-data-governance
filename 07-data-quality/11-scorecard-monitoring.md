# Scorecard and Monitoring

**Document ID:** RHC-DG-P7-011  
**Version:** 1.0  
**Status:** Implemented (illustrative scorecard only)  
**Owner:** DMO (scorecard method) `[B]`; Data Owner **A** for domain interpretation  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Approved scorecard columns; Phase 3 cadence conceptual; no numeric SLAs.

**Phase:** 7 — Data quality  
**Does not decide:** BI tool; Phase 12 KPI pack; live Rafid results

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **scorecard structure** and **monitoring cadence** for data quality `[A][B]`.

Example cell values are **illustrative only** `[A]`. They are **not** fabricated as real Rafid performance. They exist to show how a row is read.

---

## 2. Approved scorecard structure (locked)

| Column | Content |
| --- | --- |
| Domain | Phase 4 domain name |
| CDE | Confirmed CDE ID and field name |
| Dimension | One of the seven Rafid dimensions |
| Current score | Per-dimension metric or exception count — **illustrative in this file** |
| Target | From the threshold method — **`[A] Illustrative Rafid target` when numeric** |
| Trend | Qualitative (improving / stable / worsening) — not a fake time series |
| Open issues | Count or reference to Issue Register (illustrative) |
| Breaches | Whether Warning or Breach is crossed (illustrative) |
| Owner | Phase 4 Data Owner title |
| Status | Qualitative (in target / watch / breach / not yet measurable) |

No extra hidden index column. No enterprise-wide single score (see [`07-quality-scoring.md`](07-quality-scoring.md)).

---

## 3. Illustrative rows `[A]` — not Rafid measured performance

The numbers below are **`[A] Illustrative Rafid target` / illustrative current values**. They are **not** audit findings and **not** live cluster results.

| Domain | CDE | Dimension | Current score `[A]` illustrative | Target `[A]` Illustrative Rafid target | Trend `[A]` | Open issues `[A]` | Breaches `[A]` | Owner | Status `[A]` |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Patient / Person Master Data | CDE-001 National ID | Uniqueness | 2 duplicate groups (example) | 0 duplicate groups | Worsening (example) | 1 open (example) | Breach (example) | Patient Access & Experience Director | Breach — example only |
| Clinical / Medical Records Data | CDE-003 Diagnosis code | Validity | 97.2% (example) | 99% | Stable (example) | 0 (example) | Warning (example) | Chief Medical Officer (CMO) | Watch — example only |
| Provider / Clinician Data | CDE-006 Credential expiry date | Timeliness | 0 undetected (example) | 0 | Stable (example) | 0 (example) | None (example) | Medical Affairs Officer | In target — example only |
| Reference / Organizational Master Data | CDE-013 Facility / department code | Integrity | Not yet measurable (example) | 0 orphan codes | n/a | 0 (example) | n/a | Strategy & Planning Director | Not yet measurable — example only |

Do **not** brief these rows as Rafid’s actual quality.

---

## 4. Monitoring cadence (Phase 3 — conceptual, not redesigned)

| Forum | Quality use | Frequency (Phase 3 — qualitative) |
| --- | --- | --- |
| **Steward operational monitoring** | Rule exceptions, issue log hygiene, scorecard refresh | Ongoing operational work — **no numeric SLA** |
| **Domain Huddle** | Review CDE scores, breaches, closures, residual risk | Biweekly or monthly by domain risk |
| **Steward Forum** | Cross-domain themes, clash detection | Monthly |
| **DMC summarized reporting** | Material breaches, Owner non-participation, residual enterprise risk | Quarterly + extraordinary for material patient-safety or regulatory data incidents |

CDO does not chair DMC. DGO is secretariat (non-member). This file does not change Year-1 DMC membership.

---

## 5. What monitoring is not

- Not a numeric SLA pack
- Not Phase 12 maturity scores
- Not NDMO annual assessment evidence
- Not a catalog product dashboard (Phase 8 is Designed / Documented as conceptual catalog design; no catalog product is implemented)

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative scorecard cells | Section 3 |
| `[B]` | Scorecard columns; forum use | Sections 2, 4 |
| `[C]` | Entity Data Management Committee **name** | DMC |
| `[NDMO verification required]` | Official NDMO scorecard mandates | Not claimed |
