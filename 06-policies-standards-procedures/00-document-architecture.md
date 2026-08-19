# Document Architecture

**Document ID:** RHC-DG-P6-ARCH  
**Version:** 1.0  
**Status:** Implemented  
**Owner:** Data Management Office / CDO `[B]`  
**Approver:** Data Management Committee (for the Policy this architecture supports) `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Phase 6 implementation; corrects 4-Standards wording to **5 Standards**.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Stack

**1 Policy + 5 Standards + 6 Procedures** `[A][B]`, mapping to Phase 2 L3 / L4 / L5.

Templates and records are **supporting artifacts**. They are not a second policy and not additional standards.

NDMO expects entity policies and guidelines aligned to national policies and standards `[C]` at narrative level. This architecture is an entity design `[B]`. Specification-level mapping is `[NDMO verification required]`. **No compliance is claimed. No control IDs are cited.**

---

## 2. Inventory

### Policy (exactly one)

| ID | Title |
| --- | --- |
| RHC-DG-POL-001 | Enterprise Data Governance Policy |

### Standards (exactly five)

| ID | Title |
| --- | --- |
| RHC-DG-STD-001 | Data Ownership & Stewardship Standard |
| RHC-DG-STD-002 | Data Classification Standard |
| RHC-DG-STD-003 | Data Quality Standard |
| RHC-DG-STD-004 | Metadata & Catalog Standard |
| RHC-DG-STD-005 | Master Data Management Standard (**standalone**) |

### Procedures (exactly six)

| ID | Title |
| --- | --- |
| RHC-DG-PRC-001 | Data Ownership Appointment Procedure |
| RHC-DG-PRC-002 | Data Classification Procedure |
| RHC-DG-PRC-003 | Data Quality Issue Management Procedure |
| RHC-DG-PRC-004 | Metadata Registration Procedure |
| RHC-DG-PRC-005 | Data Access / Sharing Governance Procedure |
| RHC-DG-PRC-006 | Data Governance Exception Procedure |

---

## 3. Which layer answers which question `[B]`

| Layer | Answers |
| --- | --- |
| Policy | Must / must not at enterprise level |
| Standard | How “good” looks for a topic (testable rules without play-by-play) |
| Procedure | How a role performs a process (steps, evidence, escalation) |
| Template / record | What is captured as evidence |

---

## 4. Authority `[B]`

| Document type | Document owner (maintain) | Approver |
| --- | --- | --- |
| Policy | CDO | Data Management Committee |
| Standard | CDO / DMO | CDO (DMC informed; DMC **A** if the standard would change Policy intent) |
| Procedure | DMO | CDO |
| Template / record schema | DMO | CDO |

This does not change Phase 3: L3 policy **A = DMC**; governance exceptions **A = DMC**.

---

## 5. What this architecture forbids

- A second enterprise Data Governance Policy
- Folding MDM into Metadata & Catalog
- Reverting to four Standards
- Treating Templates as Standards
- Equating Rafid classification labels with unresolved NDMO national tier names `[NDMO verification required]`
