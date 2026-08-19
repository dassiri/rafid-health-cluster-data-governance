# Data Quality Standard

**Document ID:** RHC-DG-STD-003  
**Version:** 1.0  
**Status:** Implemented (documentation) — **governance-level only**  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Governance requirements only; Phase 7 framework not built.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent policy:** RHC-DG-POL-001  
**Procedure:** RHC-DG-PRC-003  

Trusted Data is an NDMO guiding principle **name** `[C]`. Data Quality is an NDMO knowledge-domain **name** `[C]`. This Standard does **not** implement that domain. No dimensions catalogue, thresholds, scorecards, KPIs, numeric targets, or quality-rule library. **Phase 7 is Designed / Documented** (quality framework in `07-data-quality/`; this Standard remains the governance parent). Operational implementation and measured performance are not claimed. No control IDs. No compliance claim.

---

## 1. Purpose

State **who is accountable** for data quality and how quality **issues** are governed `[B]`, without defining the future quality framework.

---

## 2. Data quality accountability

| Role | Accountability |
| --- | --- |
| Data Owner | **A** for quality **rules** (when defined) and **issue resolution** in the domain (Phase 4) |
| Business Data Steward | **R** — detect, describe, chase, verify operationally |
| Custodian | **R** for **technical** fixes; never **A** for business quality |
| DMO | Coordinates process, ageing visibility, Steward Forum themes |
| Consumer | Raises defects; does not close Owner accountability |

Poor quality in a domain is the **Owner’s** accountability, not the CIO’s.

---

## 3. Owner responsibilities

- Accept (when Phase 7 exists) domain quality expectations as business rules — **not defined here**
- Decide issue closure or acceptable residual risk within Policy
- Escalate cross-domain clashes via DMO/CDO/DMC (Phase 3)

---

## 4. Steward responsibilities

- Log issues per PRC-003
- Investigate with Custodian
- Do not silently “fix meaning” without Owner approval

---

## 5. Issue governance

All quality defects that affect fitness for use **shall** follow PRC-003: Log → Triage → Assign → Resolve → Verify → Close → Escalate when required. No numeric SLA. Escalation uses qualitative ageing and Phase 3 forums.

---

## 6. Quality governance expectations `[B]`

- Known issues are visible (issue record), not only in email
- Fixes do not bypass classification or sharing rules
- DMO may report issue **themes** to DMC, not a Phase 12 scorecard (not built)

---

## 7. Relationship to PRC-003 and Phase 7

| Now | Later (Phase 7 — not this Standard) |
| --- | --- |
| Accountability and issue process | Dimensions, rules, thresholds, monitoring design |

STD-003 **requires** use of PRC-003. It does **not** authorize a parallel local quality process.
