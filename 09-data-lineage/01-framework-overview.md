# Data Lineage Framework Overview

**Document ID:** RHC-DG-P9-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (methodology); domain **Data Owner** **A** for business lineage correctness  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 9 conceptual lineage framework.

**Phase:** 9 — Data lineage  
**Does not decide:** Tooling, automated capture, MDM, or live flow inventories

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved **lineage lifecycle** and why lineage exists in the fictional Rafid Health Cluster `[A]`.

It is governance operating design `[B]`. It is not a lineage product and not an NDMO compliance pack.

Lineage is **not** claimed to satisfy any specific regulatory or NDMO requirement. Specific NDMO lineage requirements remain `[NDMO verification required]`. **No compliance is claimed. No control IDs are invented.**

---

## 2. Locked lifecycle

```text
Identify lineage scope
→ Identify source
→ Identify movement
→ Identify transformation
→ Identify target
→ Identify consumer
→ Validate lineage
→ Approve lineage
→ Publish lineage
→ Maintain lineage
→ Review lineage
→ Retire lineage
```

| Stage | Intent | Who (Phase 4 pattern — not redesigned) |
| --- | --- | --- |
| **Identify lineage scope** | Decide which flow is in Year-1 / Critical Lineage candidate set | Steward **R**; Owner and DMO confirm (see criticality) |
| **Identify source** | Upstream asset or system context | Steward **R**; Custodian **C** |
| **Identify movement** | That data leaves the source toward another use | Steward **R**; Custodian **C** |
| **Identify transformation** | Conceptual change (join, code map, aggregate) — not ETL code | Steward **R**; Custodian **C** |
| **Identify target** | Downstream catalog asset | Steward **R** |
| **Identify consumer** | Report, interchange, process — not an access grant | Steward **R** |
| **Validate lineage** | Steward check against catalog and Owner meaning | Business Data Steward |
| **Approve lineage** | Owner **A** where business meaning of the flow is at stake | Data Owner |
| **Publish lineage** | Lineage metadata visible in catalog (Phase 8 fields) | Steward / DMO |
| **Maintain lineage** | Updates on approved change triggers | Steward **R** |
| **Review lineage** | Periodic confirmation | Steward **R**; Owner **A** for material change |
| **Retire lineage** | Flow no longer operational; record retained | Owner with DMO record-keeping |

No numeric SLA.

---

## 3. How lineage supports other capabilities `[A][B]`

| Capability | How lineage helps | What it does **not** do |
| --- | --- | --- |
| **Data Governance** | Makes movement visible and owned | Does not replace Policy |
| **Data Ownership** | Shows which Owner is upstream/downstream | Does not create a second Owner |
| **Data Classification** | Surfaces when a downstream asset may still hold sensitive elements | Does **not** classify; Phase 5 remains the method |
| **Data Quality** | Supports impact analysis of a source defect | Does not create a second quality framework |
| **Metadata & Catalog** | Fills Phase 8 Lineage Metadata | Does not replace the catalog |
| **Data Sharing** | Shows where data goes before a share is requested | Does not merge Owner business **A** and PDPO privacy **A** |
| **Master Data Management** | Flags master-data dependency as a criticality criterion | Does **not** start Phase 10 matching/survivorship |
| **Regulatory/audit traceability** | Provides a **governed description** of a flow for investigation | Does **not** claim a named regulation or NDMO specification is met `[NDMO verification required]` |

General audit usefulness `[B]` is **not** the same as a confirmed regulatory requirement `[NDMO verification required]`.

---

## 4. What this framework is not

- Not Purview, Collibra, Informatica, Atlan
- Not automated scanning or a graph database
- Not ETL implementation
- Not enterprise-wide column-level lineage
- Not Phase 10 MDM

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 9 lifecycle and support list | Sections 2–3 |
| `[C]` | Catalog / Quality / Classification domain **names** as already used in this repo | Context only |
| `[NDMO verification required]` | Specific NDMO or sector lineage mandates | Not claimed |
