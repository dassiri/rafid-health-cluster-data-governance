# Business Glossary

**Document ID:** RHC-DG-P8-005  
**Version:** 1.0  
**Status:** Implemented (illustrative glossary only)  
**Owner:** Domain Data Owner **A** for terms in that domain; DMO owns glossary method `[B]`  
**Approver:** CDO `[B]` (structure as framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Locked term structure; seven illustrative terms `[A]`.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Full controlled vocabulary; Arabic official terms; NDMO glossary mandate `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **glossary structure**, its relationship to the catalog, and **seven illustrative terms** `[A]`.

Examples are fictional. They are not a live Rafid vocabulary and not NDMO-mandated terms.

---

## 2. Approved term structure (locked)

| Field | Intent |
| --- | --- |
| **Business Term** | Preferred cluster term |
| **Definition** | Owner-accepted meaning |
| **Owner** | Phase 4 Data Owner title for the owning domain |
| **Steward** | **Business Data Steward** (role type only in examples) |
| **Synonyms** | Other names in use |
| **Related Terms** | Other glossary entries |
| **Domain** | Phase 4 domain |
| **Status** | Draft / Approved / Retired (glossary status — not catalog certification) |
| **Approval** | Data Owner acceptance of the definition |
| **Change History** | Material definition changes |

This structure does not create a new Policy.

---

## 3. Glossary ↔ Catalog ↔ Assets `[B]`

```text
Business Glossary  ↔  Data Catalog  ↔  Data Assets
```

| Link | Meaning |
| --- | --- |
| Glossary → Catalog | A term may point to assets that use it |
| Catalog → Glossary | An asset’s business definition and glossary links point to terms |
| Catalog → Assets | The catalog **is** the governed list of assets; assets are the registered objects |

The glossary is **not** the catalog. The catalog is **not** the data. Definitions remain **Data Owner A** (Phase 4 row 1 and row 8).

---

## 4. Seven illustrative terms `[A]`

Steward column uses **only** “Business Data Steward”. Owner titles are Phase 4 exactly.

### Patient `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Patient |
| Definition | A person registered to receive care in the cluster, identified in the person master. |
| Owner | Patient Access & Experience Director |
| Steward | Business Data Steward |
| Synonyms | Person (when used for the same master identity) |
| Related Terms | Encounter, Provider |
| Domain | Patient / Person Master Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative — not a live signature) |
| Change History | v1.0 illustrative entry |

### Encounter `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Encounter |
| Definition | A defined care interaction or visit recorded in the clinical record context. |
| Owner | Chief Medical Officer (CMO) |
| Steward | Business Data Steward |
| Synonyms | Visit (informal) |
| Related Terms | Patient, Diagnosis, Provider |
| Domain | Clinical / Medical Records Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative) |
| Change History | v1.0 illustrative entry |

### Provider `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Provider |
| Definition | A clinician or practitioner identity used for care delivery and credentialing, distinct from the HR employee record. |
| Owner | Medical Affairs Officer |
| Steward | Business Data Steward |
| Synonyms | Clinician (in some operational speech) |
| Related Terms | Patient, Encounter |
| Domain | Provider / Clinician Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative) |
| Change History | v1.0 illustrative entry |

### Claim `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Claim |
| Definition | A billing/claims record submitted or prepared for reimbursement of services. |
| Owner | Chief Financial Officer (CFO) |
| Steward | Business Data Steward |
| Synonyms | Bill (informal; not always equivalent) |
| Related Terms | Encounter, Diagnosis |
| Domain | Financial / Billing & Claims Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative) |
| Change History | v1.0 illustrative entry |

### Facility `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Facility |
| Definition | An organizational location in the cluster reference structure (hospital or other delivery site as used in org master). |
| Owner | Strategy & Planning Director |
| Steward | Business Data Steward |
| Synonyms | Site, hospital (informal) |
| Related Terms | Department |
| Domain | Reference / Organizational Master Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative) |
| Change History | v1.0 illustrative entry |

### Department `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Department |
| Definition | An organizational unit within a facility (or cluster structure) as represented in organizational reference data. |
| Owner | Strategy & Planning Director |
| Steward | Business Data Steward |
| Synonyms | Unit, ward (informal; not always equivalent) |
| Related Terms | Facility |
| Domain | Reference / Organizational Master Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative) |
| Change History | v1.0 illustrative entry |

### Diagnosis `[A]`

| Field | Value `[A]` |
| --- | --- |
| Business Term | Diagnosis |
| Definition | A recorded clinical diagnosis (coded or structured) in the medical record context. |
| Owner | Chief Medical Officer (CMO) |
| Steward | Business Data Steward |
| Synonyms | Problem (not always equivalent) |
| Related Terms | Encounter, Claim |
| Domain | Clinical / Medical Records Data |
| Status | Approved (illustrative) |
| Approval | Data Owner (illustrative) |
| Change History | v1.0 illustrative entry |

**Count:** seven terms. No additional official glossary terms in this drop.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Seven illustrative terms; example definitions | Section 4 |
| `[B]` | Glossary structure; glossary ≠ catalog | Sections 2–3 |
| `[C]` | Data Catalog and Metadata domain **name**; BDE/BDS **names** | Context |
| `[NDMO verification required]` | Official NDMO glossary field mandates | Not claimed |
