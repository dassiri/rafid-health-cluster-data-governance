# Phase 11 — Data Lifecycle Management

**Document ID:** RHC-DG-P11-000  
**Phase:** 11 — Data lifecycle  
**Status:** Implemented  
**Does not decide:** Storage architecture, backup design, Records Management programme, archiving platform, database retention configuration, or KPIs/maturity (Phase 12)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## Status

**Implemented** — conceptual **Data Lifecycle Management** governance framework for the fictional Rafid Health Cluster `[A]`. No retention periods are invented. No legal or NDMO compliance is claimed.

This is **not** a storage architecture, backup solution, enterprise Records Management implementation, technical archiving platform, or database retention configuration.

---

## Purpose

Phase 11 defines **how data is governed from creation or acquisition through authorized use and sharing to retain, archive, and dispose** — without becoming a technology or records programme.

It consumes Phase 4 ownership, Phase 5 classification **method**, Phase 6 sharing and exception **procedures** (by title/path), Phase 7 quality **dimensions**, Phase 8 catalog **hierarchy**, Phase 9 conceptual **lineage**, and Phase 10 MDM **entity** lifecycle (kept distinct). It does **not** redesign those phases.

NDMO names Data Lifecycle Governance as a Data Governance control **theme** in the Phase 2 map `[C]` (`DG.6` as already recorded — plan review and communications). That **name** is not a verified retention/archive/disposal specification. Specific NDMO retention, archiving, disposal, and lifecycle requirements remain `[NDMO verification required]`. Healthcare-specific retention requirements remain `[Legal / regulatory verification required]`.

---

## Lifecycle framework (locked)

```text
Create / Acquire
→ Register
→ Classify
→ Store
→ Use
→ Share
→ Retain
→ Archive
→ Dispose / Destroy
```

Connects to: Data Governance, Ownership, Classification, Quality, Metadata & Catalog, Lineage, MDM, Access/Sharing, Privacy/Protection, Records Management (as a **distinct** discipline — **not** built here).

---

## Lifecycle principles `[A][B]`

Purpose-driven retention · Minimum necessary retention · Classification-aware handling · Owner accountability · Legal / regulatory hold · Controlled archival · Secure disposition · Traceability · Evidence of disposition · **No indefinite retention by default**

**Do not invent legal retention periods.**

---

## Lifecycle vs Records vs Backup

| Concept | Meaning |
| --- | --- |
| **Data Lifecycle Management** | Governs data from creation to disposition |
| **Records Management** | Governs records retained as evidence or business records — **referenced, not built** |
| **Backup / DR** | Recovery and continuity — **not** retention or archival |

**Archive ≠ Backup.**

---

## Ownership

Phase 4 reused: Data Owner **A** for lifecycle decisions in the domain; Business Data Steward maintains lifecycle metadata; DMO methodology and registries; Custodian implements approved technical mechanisms; PDPO privacy input where personal data is involved.

DMC: *Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework.* **No new DMC decision right.** Steward examples: **Business Data Steward** only.

---

## Classification integration

Rafid tiers Public / Internal / Confidential / Restricted `[A][B]` influence access, sharing, storage safeguards, transmission, monitoring, and disposal **handling**.

**Classification does NOT automatically determine retention duration.** Retention considers business need, legal/regulatory requirements, records requirements, contractual obligations where applicable, litigation/legal hold, and privacy. Specific retention requirements: `[NDMO verification required]` / `[Legal / regulatory verification required]`.

---

## Retention, hold, archive, disposal

Conceptual retention decision framework and Retention Schedule **structure** with **placeholder** periods — **no invented numbers**.

Legal/regulatory hold **overrides** normal disposal. Archive eligibility is conceptual. Disposal is authorized, evidenced, and closed. Disposal Record is `[A]` Proposed Rafid governance artifact.

---

## Domain application and MDM boundary

All eight Phase 4 domains. No invented retention periods. Phase 10 MDM entity lifecycle (match/merge/deactivate) remains **distinct** from this enterprise Create→Dispose chain. **No MDM-specific retention rules.**

