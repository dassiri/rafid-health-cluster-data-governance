# Catalog MVP

**Document ID:** RHC-DG-P8-014  
**Version:** 1.0  
**Status:** Implemented (MVP design only — not a live catalog)  
**Owner:** CDO / DMO (programme) `[B]`; domain Data Owners **A** for MVP content in scope  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Three-domain MVP; qualitative success only.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Tool purchase; numeric coverage targets; expansion to all eight domains in Year-1 MVP

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the **approved catalog MVP** `[A][B]`.

The MVP is a **scope and operating choice**, not a platform implementation. Success indicators are **qualitative**. **Do not invent numeric targets.**

---

## 2. Scope (locked)

**Domains (only these three):**

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Financial / Billing & Claims Data  

The other five domains remain in the **framework** ([`13-metadata-by-domain.md`](13-metadata-by-domain.md)) but are **outside MVP operating scope**.

**Data Owners in MVP (Phase 4 titles):**

| Domain | Data Owner |
| --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) |

Steward: **Business Data Steward** only (role type).

---

## 3. Initial asset types (locked)

- Dataset  
- Master Data Entity  

Table, Report, and Dashboard remain Year-1 **types in the model** but are **not** required in the MVP operating cut. API and Data Product remain deferred.

---

## 4. Initial users (locked)

- Data Owners  
- Business Data Stewards  
- DMO  

Executive, Analyst, Data Scientist, and IT/Custodian personas exist in the conceptual catalog but are **not** the MVP operating user set.

---

## 5. Minimum metadata (locked)

MVP uses the **approved mandatory fields** (not a reduced set):

Asset ID · Asset Name · Description · Domain · Data Owner · Data Steward · Classification · Business Definition · System / Primary System · Status · Created Date

System / Primary System remains mandatory with the “not exactly one source system” rule.

Recommended and capability-dependent fields may be filled when known; they are not faked for MVP completeness theatre.

---

## 6. Governance workflow (locked)

The **full** registration workflow applies to MVP scope:

Identify → Submit metadata → Steward validation → Owner approval where required → DMO governance check → Publish → Maintain

Procedure (unchanged):

**Metadata Registration Procedure** — `06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`

---

## 7. Qualitative success indicators `[A][B]`

Success is described **without numbers**:

- MVP-scope operational assets can be identified and registered
- Mandatory metadata is present before publish
- Classification is linked (unlabeled is not Public)
- Owner and Business Data Steward are visible
- DMO can perform a governance check without rewriting meaning
- Users in the MVP set can discover **metadata**, not Restricted/Confidential **data**
- No catalog product is required to declare the MVP **design** complete

Do **not** add “80% of datasets catalogued” or similar targets (Phase 12 is not this file).

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved MVP cut | Sections 2–7 |
| `[C]` | Catalog domain **name** | Context |
| `[NDMO verification required]` | Official NDMO catalog rollout metrics | Not claimed |
