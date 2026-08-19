# Enterprise Ownership Matrix

**Document ID:** RHC-DG-P4-002  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

One-page view of approved enterprise ownership for the fictional Rafid Health Cluster `[A]`. Each domain has **exactly one** Data Owner `[B]`. NDMO Owner name: Business Data Executive `[C]`. Control-level mapping `[NDMO verification required]`.

---

## 2. Matrix

| Domain | Data Owner (one A) | Business Data Steward | IT / Custodian | DMO role |
| --- | --- | --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access | Technical implementation only | Coordinates; not Owner |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) | Technical implementation only | Coordinates; not Owner |
| Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator | Technical implementation only | Coordinates; not Owner |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager | Technical implementation only | Coordinates; not Owner |
| Human Resources / Workforce Data | HR Director | HR Operations Manager | Technical implementation only | Coordinates; not Owner |
| Supply Chain & Asset Data | Supply Chain Director | Inventory / Procurement Manager | Technical implementation only | Coordinates; not Owner |
| Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) | Quality Improvement Manager | Technical implementation only | Coordinates; not Owner |
| Reference / Organizational Master Data | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO | Technical implementation only | Hosts the **Steward** only; **not** Owner |

Coverage: **8 domains, 8 Owners, 0 IT Owners, 0 shared Owners.**

---

## 3. Scope of ownership

Ownership applies to the domain’s data **across all cluster facilities** `[B]`, consistent with Phase 3 federated-by-domain (not federated-by-hospital).

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Phase 4 title map | Cells |
| `[B]` | One Owner; enterprise-wide | Rules |
| `[C]` | NDMO BDE / BDS / IT Data Steward names | Role types |
| `[NDMO verification required]` | Control-level organization requirements | Not used as IDs |
