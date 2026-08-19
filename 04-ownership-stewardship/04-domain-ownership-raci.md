# Domain Ownership RACI

**Document ID:** RHC-DG-P4-004  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

The ten-row decision RACI in [`03-ownership-decision-matrix.md`](03-ownership-decision-matrix.md) is **enterprise-standard**. It applies to **every** domain below. This file does not create a different Accountable model per hospital or per domain.

Titles `[A]` fill the Data Owner and Business Data Steward slots.

---

## 2. How to read a domain row

| Slot | Who fills it |
| --- | --- |
| **A / C as “DO”** | The domain’s Data Owner title |
| **R / C as “BDS”** | The domain’s Business Data Steward title |
| **CUST** | IT Data Steward / Custodian for the systems that hold the domain — never DO |
| **DMO** | Data Management Office — coordinator, not business Owner |
| **PDPO** | Personal Data Protection Officer — **A** only on sharing privacy review (row 7) |
| **DMC** | Data Management Committee — **A** only on access exception (row 5) |

---

## 3. Domain slot assignments `[A]`

| Domain | Fills DO | Fills BDS | IT is Owner? |
| --- | --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access | No |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | No |
| Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator | No |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager | No |
| Human Resources / Workforce Data | HR Director | HR Operations Manager | No |
| Supply Chain & Asset Data | Supply Chain Director | Inventory / Procurement Manager | No |
| Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) | Quality Improvement Manager | No |
| Reference / Organizational Master Data | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | No |

---

## 4. Consulted extras (not a second A) `[B]`

Where ownership was contested, the **alternative** title is **C** on relevant decisions — never a second **A**.

| Domain | Typical extra Consulted (not Owner) |
| --- | --- |
| Patient / Person Master | CMO (clinical-safety impact of identity rules) |
| Clinical / Medical Records | Patient Access & Experience Director (identity); CQPSO (indicator extracts) |
| Provider / Clinician | CMO (privilege implications); HR Director (employee join) |
| Financial / Billing & Claims | CMO / HIM (clinical documentation that drives charges); Patient Access |
| HR / Workforce | Medical Affairs Officer (practitioner-employee join) |
| Supply Chain & Asset | CFO (financial asset treatment) |
| Quality & Patient Safety | CMO (record-sourced indicators); Patient Access (identity) |
| Reference / Organizational Master | CIO as Custodian/consult for consuming systems |

---

## 5. Sharing rows (all domains)

When a share is requested:

1. **Data sharing — business approval** — domain **DO = A**, **BDS = R**, **PDPO = C/I**, **DMO = C**, **CUST = C/I**.
2. **Data sharing — privacy compliance review (personal data)** — **PDPO = A**, **DO = C**, **BDS = C**, **CUST = I**, **DMO = C**.

If the dataset is not personal data, row 7 is recorded as not applicable; row 6 still runs. PDPO remains **I** on row 6 when personal data is clearly absent.

These two rows stay **separate** for every domain.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Owner/Steward titles | Section 3 |
| `[B]` | One RACI, one A, consulted losers of contested ownership | Sections 4–5 |
| `[C]` | NDMO role names | Slot types |
| `[NDMO verification required]` | Control-level duties | Not used as IDs |
