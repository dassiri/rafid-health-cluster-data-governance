# NDMO Alignment (Ownership and Stewardship)

**Document ID:** RHC-DG-P4-008  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented (alignment notes only)  
**Does not claim:** Implementation, audit evidence, or specification completion

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

Phase 4 alignment is **domain-level only** where it is defensible. It maps Rafid ownership groupings to NDMO **knowledge-domain names** and **role names**.

**Not used in this file:** unverified specification-level control IDs.

---

## 2. Role-name alignment `[C]`

| Rafid working title `[B]` / `[A]` | NDMO name `[C]` | This phase |
| --- | --- | --- |
| Data Owner | Business Data Executive | Eight titles assigned to eight domains |
| Business Data Steward | Business Data Steward | Eight steward titles assigned |
| Data Custodian | IT Data Steward | Technical only; never business Owner |
| DMO | Data Management Office | Coordinates; not business Owner |
| Data Management Committee | Entity Data Management Committee | Approves Owner changes; Year-1 composition `[A]` |

Exact job-content alignment to NDMO’s Organizational Manual is `[NDMO verification required]`.

---

## 3. Knowledge-domain alignment (names only) `[C]`

Official NDMO knowledge-domain **names** (Standards v1.5, Section 6) that **touch** these ownership domains — not an implementation register:

| Rafid ownership domain `[A]` | Defensible NDMO name contact `[C]` | Limit |
| --- | --- | --- |
| Patient / Person Master Data | Reference and Master Data Management; Personal Data Protection | Identity master is personal data-heavy; MDM **name** only |
| Clinical / Medical Records Data | Personal Data Protection; Document and Content Management (records as content) | Clinical content is personal/health data; no procedure designed |
| Provider / Clinician Data | Reference and Master Data Management; Personal Data Protection | Practitioner master; personal data possible |
| Financial / Billing & Claims Data | Data Quality (fitness for billing/reporting) as a later quality workstream | Not a finance-specific NDMO domain name |
| Human Resources / Workforce Data | Personal Data Protection | Workforce personal data |
| Supply Chain & Asset Data | Reference and Master Data Management (item/vendor/asset masters) | Name contact only |
| Quality & Patient Safety Data | Data Quality (as a knowledge domain) **and** often personal data if patient-linked | Quality **framework** is Phase 7, not this file |
| Reference / Organizational Master Data | Reference and Master Data Management | Closest name match; not “implemented MDM” |

**Data Classification** as an NDMO knowledge domain `[C]` is relevant to **who** approves classification application (Owner **A**). Applying levels is **Phase 5** — Designed / Documented; operational implementation and measured performance are not claimed.

**Data Governance** as an NDMO knowledge domain `[C]` is the home of organization/role **names**. Phase 4 does not treat ownership assignment as a completed governance-domain implementation.

---

## 4. What remains `[NDMO verification required]`

- Specification-level organization, stewardship, and MDM requirements
- Whether NDMO requires a particular executive title (CMO vs Medical Affairs vs other) for health data
- Sharing-regulation steps beyond the Standards’ statement that Business Data Executive approval appears in the sharing process `[C]`
- PDPO versus PDPL DPO
- Any control ID crosswalk of the `[B]` registries in [`07-ownership-governance-controls.md`](07-ownership-governance-controls.md)

---

## 5. Statements that are not made

- Rafid is not NDMO-compliant by virtue of this mapping.
- The eight domains are not official NDMO domain IDs.
- DMO hosting the Reference Data steward is not NDMO “DMO owns master data.”

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5 — 15 domain **names**; BDE/BDS/IT steward/DMO/DMC **names**; BDE in sharing process as stated | Sections 2–3 |
| `[A]` / `[B]` | Approved Rafid ownership model | What is being mapped |
| `[NDMO verification required]` | Organizational Manual; specification IDs; PDPL; sharing regulation | Section 4 |