---

## Integration, artifacts, exceptions, MVP

Quality / metadata / lineage / MDM / sharing reused, not redesigned. Sharing still two **A**s (Owner business; PDPO privacy).

Artifacts `[A]` Proposed Rafid governance artifacts — not NDMO-mandated. **No new Policy/Standard/Procedure stack.**

Exceptions: **Data Governance Exception Procedure** — `06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md` (title + path only).

**MVP:** Patient / Person Master; Clinical / Medical Records; Financial / Billing & Claims. No actual retention periods. No legal/regulatory compliance claim.

---

## NDMO verification limitations

Specific NDMO retention, archiving, disposal, and lifecycle requirements: `[NDMO verification required]`.  
Healthcare-specific retention: `[Legal / regulatory verification required]`.

---

## Boundary with Phase 12

Phase 12 (KPIs and maturity) lives in `12-kpis-maturity/`. This Phase 11 folder was **not** redesigned. Lifecycle KPIs (for example Retention Schedule Coverage) measure **rule occupancy**, not invented retention periods. **No live Rafid KPI values are claimed in Phase 11.**

---

## Files

| Path | ID |
| --- | --- |
| [01-lifecycle-framework.md](01-lifecycle-framework.md) | RHC-DG-P11-001 |
| [02-lifecycle-principles.md](02-lifecycle-principles.md) | RHC-DG-P11-002 |
| [03-lifecycle-vs-records-vs-backup.md](03-lifecycle-vs-records-vs-backup.md) | RHC-DG-P11-003 |
| [04-lifecycle-ownership.md](04-lifecycle-ownership.md) | RHC-DG-P11-004 |
| [05-lifecycle-and-classification.md](05-lifecycle-and-classification.md) | RHC-DG-P11-005 |
| [06-retention-governance.md](06-retention-governance.md) | RHC-DG-P11-006 |
| [07-retention-schedule.md](07-retention-schedule.md) | RHC-DG-P11-007 |
| [08-legal-regulatory-hold.md](08-legal-regulatory-hold.md) | RHC-DG-P11-008 |
| [09-archiving.md](09-archiving.md) | RHC-DG-P11-009 |
| [10-disposal-destruction.md](10-disposal-destruction.md) | RHC-DG-P11-010 |
| [11-disposal-evidence.md](11-disposal-evidence.md) | RHC-DG-P11-011 |
| [12-end-to-end-workflow.md](12-end-to-end-workflow.md) | RHC-DG-P11-012 |
| [13-lifecycle-by-domain.md](13-lifecycle-by-domain.md) | RHC-DG-P11-013 |
| [14-mdm-lifecycle-boundary.md](14-mdm-lifecycle-boundary.md) | RHC-DG-P11-014 |
| [15-lifecycle-and-quality.md](15-lifecycle-and-quality.md) | RHC-DG-P11-015 |
| [16-lifecycle-and-metadata.md](16-lifecycle-and-metadata.md) | RHC-DG-P11-016 |
| [17-lifecycle-and-lineage.md](17-lifecycle-and-lineage.md) | RHC-DG-P11-017 |
| [18-lifecycle-and-mdm.md](18-lifecycle-and-mdm.md) | RHC-DG-P11-018 |
| [19-lifecycle-and-sharing.md](19-lifecycle-and-sharing.md) | RHC-DG-P11-019 |
| [20-governance-artifacts.md](20-governance-artifacts.md) | RHC-DG-P11-020 |
| [21-retention-exceptions.md](21-retention-exceptions.md) | RHC-DG-P11-021 |
| [22-lifecycle-mvp.md](22-lifecycle-mvp.md) | RHC-DG-P11-022 |
| [23-interview-defensibility.md](23-interview-defensibility.md) | RHC-DG-P11-023 |
| [24-ndmo-alignment.md](24-ndmo-alignment.md) | RHC-DG-P11-024 |
