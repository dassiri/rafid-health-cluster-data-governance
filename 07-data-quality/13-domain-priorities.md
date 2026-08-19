# Domain Quality Priorities (Illustrative)

**Document ID:** RHC-DG-P7-013  
**Version:** 1.0  
**Status:** Implemented (illustrative priorities only)  
**Owner:** Each domain Data Owner **A** for confirming which priorities become CDEs or issues  
**Approver:** CDO `[B]` (this list as a framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with Domain Huddles `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Approved illustrative domain priorities; not extra CDEs.

**Phase:** 7 — Data quality  
**Does not decide:** Additional CDEs; live heat maps; CBAHI/MOH overlay as verified requirements `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records **illustrative quality priorities** by domain `[A]`.

They explain **where to look first**. They are **not**:

- Additional CDEs (the catalogue remains **exactly 13**)
- Measured Rafid findings
- NDMO-mandated defect lists `[NDMO verification required]`

Where a priority maps to a catalogue CDE, the CDE ID is noted. Where it does not, it remains a **watch-item** until the two-step CDE method confirms dedicated CDE governance.

---

## 2. Approved illustrative priorities `[A]`

### Patient / Person Master Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Identity duplication | CDE-002 Patient identifier (MRN); uniqueness also on CDE-001 |
| Missing/incorrect National ID | CDE-001 National ID |
| Stale contact information | **Watch-item** — not a 14th CDE |

**Owner:** Patient Access & Experience Director · **Steward:** Head of Patient Registration & Access

### Clinical / Medical Records Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Missing structured fields | Watch-item unless later confirmed as a CDE; diagnosis structured coding is CDE-003 |
| Invalid diagnosis codes | CDE-003 Diagnosis code |
| Delayed documentation | CDE-004 Encounter documentation timestamp |

**Owner:** Chief Medical Officer (CMO) · **Steward:** Head of Health Information Management (HIM)

### Provider / Clinician Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Expired credentials undetected | CDE-006 Credential expiry date |
| Provider-ID mismatch between HR and EMR | CDE-005 Provider identifier (consistency with CDE-009 as cross-domain) |

**Owner:** Medical Affairs Officer · **Steward:** Credentialing Coordinator  
**Consulted (not a second A):** HR Director at the employee–practitioner join (Phase 4)

### Financial / Billing & Claims Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Claim rejections from coding mismatch | CDE-008 Billed service / charge code (consistency with CDE-003) |
| Duplicate claims | CDE-007 Claim identifier |
| Incomplete charge capture | CDE-008 Completeness |

**Owner:** Chief Financial Officer (CFO) · **Steward:** Revenue Cycle Manager

### HR / Workforce Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Roster-to-EMR provider mismatch | CDE-009 Employee / staff identifier (consistency with CDE-005) |
| Payroll entry errors | Watch-item on CDE-009 accuracy/completeness — not a 14th CDE |

**Owner:** HR Director · **Steward:** HR Operations Manager

### Supply Chain & Asset Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Inconsistent item coding | CDE-010 Item master code |
| Expiry-tracking gaps | CDE-011 Item expiry date |

**Owner:** Supply Chain Director · **Steward:** Inventory / Procurement Manager

### Quality & Patient Safety Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Underreporting | Watch-item (completeness of incident **events**, not a 14th field-CDE) |
| Inconsistent severity classification | CDE-012 Incident severity classification |
| Delayed entry | Watch-item (timeliness of incident records) — not a 14th CDE |

**Owner:** Chief Quality & Patient Safety Officer (CQPSO) · **Steward:** Quality Improvement Manager

### Reference / Organizational Master Data

| Priority `[A]` | Relation to CDE catalogue |
| --- | --- |
| Facility/department code drift | CDE-013 Facility / department code |
| Lack of single source of truth | Governance principle on CDE-013; **Phase 10 architecture is not built** |

**Owner:** Strategy & Planning Director · **Steward:** Enterprise Data / PMO Analyst within DMO (DMO is not Owner)

---

## 3. All eight domains

The eight Phase 4 domains are all represented above. Priorities are `[A]` illustrative.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Phase 7 domain priority list | Section 2 |
| `[B]` | Watch-item vs confirmed CDE | Method |
| `[C]` | Data Quality domain **name** | Context |
| `[NDMO verification required]` | Sector quality-indicator mandates as CDE law | Not claimed |
