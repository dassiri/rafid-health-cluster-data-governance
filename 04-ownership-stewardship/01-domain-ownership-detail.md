# Domain Ownership Detail

**Document ID:** RHC-DG-P4-001  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented  
**Does not decide:** Dataset classification, system-of-record technology, or named incumbents

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved Owner and Steward for each of the eight enterprise data domains in the fictional Rafid Health Cluster `[A]`.

**Principles (approved)** `[B]`

- Exactly one accountable Data Owner per domain.
- Ownership is enterprise-wide across the cluster, not hospital-by-hospital.
- Business Data Stewards execute day-to-day governance.
- IT Data Stewards / Custodians perform technical implementation and are **not** business Data Owners.
- The DMO coordinates the framework and does **not** become the operational Data Owner of a business domain.
- Shared ownership is not used. Where ownership was contested, one Accountable Owner was selected; the alternative role remains **Consulted**.

NDMO names the Owner as Business Data Executive and the steward as Business Data Steward `[C]`. Exact specification-level duties are `[NDMO verification required]`.

---

## 2. Domain 1 — Patient / Person Master Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Patient Access & Experience Director `[A]` |
| **Business Data Steward** | Head of Patient Registration & Access `[A]` |
| **IT role** | Custodian only (EMR / MPI technical) — **not** Owner |

**In scope (identity master)** `[A]` / `[B]`: patient/person identity attributes used to match a person across the cluster (for example medical record number, national ID capture, demographics used for registration, contact details used for access).

**Out of scope of this domain:** clinical documentation and medical-record *content* (Domain 2). The CMO is **Consulted** on identity rules that affect clinical safety; the CMO is **not** Owner of this domain.

**Why this Owner:** identity is created and repaired at registration/access, not in the clinical note. Assigning CMO here would collapse “who the patient is” into “what was documented,” which Phase 4 rejected.

---

## 3. Domain 2 — Clinical / Medical Records Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Chief Medical Officer (CMO) `[A]` |
| **Business Data Steward** | Head of Health Information Management (HIM) `[A]` |
| **IT role** | Custodian only (EMR clinical modules) — **not** Owner |

**In scope:** clinical documentation, orders/results as part of the medical record, and related clinical content used for care `[A]` / `[B]`.

**Out of scope of this domain:** enterprise person identity master (Domain 1); clinician credentialing master (Domain 3).

**Consulted:** Patient Access & Experience Director (identity collisions); CQPSO (safety indicators that extract from the record); PDPO when content is personal/health data `[C]` PDPO **name**.

**Why this Owner:** clinical meaning and record integrity sit with medical leadership. HIM executes coding, completeness, and record processes as Steward — not as Owner.

---

## 4. Domain 3 — Provider / Clinician Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Medical Affairs Officer `[A]` |
| **Business Data Steward** | Credentialing Coordinator `[A]` |
| **IT role** | Custodian only — **not** Owner |

**In scope:** practitioner identity, credentials, privileges, and related clinician master attributes used across facilities `[A]` / `[B]`.

**Consulted (contested alternative, not Accountable):** CMO — remains **C** for clinical privilege implications. CMO is not a second Owner.

**Why this Owner:** credentialing and medical-affairs processes own “who may practice,” which is distinct from medical-record content (CMO) and from workforce HR records (HR Director).

---

## 5. Domain 4 — Financial / Billing & Claims Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Chief Financial Officer (CFO) `[A]` |
| **Business Data Steward** | Revenue Cycle Manager `[A]` |
| **IT role** | Custodian only (billing systems) — **not** Owner |

**In scope:** charges, claims, eligibility, and related revenue-cycle data `[A]`.

**Consulted:** Clinical Owner where charge capture depends on clinical documentation; Patient Access where registration data feeds billing.

---

## 6. Domain 5 — Human Resources / Workforce Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | HR Director `[A]` |
| **Business Data Steward** | HR Operations Manager `[A]` |
| **IT role** | Custodian only (HRIS) — **not** Owner |

**In scope:** staff identity, roster, HR employment attributes `[A]`.

**Out of scope of this domain:** clinician *credentialing/privileging* master (Domain 3), even when the person is also an employee.

**Consulted:** Medical Affairs Officer at the employee–practitioner join; PDPO for personal data.

---

## 7. Domain 6 — Supply Chain & Asset Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Supply Chain Director `[A]` |
| **Business Data Steward** | Inventory / Procurement Manager `[A]` |
| **IT role** | Custodian only (ERP / inventory) — **not** Owner |

**In scope:** items, vendors, equipment/asset masters used for supply and assets `[A]`.

**Consulted:** CFO for financial asset treatment; clinical engineering / CMO only as **C** for clinically used devices — not as Owner of the supply domain.

---

## 8. Domain 7 — Quality & Patient Safety Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Chief Quality & Patient Safety Officer (CQPSO) `[A]` |
| **Business Data Steward** | Quality Improvement Manager `[A]` |
| **IT role** | Custodian only — **not** Owner |

**In scope:** incidents, quality indicators, accreditation-evidence datasets owned as quality/safety information `[A]` / `[B]`.

**Consulted:** CMO where indicators are extracted from the medical record; Patient Access where identity matching affects indicator integrity. Those roles are **not** Owners of this domain.

---

## 9. Domain 8 — Reference / Organizational Master Data

| Element | Approved assignment |
| --- | --- |
| **Data Owner** | Strategy & Planning Director `[A]` |
| **Business Data Steward** | Enterprise Data / PMO Analyst **within the DMO** `[A]` |
| **IT role** | Custodian only — **not** Owner |

**In scope:** cluster organizational reference data (facility/department structures, enterprise location codes, planning reference lists) `[A]` / `[B]`.

**DMO boundary:** the steward **sits in** the DMO for coordination skill. The DMO is **not** the Data Owner. Accountable Owner is Strategy & Planning Director.

**Consulted:** CIO (systems that consume org codes) as Custodian/consult; **not** Owner.

NDMO names Reference and Master Data Management as a knowledge domain `[C]`. This Rafid domain is an ownership grouping `[B]`, not a claim that NDMO Domain 7 is implemented.

---

## 10. What this file does not do

- It does not classify any dataset (Phase 5).
- It does not appoint named people.
- It does not give IT business ownership of any domain.

---

## 11. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Phase 4 domain–title map; Rafid fiction | Owner and Steward titles; domain examples |
| `[B]` | Approved ownership principles; federated-by-domain (Phase 3) | One Owner; cluster-wide; no shared A |
| `[C]` | NDMO Standards v1.5 — BDE / BDS / IT Data Steward **names**; MDM domain **name** | Role naming; Domain 8 alignment note |
| `[NDMO verification required]` | Specification-level duties; Organizational Manual | Not cited as control IDs |
