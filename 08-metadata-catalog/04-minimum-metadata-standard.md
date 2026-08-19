# Minimum Metadata Standard

**Document ID:** RHC-DG-P8-004  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (field method); Data Owner **A** for business field values  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Mandatory / Recommended / Capability-dependent; System/Primary System rule locked.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Physical database columns; NDMO official field list `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **minimum metadata model** for catalog assets `[A][B]`.

The model is **proportionate and implementable**. It is not a maximum enterprise schema. Specific NDMO metadata fields remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Three occupancy rules (locked)

| Occupancy | Meaning |
| --- | --- |
| **Mandatory** | Required to **publish** an operational catalog asset |
| **Recommended** | Expected for a healthy record; absence is a metadata-quality gap, not a block if Mandatory is complete (Steward still plans the fill) |
| **Capability-dependent** | Recorded when quality, operations, or lineage capability exists; do not invent fake values |

---

## 3. Mandatory fields (locked)

| Field | Intent |
| --- | --- |
| **Asset ID** | Stable Rafid identifier `[A]` (not an NDMO control ID) |
| **Asset Name** | Business-usable name |
| **Description** | Short what-it-is statement |
| **Domain** | One of the eight Phase 4 domains |
| **Data Owner** | Phase 4 Data Owner title |
| **Data Steward** | Role: **Business Data Steward** (title type; named operational titles are not required on the Year-1 record) |
| **Classification** | Rafid Public / Internal / Confidential / Restricted `[A][B]` — **not** NDMO national tiers |
| **Business Definition** | Owner-accepted meaning (Phase 6) |
| **System / Primary System** | Primary or authoritative **system context where one applies** — see §5 |
| **Status** | Certification/trust status ([`09-certification-trust-model.md`](09-certification-trust-model.md)) |
| **Created Date** | Date the catalog record was created (governance date, not a system SLA) |

These fields remain **mandatory**. Their occupancy is not reduced in the MVP.

---

## 4. Recommended fields `[A][B]`

Approved recommended complement (still proportionate):

| Field | Intent |
| --- | --- |
| **Asset type** | Dataset / Table / Report / Dashboard / Master Data Entity |
| **Last updated date** | When metadata last changed |
| **Last reviewed date** | When Owner/Steward last confirmed the record |
| **Glossary links** | Related business terms |
| **Tags / keywords** | Discovery aids (not a second classification scheme) |
| **Intended use / usage context** | Why the asset exists |
| **Contains personal data** | Yes / No / Uncertain — **indicator only**, not the personal data itself |
| **IT Data Steward / Custodian** | Technical contact **role**, not business Owner |
| **Related assets** | Other catalog assets |
| **Version** | Record version (governance, not software release) |

Recommended fields are **not** promoted to Mandatory in this phase.

---

## 5. System / Primary System (critical rule)

**System / Primary System is mandatory.**

It identifies the **primary or authoritative system context where one applies**.

It does **not** require exactly one source system.

| Asset nature `[A]` | Acceptable System / Primary System value |
| --- | --- |
| Sourced from one operational system | That system class (for example EMR / registration) |
| Derived, aggregated, or virtual | Multiple contributing systems **or** “none directly / derived” with contributing systems listed in recommended or capability-dependent fields |

Do **not** block registration because a report has several contributors. Do **not** drop the field.

Fine-grained technical lineage remains Phase 9.

---

## 6. Capability-dependent fields (locked)

| Field | When it applies |
| --- | --- |
| **Data format** | When a useful technical format is known |
| **Quality status** | When Phase 7 monitoring exists for linked CDEs/rules |
| **Relevant CDEs** | When confirmed CDEs apply (Phase 7 catalogue — not expanded here) |
| **Known issues** | When issues are logged on the Phase 6 quality issue path |
| **Upstream source** | When coarse lineage metadata is available |
| **Downstream consumers** | When known at governance level |
| **Transformation reference** | Conceptual pointer only — not a mapping engine |

Do not fabricate quality or lineage values to look complete.

---

## 7. What this file does not do

- Does not implement a catalog schema in a tool
- Does not require column-level metadata for publish
- Does not invent NDMO field IDs

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved occupancy model and field lists | Sections 2–6 |
| `[C]` | Data Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Official NDMO mandatory metadata fields | Not claimed |
