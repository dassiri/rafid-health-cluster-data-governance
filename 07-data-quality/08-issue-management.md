# Data Quality Issue Management

**Document ID:** RHC-DG-P7-008  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO (method) `[B]`; Data Owner **A** for issue closure in the domain  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Integrates Phase 6 issue procedure; four-level severity `[A][B]`.

**Phase:** 7 — Data quality  
**Does not decide:** Ticket-tool vendor; numeric SLAs; a second issue process

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records how Phase 7 **uses** the Phase 6 issue path, with quality-specific severity, RCA, and trend analysis `[A][B]`.

It does **not** create a parallel procedure. It does **not** redesign Phase 6.

---

## 2. Phase 6 procedure (mandatory reference)

Quality defects that affect fitness for use follow:

**Data Quality Issue Management Procedure**

`06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`

That file also records Document ID **RHC-DG-PRC-003**. This Phase 7 file refers to the procedure **by title and full repository path** as required.

Phase 6 process (unchanged):

```text
Log → Triage → Assign → Resolve → Verify → Close → Escalate when required
```

**Close** remains **Data Owner A**. IT does not close business-meaning issues as Owner.

---

## 3. Quality lifecycle mapping (locked)

Phase 7 expresses the same path with quality-analysis steps inserted. This is **not** a second procedure.

```text
Issue detected
→ Log
→ Triage
→ Severity
→ Assign Owner/Steward
→ Root Cause
→ Remediation
→ Verification
→ Closure
→ Trend Analysis
```

| Phase 7 step | Phase 6 step | Notes |
| --- | --- | --- |
| Issue detected | (before Log) | Monitoring, consumer report, or rule breach |
| Log | Log | Data Quality Issue Record |
| Triage | Triage | DMO routing; Steward of likely domain; no numeric priority SLA |
| Severity | (quality overlay) | Critical / High / Medium / Low `[A][B]` — does not replace triage |
| Assign Owner/Steward | Assign | Owner **A** remains; Custodian **R** if system fix |
| Root Cause | part of Resolve | Lightweight categories — [`09-root-cause-analysis.md`](09-root-cause-analysis.md) |
| Remediation | Resolve | [`10-remediation.md`](10-remediation.md) |
| Verification | Verify | Steward |
| Closure | Close | Data Owner **A** |
| Trend Analysis | (after Close) | Steward Forum / Domain Huddle / DMC summary — not a Phase 12 KPI pack |

**Escalate when required** remains Steward → Owner → DGO → CDO → DMC (Phase 3). Cross-domain, qualitative ageing, care-safety or cluster-report risk. **No numeric SLA.**

---

## 4. Severity model `[A][B]`

Four levels. This is a **Rafid design choice** informed by common practice. It is **not** an NDMO-mandated severity catalogue `[NDMO verification required]`.

| Severity | Use when (qualitative) |
| --- | --- |
| **Critical** | Patient safety, material regulatory exposure, or financial integrity is immediately at risk (for example undetected expired credentials; duplicate National ID affecting care identity). |
| **High** | Material operational, coding, billing, or decision impact; workaround is painful or unsafe if ignored. |
| **Medium** | Contained defect; workaround exists; still must be visible and owned. |
| **Low** | Limited local impact; still logged if it affects a CDE or a stated rule. |

Severity is **not** a clock. Critical does not create a numeric “fix in N hours” SLA in this framework.

Default severities on illustrative rules (DQ-001 … DQ-008) are starting labels only `[A]`. The Steward may propose a change; the Owner **A** confirms for that issue.

---

## 5. Privacy overlay

If the issue involves personal data or privacy implications, **PDPO is Consulted**. PDPO does **not** become Data Owner of the quality defect. Sharing/access disputes remain the Data Access / Sharing Governance Procedure; they are not merged into quality close.

---

## 6. Related procedures (do not merge)

| Situation | Path |
| --- | --- |
| Quality / fitness-for-use defect | This file + Data Quality Issue Management Procedure (path in §2) |
| Misclassification | Data Classification Procedure |
| Sharing / access | Data Access / Sharing Governance Procedure (two As: Owner business; PDPO privacy) |
| Out-of-policy exception | Data Governance Exception Procedure (**DMC = A**) |

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Four-level severity; quality overlay on Phase 6 path | Sections 3–4 |
| `[C]` | Data Quality domain **name**; PDPO **name** | Context |
| `[NDMO verification required]` | Official NDMO issue-severity or SLA mandates | Not claimed |
