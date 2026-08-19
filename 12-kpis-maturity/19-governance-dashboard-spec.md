# Governance Dashboard Specification

**Document ID:** RHC-DG-P12-019  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (specification); CDO oversight  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual views only; no software.

**Phase:** 12 — KPIs and maturity  
**Does not decide:** Tool vendor, cloud BI, refresh pipelines, UX

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document is a **conceptual dashboard specification** `[A]`.

**Not software. Not Power BI / Tableau / Looker / Purview. Not a data pipeline.**

It is `[A]` Proposed Rafid governance artifact (see [26](26-governance-artifacts.md)). **Not** NDMO-mandated.

---

## 2. Views (conceptual)

| View | Audience | Content |
| --- | --- | --- |
| **Executive** | DMC (quarterly) | DG-KPI-001–012 as status tiles **when evidenced**; narrative for not-evidenced; exception count; Critical aging theme |
| **Management** | CDO / DMO | Executive set plus DG-KPI-013–020; evidence pointers |
| **Domain** | Data Owner + Business Data Steward | Domain filter for quality, catalog, issues, classification; eight Owner titles only |
| **Operational** | Custodian / Steward | Issue lists; duplicate review queue; metadata gaps |

No view publishes a **cluster-wide quality index**. No view treats backup jobs as retention.

---

## 3. Tile behaviour `[A][B]`

| State | Display |
| --- | --- |
| Evidenced | Value + period + source (when a live process exists — **not claimed in this drop**) |
| Not evidenced | Explicit **Not evidenced** |
| Illustrative only | Label **`[A] Illustrative Rafid target`** if a teaching number is shown |

This repository **does not** populate tiles with fake Rafid percentages.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Four conceptual views | Section 2 |
| `[B]` | Status vs vanity dashboards | Section 3 |
| `[NDMO verification required]` | Official NDMO dashboard requirements | Not claimed |
