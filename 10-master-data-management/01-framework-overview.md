# MDM Framework Overview

**Document ID:** RHC-DG-P10-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (methodology); domain **Data Owner** **A** for master meaning  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual MDM framework; no platform.

**Phase:** 10 — Master data management  
**Does not decide:** Vendor, hub, matching engine, Phase 11 retention

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the approved **MDM lifecycle** for the fictional Rafid Health Cluster `[A]`.

It is governance operating design `[B]`. It is not an MDM product. Reference and Master Data Management is an NDMO knowledge-domain **name** `[C]`. Specific NDMO MDM requirements remain `[NDMO verification required]`. **No compliance is claimed. MDM is not briefed as NDMO-mandated unless verified.**

Parent Standard (not redesigned): **Master Data Management Standard** — `06-policies-standards-procedures/standards/05-master-data-management-standard.md`

---

## 2. Locked lifecycle

```text
Identify master domain
→ Define master entity
→ Assign ownership
→ Define business rules
→ Identify source systems
→ Define matching requirements
→ Define survivorship principles
→ Create / reconcile master record
→ Distribute trusted representation
→ Monitor quality
→ Resolve conflicts
→ Maintain
→ Retire
```

| Stage | Who (Phase 4 — not redesigned) |
| --- | --- |
| Identify domain / define entity / assign ownership | Data Owner **A**; Steward **R**; DMO method |
| Business rules, matching requirements, survivorship principles | Owner **A**; Steward **R**; Custodian **C** |
| Create / reconcile / distribute | Steward **R**; Custodian implements in **existing** systems |
| Monitor quality | Phase 7 path; uniqueness/consistency emphasized for masters |
| Resolve conflicts | Owner **A**; DMO coordinates cross-domain; DMC only under **existing** Phase 3 authority |
| Maintain / retire | Owner **A** for business meaning; DMO registry |

No numeric SLA. No new Phase 6 procedure.

---

## 3. How MDM supports other capabilities `[A][B]`

| Capability | How MDM helps | What it does **not** do |
| --- | --- | --- |
| **Data Governance** | Shared identities have Owner, rules, and a register | Does not replace POL-001 |
| **Data Ownership** | One Owner per master domain (Phase 4) | Does not create a second **A** |
| **Data Quality** | Uniqueness/consistency of shared entities | Does not create a second DQ framework |
| **Metadata & Catalog** | Master Data Entity remains a Year-1 catalog type | Does not replace the catalog |
| **Data Lineage** | Master change prompts lineage impact (Phase 9) | Does not redesign lineage |
| **Data Classification** | Master datasets still classified under Phase 5 | Does not auto-classify masters |
| **Data Sharing** | Identity clarity before a share | Does not merge Owner **A** and PDPO **A** |
| **Reporting / Analytics** | Stable keys for KPIs (e.g. claim rejection example in Phase 9) | Does not invent numeric KPI targets |

---

## 4. What this framework is not

- Not SAP MDG, Informatica MDM, Reltio, Semarchy  
- Not a matching engine, MDM database, API, ETL, or ML matcher  
- Not Phase 11 enterprise lifecycle  
- Not NDMO specification completion  

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved lifecycle and support list | Sections 2–3 |
| `[C]` | Reference and Master Data Management domain **name** | Context |
| `[NDMO verification required]` | Specification-level MDM mandates | Not claimed |
