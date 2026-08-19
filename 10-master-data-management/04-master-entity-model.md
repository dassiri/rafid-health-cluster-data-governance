# Master Entity Model

**Document ID:** RHC-DG-P10-004  
**Version:** 1.0  
**Status:** Implemented (illustrative entity model)  
**Owner:** Each Core MDM Data Owner **A** for that entity  
**Approver:** CDO `[B]` (model as framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Three core entities; Phase 8 hierarchy reused; classification examples labeled.

**Phase:** 10 — Master data management  
**Does not decide:** Physical schema; Phase 5 standing rules for masters

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records a **conceptual** MDM entity model for the three Core MDM entities.

It **reuses the Phase 8 hierarchy exactly**:

```text
Data Domain → Data Asset → Data Structure / Object → Data Element
```

It does **not** create a parallel metadata hierarchy.

---

## 2. Classification examples — mandatory clarification

Illustrative classifications below are:

**`[A]` Illustrative Phase 5 classification examples**

Approved examples for teaching:

| Entity | Illustrative Rafid tier `[A]` |
| --- | --- |
| Patient / Person | Restricted |
| Provider / Clinician | Confidential |
| Facility / Organization | Internal |

**These examples do NOT create automatic or standing classification rules for master entities generally.** The actual classification decision for any specific master entity, dataset, or attribute remains governed by the **Phase 5 Data Classification Framework** and **approved by the Data Owner**. Phase 5 is **not** redesigned. Rafid tiers are not NDMO national tiers `[NDMO verification required]`.

---

## 3. Patient / Person `[A]`

| Element | Content |
| --- | --- |
| **Entity** | Patient / Person |
| **Business definition** | A person registered to receive care, as the cluster identity master (glossary term **Patient**) |
| **Business identifier** | Patient identifier (MRN) plus National ID where applicable (Phase 7 CDE-001, CDE-002) |
| **Source systems** | EMR / registration / MPI class `[A]` — not a named vendor |
| **Golden/master representation** | Logical trusted person identity ([`05-golden-record.md`](05-golden-record.md)) |
| **Owner** | Patient Access & Experience Director |
| **Steward** | Business Data Steward |
| **Classification** | `[A]` Illustrative Phase 5 classification example: **Restricted** — not a standing rule |
| **Key attributes** | Identifiers, name, date of birth, contact (contact remains a quality watch-item, not a 14th CDE) |
| **Relationships** | Linked to Encounter (transaction); Provider (other master); Facility (supporting master) |
| **Quality rules** | Uniqueness/completeness of National ID and MRN (DQ-001, DQ-003) — Phase 7 reused |
| **Lifecycle** | [`13-master-data-lifecycle.md`](13-master-data-lifecycle.md) |

Catalog placement: Domain = Patient / Person Master Data → Asset type **Master Data Entity**.

---

## 4. Provider / Clinician `[A]`

| Element | Content |
| --- | --- |
| **Entity** | Provider / Clinician |
| **Business definition** | Practitioner identity used for care delivery and credentialing, distinct from the HR employee record (glossary **Provider**) |
| **Business identifier** | Provider identifier (CDE-005); credential/licence attributes (CDE-006) |
| **Source systems** | Credentialing system / EMR provider master class `[A]` |
| **Golden/master representation** | Logical trusted provider identity |
| **Owner** | Medical Affairs Officer |
| **Steward** | Business Data Steward |
| **Classification** | `[A]` Illustrative Phase 5 classification example: **Confidential** — not a standing rule |
| **Key attributes** | Provider ID, name, licence/expiry, specialty (illustrative) |
| **Relationships** | Linked to Encounter (transaction); may join HR employee ID (HR remains Non-MDM) |
| **Quality rules** | Provider ID uniqueness/consistency; credential expiry timeliness (DQ-004) |
| **Lifecycle** | [`13-master-data-lifecycle.md`](13-master-data-lifecycle.md) |

---

## 5. Facility / Organization `[A]`

| Element | Content |
| --- | --- |
| **Entity** | Facility / Organization |
| **Business definition** | Organizational location/unit as used in org reference (glossary **Facility**, **Department**) |
| **Business identifier** | Facility / department code (CDE-013) |
| **Source systems** | Org reference / planning lists `[A]` |
| **Golden/master representation** | **Not** a full golden-record program in MVP — lightweight trusted **codes** ([`16-mdm-mvp.md`](16-mdm-mvp.md)) |
| **Owner** | Strategy & Planning Director |
| **Steward** | Business Data Steward |
| **Classification** | `[A]` Illustrative Phase 5 classification example: **Internal** — not a standing rule |
| **Key attributes** | Facility code, name, location (illustrative) |
| **Relationships** | Context for Patient and Provider activity; Domain 8 reference structures |
| **Quality rules** | Integrity of facility/department codes (DQ-008) |
| **Lifecycle** | Code create/deactivate; **no** separate Facility matching engine |

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative attributes, systems, classification examples | Sections 2–5 |
| `[B]` | Conceptual entity model | Structure |
| `[C]` | Role **names** | Naming |
| `[NDMO verification required]` | Official NDMO master-entity schemas | Not claimed |
