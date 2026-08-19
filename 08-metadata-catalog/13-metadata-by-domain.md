# Metadata by Domain (Illustrative)

**Document ID:** RHC-DG-P8-013  
**Version:** 1.0  
**Status:** Implemented (illustrative only)  
**Owner:** Each domain Data Owner **A** for assets in that domain  
**Approver:** CDO `[B]` (this file as framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Eight domains; Steward column = Business Data Steward only.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Live inventory; extra asset types; named operational steward titles

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **applies** the catalog framework to all **eight** approved domains `[A]`.

Example assets and metadata are **fictional/illustrative** `[A]`. They are not a live Rafid inventory.

**Steward column uses only “Business Data Steward.”** Named operational titles (for example Head of HIM) are **not** used in this file.

Classification values are illustrative Rafid tiers `[A][B]`, not NDMO national tiers `[NDMO verification required]`.

---

## 2. How to read a domain block

Mandatory fields are shown in abbreviated form. System / Primary System follows the § rule in [`04-minimum-metadata-standard.md`](04-minimum-metadata-standard.md): primary context where one applies; not a demand for exactly one source.

Status values are internal trust statuses, not regulatory certification.

---

## 3. Domain 1 — Patient / Person Master Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Patient demographic dataset |
| Asset type | Dataset |
| Domain | Patient / Person Master Data |
| Data Owner | Patient Access & Experience Director |
| Data Steward | Business Data Steward |
| Classification | Restricted |
| Business Definition | Cluster person-master demographics used for registration and identity |
| System / Primary System | EMR / registration (authoritative context) |
| Status | Reviewed (illustrative) |
| Glossary | Patient |

---

## 4. Domain 2 — Clinical / Medical Records Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Encounter clinical dataset |
| Asset type | Dataset |
| Domain | Clinical / Medical Records Data |
| Data Owner | Chief Medical Officer (CMO) |
| Data Steward | Business Data Steward |
| Classification | Restricted |
| Business Definition | Structured encounter and diagnosis content of the medical record |
| System / Primary System | EMR clinical |
| Status | Registered (illustrative) |
| Glossary | Encounter, Diagnosis |

---

## 5. Domain 3 — Provider / Clinician Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Provider master entity |
| Asset type | Master Data Entity |
| Domain | Provider / Clinician Data |
| Data Owner | Medical Affairs Officer |
| Data Steward | Business Data Steward |
| Classification | Confidential |
| Business Definition | Practitioner identity and credentialing attributes used across facilities |
| System / Primary System | Credentialing system (authoritative context) |
| Status | Reviewed (illustrative) |
| Glossary | Provider |

---

## 6. Domain 4 — Financial / Billing & Claims Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Claims dataset |
| Asset type | Dataset |
| Domain | Financial / Billing & Claims Data |
| Data Owner | Chief Financial Officer (CFO) |
| Data Steward | Business Data Steward |
| Classification | Restricted |
| Business Definition | Claims prepared or submitted for reimbursement |
| System / Primary System | Billing / claims (authoritative context); contributing clinical codes may be listed as multiple contributors on derived extracts — still one primary context |
| Status | Registered (illustrative) |
| Glossary | Claim |

---

## 7. Domain 5 — HR / Workforce Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Workforce roster dataset |
| Asset type | Dataset |
| Domain | Human Resources / Workforce Data |
| Data Owner | HR Director |
| Data Steward | Business Data Steward |
| Classification | Confidential |
| Business Definition | Staff identity and roster attributes (not the clinician credentialing master) |
| System / Primary System | HRIS |
| Status | Registered (illustrative) |

---

## 8. Domain 6 — Supply Chain & Asset Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Item master entity |
| Asset type | Master Data Entity |
| Domain | Supply Chain & Asset Data |
| Data Owner | Supply Chain Director |
| Data Steward | Business Data Steward |
| Classification | Internal |
| Business Definition | Item codes used in inventory and procurement |
| System / Primary System | ERP / inventory |
| Status | Registered (illustrative) |

---

## 9. Domain 7 — Quality & Patient Safety Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Patient safety incident dataset |
| Asset type | Dataset |
| Domain | Quality & Patient Safety Data |
| Data Owner | Chief Quality & Patient Safety Officer (CQPSO) |
| Data Steward | Business Data Steward |
| Classification | Restricted |
| Business Definition | Incident records used for safety learning (patient-linked as typical) |
| System / Primary System | Quality / incident system |
| Status | Registered (illustrative) |

---

## 10. Domain 8 — Reference / Organizational Master Data `[A]`

| Field | Illustrative value `[A]` |
| --- | --- |
| Example asset | Facility / department reference entity |
| Asset type | Master Data Entity |
| Domain | Reference / Organizational Master Data |
| Data Owner | Strategy & Planning Director |
| Data Steward | Business Data Steward |
| Classification | Internal |
| Business Definition | Organizational facility and department codes (single source of truth **principle**; Phase 10 architecture not built) |
| System / Primary System | Org reference / planning lists |
| Status | Reviewed (illustrative) |
| Glossary | Facility, Department |

DMO is **not** the Data Owner. The Steward role sits in DMO for this domain in Phase 4; this file still labels the role **Business Data Steward** only.

---

## 11. Coverage

All eight domains are represented. Examples remain `[A]`.

---

## 12. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative assets and field values | Sections 3–10 |
| `[B]` | Same metadata standard in every domain | Method |
| `[C]` | Role **names** | Context |
| `[NDMO verification required]` | National classification names for these examples | Not applied |
