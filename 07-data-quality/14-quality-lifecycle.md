# Data Quality Lifecycle

**Document ID:** RHC-DG-P7-014  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO (lifecycle method) `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Identify-to-Improve lifecycle; ownership applied throughout.

**Phase:** 7 — Data quality  
**Does not decide:** A separate data-lifecycle / retention framework (Phase 11); Phase 5 classification lifecycle

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **data quality lifecycle** (how quality work runs over time) `[A][B]`.

It is **not** the enterprise data retention/lifecycle framework (Phase 11). Classification of datasets remains Phase 5. This lifecycle is about **quality management of CDEs and issues**.

---

## 2. Approved quality lifecycle (locked)

```text
Identify
→ Define
→ Measure
→ Monitor
→ Detect
→ Remediate
→ Verify
→ Report
→ Improve
```

This lifecycle **sits inside** the closed-loop framework in [`01-framework-overview.md`](01-framework-overview.md). It does not replace it.

---

## 3. Ownership throughout `[B]` (Phase 4 not redesigned)

| Stage | Data Owner | Business Data Steward | Custodian | DMO | DMC | PDPO |
| --- | --- | --- | --- | --- | --- | --- |
| **Identify** | **A** (confirms CDE) | **R** (candidate + criteria) | C (location) | Method / routing | I | C if privacy/security impact |
| **Define** | **A** (business meaning and rule) | **R** | C | C | I | C if personal data definition |
| **Measure** | **A** (accepts method for business use) | **R** | **R** technical extract | C | I | I / C |
| **Monitor** | **A** (domain huddle) | **R** operational | C | Oversight of registries | Summaries | C if personal-data issues |
| **Detect** | **A** remains | **R** log | May detect technically | Triage routing | — | — |
| **Remediate** | **A** residual | **R** coordinate | **R** technical | Coordinate cross-domain | Exception **A** if out of policy | C if privacy in the fix |
| **Verify** | **A** (close) | **R** verify | C | C | I | I / C |
| **Report** | **A** domain truth | **R** pack | C | DMC pack coordination | Receives summary | I / C |
| **Improve** | **A** rule/threshold/CDE confirmation updates | **R** proposals | C | Method improvement | Policy-level **A** | C as needed |

Single **A** per decision type is unchanged: Owner for in-policy quality; **DMC** for governance exceptions; **PDPO** only for the separate sharing privacy review — not for quality close.

---

## 4. Improve feeds Identify/Define

Continuous improvement may:

- Confirm a watch-item as a CDE (still using the two-step method — **no auto-CDE**)
- Add a **representative** rule using the approved structure (not a large catalogue in this drop)
- Adjust Target / Warning / Breach — still labeled `[A]` until a live Owner decision exists
- Retire a rule that no longer tests a material risk

It may **not** add CDEs in this repository drop beyond the locked 13.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Nine-stage quality lifecycle; RACI application | Sections 2–3 |
| `[C]` | Role **names**; Data Quality domain **name** | Naming |
| `[NDMO verification required]` | Official NDMO quality-lifecycle procedure | Not claimed |
