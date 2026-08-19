# Data Quality Issue Management Procedure

**Document ID:** RHC-DG-PRC-003  
**Version:** 1.0  
**Status:** Implemented (documentation) — **not** a Phase 7 quality framework  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Issue path only; no dimensions or thresholds.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent standard:** RHC-DG-STD-003  

Does **not** define quality dimensions, scorecards, KPIs, or rules. **Phase 7 is Designed / Documented** (quality framework in `07-data-quality/`). Operational implementation and measured performance are not claimed.

---

## 1. Purpose

Govern a data-quality (or data-defect) **issue** from log to close `[B]`.

## 2. Process

```text
Log → Triage → Assign → Resolve → Verify → Close → Escalate when required
```

| Step | Who | Action |
| --- | --- | --- |
| **Log** | Anyone (Consumer, Steward, Custodian) | Data Quality Issue Record; domain if known |
| **Triage** | DMO routing; Steward of likely domain | Confirm Owner domain; not a numeric priority SLA |
| **Assign** | Steward | Owner **A** remains; Custodian **R** if system fix |
| **Resolve** | Steward + Custodian | Fix or Owner-accepted residual |
| **Verify** | Steward | Defect no longer reproduced **or** residual documented |
| **Close** | Data Owner **A** | Issue Record closed; residual documented if accepted |
| **Escalate when required** | Steward → Owner → DGO → CDO → DMC | Cross-domain, ageing, care-safety / cluster-report risk (Phase 3); no numeric SLA |

IT does not close business meaning issues as Owner.

## 3. Inputs / outputs / evidence

| Inputs | Outputs | Evidence |
| --- | --- | --- |
| Issue description; dataset if known | Decision; fix or residual | Data Quality Issue Record |

## 4. Relationship to other procedures

Misclassification → PRC-002. Sharing/access disputes → PRC-005. Policy exceptions → PRC-006. Master-identity duplicates → still this procedure under Patient/Person or Provider Owner (STD-005), without MDM matching design.
