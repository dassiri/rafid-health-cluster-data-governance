# Data Ownership & Stewardship Standard

**Document ID:** RHC-DG-STD-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]` (DMC informed; DMC **A** if this Standard would change POL-001)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Codifies Phase 4 without redesign.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent policy:** RHC-DG-POL-001  
**Procedure:** RHC-DG-PRC-001  

NDMO names: Business Data Executive, Business Data Steward, IT Data Steward, Data Management Office `[C]`. Specification-level duties `[NDMO verification required]`. No control IDs. No compliance claim.

---

## 1. Purpose

Make Phase 4 ownership **testable** `[B]`: one Owner per domain, cluster-wide, with stewards executing and IT remaining custodian.

---

## 2. Mandatory rules

1. Exactly **one** Data Owner per domain. Shared **A** is not used.
2. Ownership is **enterprise-wide**, not hospital-by-hospital.
3. Data Owner = **business accountability**.
4. Business Data Steward = **operational governance**.
5. IT Data Steward / Custodian = **technical implementation**, never business Owner.
6. DMO = **governance coordination**, not operational Owner of a business domain (including when the Reference/Org Master steward sits in DMO).
7. Contested ownership: one **A**; the other title is **C** only.

---

## 3. Approved domain assignments `[A]` (unchanged)

| Domain | Data Owner | Business Data Steward |
| --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) |
| Provider / Clinician Data | Medical Affairs Officer | Credentialing Coordinator |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager |
| Human Resources / Workforce Data | HR Director | HR Operations Manager |
| Supply Chain & Asset Data | Supply Chain Director | Inventory / Procurement Manager |
| Quality & Patient Safety Data | Chief Quality & Patient Safety Officer (CQPSO) | Quality Improvement Manager |
| Reference / Organizational Master Data | Strategy & Planning Director | Enterprise Data / PMO Analyst within DMO |

---

## 4. Decision rights (Phase 4)

| Decision | A |
| --- | --- |
| Data definition; quality rules; dataset classification; in-policy access; business sharing; metadata/catalog **content**; issue resolution; retention/lifecycle (business) | Data Owner |
| Access exception (out of policy) | DMC |
| Sharing — privacy compliance review (personal data) | PDPO |
| Registry completeness / methodology | DMO |

IT is never **A** on business meaning or classification **value**.

---

## 5. Registries and lifecycle `[B]`

DMO maintains the **Ownership Registry**, **Steward Registry**, and **Ownership Change Record** (schemas: Phase 4; catalogue in `templates-records/`). Owner changes require DMC approval (PRC-001). Vacant Owner title is not DMO ownership. Unassigned-domain escalation: DMO → CDO → DMC → CEO.

---

## 6. Evidence

Registered Owner and Steward titles; DMC ratification of appointments/changes; Change Records.

This Standard does not appoint named people.
