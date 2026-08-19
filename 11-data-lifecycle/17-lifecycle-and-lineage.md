# Data Lifecycle and Lineage

**Document ID:** RHC-DG-P11-017  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for impact in the domain; DMO lineage method `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 9 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 9 conceptual lineage reused; no technical lineage.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Automated lineage, column-level graphs, or ETL

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **reuses Phase 9 conceptual / business lineage**.

**Do NOT create technical lineage.**  
Phase 9 is **not** redesigned. Classification still does **not** automatically inherit the highest downstream tier (Phase 9 lock).

---

## 2. Impact chain (locked) `[A][B]`

```text
Lifecycle change
→ lineage impact
→ affected downstream assets
→ owner review where necessary
```

| Example lifecycle change | Lineage concern |
| --- | --- |
| **Source retirement** | Downstream reports/dashboards lose a source; Owner of downstream domain reviews fitness |
| **System migration** | Mapping of retained/archived copies; Critical Lineage paths in Phase 9 remain conceptual |
| **Asset archival** | Active processes must not silently depend on archive as operational feed |
| **Asset disposal** | Confirm no required downstream use; hold check still applies |

Business Data Steward traces coarse upstream/downstream using Phase 8 Lineage Metadata and Phase 9 records. Data Owner **A** for the change in the source domain; consulted Owners where downstream impact is material.

Illustrative E2E flow in Phase 9 remains **illustrative** — not real MOH/NPHIES/Rafid architecture.

---

## 3. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Change → impact → review | Section 2 |
| `[C]` | Lineage-related domain **names** already in Phase 9 | Context |
| `[NDMO verification required]` | Official NDMO lineage-on-disposal specs | Not claimed |
