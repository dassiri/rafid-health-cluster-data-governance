# Data Lifecycle Framework

**Document ID:** RHC-DG-P11-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (methodology); domain **Data Owner** **A** for lifecycle decisions  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Enterprise Create→Dispose chain; no invented retention periods.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Storage, backup, records programme, or verified legal periods

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records the **enterprise data lifecycle** for the fictional Rafid Health Cluster `[A]`.

It is governance operating design `[B]`. It is not a platform. Specific NDMO retention, archiving, disposal, or lifecycle requirements are **not** claimed as mandated `[NDMO verification required]`. Healthcare retention law is `[Legal / regulatory verification required]`. **No compliance is claimed.**

---

## 2. Locked lifecycle

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

| Stage | Intent (conceptual) |
| --- | --- |
| **Create / Acquire** | Data comes into existence or is received |
| **Register** | Catalog / metadata registration (Phase 8 / Metadata Registration Procedure) |
| **Classify** | Rafid tier (Phase 5) — Owner **A** |
| **Store** | Held under approved handling — **not** a storage architecture |
| **Use** | Operational and analytic use within authorization |
| **Share** | Two Phase 4 decisions (Owner business **A**; PDPO privacy **A** where personal data) |
| **Retain** | Keep according to an Owner-approved **rule** whose **period is verified**, not invented |
| **Archive** | Reduced active use while still retained — **not** backup |
| **Dispose / Destroy** | Authorized, evidenced removal when eligible and not on hold |

---

## 3. How lifecycle connects `[A][B]`

| Capability | Connection | Not this phase |
| --- | --- | --- |
| **Data Governance** | Lifecycle is a governed process with registers | Not a new Policy stack |
| **Data Ownership** | Owner **A** for domain lifecycle decisions (Phase 4) | No new Owner titles |
| **Data Classification** | Handling influenced by tier (Phase 5) | Tier does **not** auto-set duration |
| **Data Quality** | Lifecycle events affect fitness (Phase 7) | No second DQ framework |
| **Metadata & Catalog** | Lifecycle metadata on assets (Phase 8) | Hierarchy not redesigned |
| **Data Lineage** | Retirement/archive/disposal has downstream impact (Phase 9) | No technical lineage |
| **Master Data Management** | Entity deactivate vs enterprise dispose (Phase 10) | No MDM-specific retention rules |
| **Data Access / Sharing** | Share only if authorized; recipient copies may have retention obligations | No invented contracts |
| **Privacy / Protection** | PDPO input where personal data; NCA remains security domain `[C]` | No NCA control catalogue |
| **Records Management** | Distinct discipline for evidential records | **Not built** as a separate framework |

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved nine-stage chain | Sections 2–3 |
| `[C]` | Guiding principle **names**; NCA mandate for security domain **name** | Context |
| `[NDMO verification required]` | Specific NDMO lifecycle/retention/archive/disposal specifications | Not claimed |
| `[Legal / regulatory verification required]` | Healthcare retention law | Not invented |
