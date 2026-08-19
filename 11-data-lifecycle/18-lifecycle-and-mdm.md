# Data Lifecycle and Master Data

**Document ID:** RHC-DG-P11-018  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for the master domain; DMO MDM + lifecycle methods `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 10 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Deactivation impact vs enterprise retention; no MDM-specific retention rules.

**Phase:** 11 — Data lifecycle  
**Does not decide:** New Core MDM entities or match rules

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document **reuses Phase 10**.

**Do NOT create MDM-specific retention rules.**  
**Do NOT redesign Phase 10.**

Boundary detail: [14-mdm-lifecycle-boundary.md](14-mdm-lifecycle-boundary.md)

---

## 2. Interaction chain (locked) `[A][B]`

```text
Master entity deactivation
→ downstream impact review
→ lifecycle treatment of related data
→ retention/disposition according to applicable rules
```

| Step | Meaning |
| --- | --- |
| Master entity deactivation | Phase 10: identity no longer active (Owner **A**; Business Data Steward **R**) |
| Downstream impact review | Phase 9 conceptual lineage — clinical, financial, quality uses of that identity |
| Lifecycle treatment of related data | Encounter, claim, and other **related** assets follow **their** Retention Rules — not a hidden MDM clock |
| Retention/disposition according to applicable rules | Same Phase 11 schedule, hold, archive, and disposal governance. Periods remain `[Legal / regulatory verification required]` / `[NDMO verification required]` until verified |

Logical golden record (Phase 10) is **not** an archive store and **not** a backup.

Facility remains **lightweight supporting only** in MVP. HR/Finance/Quality remain Non-MDM at that maturity. Supply Chain/Item remains **reference data**. None of those cuts invent a retention number.

---

## 3. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Deactivate → impact → enterprise rules | Section 2 |
| `[C]` | Reference and Master Data Management domain **name** | Context |
| `[NDMO verification required]` | Official NDMO master-data retention specs | Not claimed |
| `[Legal / regulatory verification required]` | Healthcare identity/record clocks | Not invented |
