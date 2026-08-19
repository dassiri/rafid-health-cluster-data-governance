# Data Classification Procedure

**Document ID:** RHC-DG-PRC-002  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Implements Phase 5 / STD-002.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent standard:** RHC-DG-STD-002  

Rafid tiers **Public / Internal / Confidential / Restricted** `[A][B]` are **not** NDMO national tiers `[NDMO verification required]`.

---

## 1. Purpose

Classify a **dataset** and keep the Classification Registry current `[B]`.

## 2. Process

```text
Identify dataset
  → Propose classification
  → Data Owner approval
  → Registry
  → Technical implementation
  → Review / Reclassification
```

| Step | Who | Action |
| --- | --- | --- |
| Identify dataset | Steward; Custodian **C** | Name, domain, systems; one Owner **A** (STD-001) |
| Propose classification | Steward | Qualitative highest-impact narrative; **no score**; PDPO **C** if personal |
| Data Owner approval | Data Owner **A** | Approve Rafid tier |
| Registry | Steward **R**; DMO completeness **A** | Classification Registry fields (Phase 5) |
| Technical implementation | Custodian **R** | Handling only; **does not pick** the tier |
| Review / Reclassification | Steward flags; Owner **A** | Triggers in Phase 5; **only Owner** approves change |

## 3. Data states

New, existing (unlabeled ≠ Public), imported (receiving Owner **A**), derived/aggregated (highest impact default), shared (does not auto-downgrade), archived (tier persists) — Phase 5.

## 4. Escalation

Owner silent: DMO → CDO → DMC (Phase 3). Security block on implementation: CISO path **and** CDO; still not IT classification **A**.

## 5. Evidence

Registry row; Owner approval date; rationale; related systems. Restricted external share is **not** this procedure — use PRC-005.
