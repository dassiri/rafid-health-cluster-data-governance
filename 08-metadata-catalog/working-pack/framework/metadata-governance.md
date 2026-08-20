# Metadata Governance (Working Pack)

**Document ID:** RHC-DG-P8-WP-003  
**Version:** 1.0  
**Status:** Implemented (working design only)  
**Owner:** DMO `[B]` (method); Data Owner **A** for domain metadata content  
**Parent design:** [`../../12-metadata-ownership.md`](../../12-metadata-ownership.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This file applies **existing** Phase 3–4 roles to metadata decisions. It does **not** create new roles, a new RACI, or a new Data Management Committee decision class.

Role types: [`../../../03-operating-model/03-role-catalogue.md`](../../../03-operating-model/03-role-catalogue.md)  
Domain titles: [`../../../04-ownership-stewardship/01-domain-ownership-detail.md`](../../../04-ownership-stewardship/01-domain-ownership-detail.md)  
Decision rows used: definition (row 1), classification (row 3), catalog content (row 8).

NDMO names: Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office, Entity Data Management Committee `[C]`. Specification-level duties remain `[NDMO verification required]`.

---

## 2. Roles and metadata duties

### 2.1 Data Owner (Business Data Executive)

Phase 4 titles (unchanged): Patient Access & Experience Director; Chief Medical Officer (CMO); Medical Affairs Officer; Chief Financial Officer (CFO); HR Director; Supply Chain Director; Chief Quality & Patient Safety Officer (CQPSO); Strategy & Planning Director.

| Area | Duty |
| --- | --- |
| **Responsibilities** | Accept business definitions; accept classification of domain datasets; accept catalog content; appoint / support the Business Data Steward; accept **Certified** trust status |
| **Metadata decisions** | Meaning of the asset; whether the description is trustworthy for discovery |
| **Approval** | Business definition; classification value; catalog content; Certified status |
| **Review** | Material change to definition, classification, Owner, or CDE confirmation |

The Owner does **not** run the catalog programme. IT is **not** the Data Owner.

### 2.2 Business Data Steward

Phase 4 appointed titles (working pack records these titles): Head of Patient Registration & Access; Head of Health Information Management (HIM); Credentialing Coordinator; Revenue Cycle Manager; HR Operations Manager; Inventory / Procurement Manager; Quality Improvement Manager; Enterprise Data / PMO Analyst within DMO.

Phase 8 catalog operating design also allows the **role type** “Business Data Steward” on a Year-1 record. Both are the same seat.

| Area | Duty |
| --- | --- |
| **Responsibilities** | Identify assets; draft definitions; complete minimum metadata; maintain the record; validate completeness; keep glossary links current |
| **Metadata decisions** | Operational completeness; whether mandatory fields are ready for Owner/DMO review |
| **Approval** | Registered and Reviewed trust statuses; cannot approve meaning without the Owner |
| **Review** | Periodic metadata review; raise gaps to the Owner |

DMO **hosts** the Steward for Reference / Organizational Master Data. DMO is **not** that domain’s Data Owner.

### 2.3 Data Management Office / DMO

| Area | Duty |
| --- | --- |
| **Responsibilities** | Metadata method; catalog programme oversight; registration governance check; Steward Registry; certification register method |
| **Metadata decisions** | Whether the **record is complete as a governed object** (domain, Owner, classification present). DMO cannot rewrite clinical or finance meaning |
| **Approval** | Governance check before publish; not content ownership |
| **Review** | Cross-domain consistency; exception routing via the existing Data Governance Exception Procedure |

CDO remains accountable for the catalog **programme**.

### 2.4 IT / Data Custodian (IT Data Steward)

| Area | Duty |
| --- | --- |
| **Responsibilities** | Supply technical metadata (system, schema, table, type) where known; apply system changes after a business decision |
| **Metadata decisions** | Technical accuracy of system/structure fields |
| **Approval** | None for business meaning or classification |
| **Review** | Technical metadata when the system changes |

Custodian is **Consulted**. Custodian is never **A** for definition, classification, or catalog content.

### 2.5 Data Management Committee (Entity Data Management Committee)

| Area | Duty |
| --- | --- |
| **Responsibilities** | Strategy; L3 policy; material exceptions; residual sharing risk; Owner non-participation |
| **Metadata decisions** | **None** at asset level. No new “catalog appeal” class |
| **Approval** | Policy-level exceptions only, using the existing exception procedure (**DMC = A**) |
| **Review** | Escalated themes (coverage, Owner non-participation), not every catalog page |

DMC does **not** approve each asset. DMC does **not** become catalog content Owner.

### 2.6 Governance forums (existing set — not a new role)

| Forum | Metadata use |
| --- | --- |
| **Data Management Committee** | Escalation and policy exceptions only |
| **Steward Forum** (monthly) | Cross-domain catalog practice; clash detection; standard **proposals** |
| **Domain huddle** | In-domain definition, classification pack, catalog entry, issue closure |
| **DMO operations huddle** | Intake routing only — not a board |

There is no per-hospital governance board.

---

## 3. Decision snapshot

| Decision | A | R | C |
| --- | --- | --- | --- |
| Business definition | Data Owner | Business Data Steward | PDPO if personal/health-identifying |
| Classification value | Data Owner | Business Data Steward | PDPO when personal |
| Minimum metadata completeness | — | Business Data Steward | Custodian (technical fields); DMO (method) |
| Catalog content publish | Data Owner (content) | Steward | DMO (governance check) |
| Certified trust status | Data Owner | Steward | DMO (register) |
| Catalog programme / method | CDO / DMO | DMO | Owners, Stewards |
| Policy exception to publish without Owner-accepted definition | DMC | DMO | Owner, CDO |

---

## 4. What this file does not do

- Does not add a metadata-specific Council
- Does not make DMO the Owner of Patient, Clinical, or Finance data
- Does not assign IT as Data Owner
