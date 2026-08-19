# MDM KPIs

**Document ID:** RHC-DG-P12-009  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for Core MDM domains; DMO method `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 10 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 10 reused; no match-score KPIs; no MDM-specific retention KPIs.

**Phase:** 12 — KPIs and maturity  
**Does not decide:** Hub, engine, or numeric match thresholds

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **reuses Phase 10**.

Core MDM: Patient, Provider; Facility **lightweight supporting only**. Golden record remains **logical**.  
**Do not create match-algorithm KPIs.**  
**Do not create MDM-specific retention rules or periods.**

Deactivate ≠ dispose (Phase 11 boundary reused).

---

## 2. KPIs in this domain

| KPI ID | Role |
| --- | --- |
| DG-KPI-008 | Executive — Master Data Duplicate Resolution Rate (review-case outcomes) |
| DG-KPI-016 | Supporting — Master Entity Registry Occupancy (Patient / Provider required occupancy; Facility supporting-only not forced to the same bar) |

Owners when interpreted by entity: Patient Access & Experience Director (Patient); Medical Affairs Officer (Provider). Steward: **Business Data Steward**.

Duplicates remain issues under the existing DQ issue procedure path (Phase 10).

Target Status: **To be established after baseline measurement.**

---

## 3. Explicitly not KPIs

- Average match score  
- “Golden record completeness %” as a physical-hub metric  
- Unique-patient count as a vanity volume metric without quality/duplicate context  

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Duplicate resolution without scores | Section 2 |
| `[C]` | Reference and Master Data Management domain **name** | Context |
| `[NDMO verification required]` | Official NDMO MDM KPIs | Not claimed |
