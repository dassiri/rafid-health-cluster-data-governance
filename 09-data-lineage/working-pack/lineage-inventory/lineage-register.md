# Lineage Register (Working Pack)

**Document ID:** RHC-DG-P9-WP-006  
**Version:** 1.0  
**Status:** Implemented (synthetic register only — not a live lineage graph)  
**Owner:** Each domain Data Owner **A** for flows targeting that domain; DMO owns the registry method `[B]`  
**Parent design:** Phase 9 artifacts — [`../../15-governance-artifacts.md`](../../15-governance-artifacts.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

This register is a **synthetic** working list of **13** lineage relationships `[A]`.

It instantiates the locked Phase 9 end-to-end example and the Patient Claim Rejection Rate business lineage, using catalog assets from the Phase 8 working pack.

It is **not** a live Rafid inventory, **not** a Purview extract, and **not** measured operational evidence.

Machine-readable register: [`lineage-register.csv`](lineage-register.csv)

---

## 2. Coverage

| Domain | Role in this register | Catalog MVP |
| --- | --- | --- |
| Patient / Person Master Data | Originating capture and person master | In MVP |
| Clinical / Medical Records Data | Encounter documentation and diagnosis | In MVP |
| Financial / Billing & Claims Data | Claims extract, interchange consumer, financial reporting | In MVP |

Provider / Clinician and Facility remain **outside** Year-1 operating scope. Existing coarse pointers `LIN-PRV-001` and `LIN-FAC-001` are not expanded here.

**Count:** 13 hops. No real patient, encounter, or claim identifiers.

---

## 3. Register summary

| Lineage ID | Source → Target | Type | Criticality | MVP | CDE context |
| --- | --- | --- | --- | --- | --- |
| LIN-001 | Patient Registration Dataset → Patient | Business; Conceptual | Critical | P1 | CDE-001; CDE-002 |
| LIN-002 | Patient → Encounter | Conceptual | Critical | P1 | CDE-002 consumed |
| LIN-003 | Encounter Documentation Dataset → Claim Submission Dataset | Conceptual | Critical | P1 | CDE-003 consumed; CDE-008 |
| LIN-004 | Claim Submission Dataset → External Claims Interchange | Conceptual | Critical | P1 | CDE-007; CDE-008 |
| LIN-005 | Claims → Patient Claim Rejection Rate | Business | Critical | P1 | CDE-007; CDE-008; CDE-003 consumed |
| LIN-006 | Patient_ID (registration) → Patient_ID (master) | Technical (selective) | Critical | P1 | CDE-002 |
| LIN-007 | National_ID (registration) → National_ID (master) | Technical (selective) | Critical | P1 | CDE-001 |
| LIN-008 | Diagnosis_Code → claim billing input | Technical (selective) | Critical | P1 | CDE-003 |
| LIN-009 | Claim_ID → Claim_Count | Technical (selective) | Important | P2 | CDE-007 |
| LIN-010 | Encounter_Date → clinical reporting | Business | Important | P2 | CDE-004 |
| LIN-011 | Patient → Claim Submission Dataset | Conceptual | Important | P2 | CDE-002 consumed |
| LIN-012 | Claim Submission Dataset → financial reporting | Business; Conceptual | Important | P2 | CDE-007 |
| LIN-013 | Encounter_ID → claim (consumed) | Technical (selective) | Standard | P3 | Not a catalogue CDE |

---

## 4. Chain groups (Phase 8 pointers reused)

| Chain ID (Phase 8 inventory) | Hops in this pack | Coarse path `[A]` |
| --- | --- | --- |
| LIN-REG-PAT-001 | LIN-001, LIN-006, LIN-007 | Registration / MPI → Person master → Encounter and billing consumers |
| LIN-ENC-001 | LIN-002, LIN-010, LIN-013 | Person master + EMR clinical → Encounter documentation → Claims / reporting consumers |
| LIN-CLM-001 | LIN-003, LIN-004, LIN-005, LIN-008, LIN-009, LIN-011, LIN-012 | Encounter → Charge capture → Claim submission → External claims interchange / reporting |

---

## 5. Critical Lineage Register (Year-1 focus)

Confirmed **Critical** rows (illustrative confirmation — not live DMC minutes):

LIN-001, LIN-002, LIN-003, LIN-004, LIN-005, LIN-006, LIN-007, LIN-008.

These cover the two locked use cases at Levels 1–2, plus selective Level 4 for CDE-001, CDE-002, and CDE-003.

Important and Standard rows remain on the Lineage Registry. They are not all Year-1 Critical Register focus.

---

## 6. Ownership rule on cross-domain hops

Cross-domain rows record the **target** Data Owner as the primary Owner on the register row.

| Hop | Target Owner (row) | Source Owner (still A for source asset) |
| --- | --- | --- |
| LIN-002 | CMO | Patient Access & Experience Director |
| LIN-003 | CFO | CMO |
| LIN-008 | CFO | CMO |
| LIN-011 | CFO | Patient Access & Experience Director |
| LIN-013 | CFO | CMO |

There is **no shared A**. DMO coordinates.

---

## 7. Catalog back-reference

Every hop that names a catalog asset uses a Phase 8 working-pack ID. Consumer-only targets (illustrative KPI or reporting use) are labelled `n/a — business consumer` and do **not** invent a new catalog asset or a new MVP domain.

External Claims Interchange is a **consumer** of META-CLM-001. It is not a fourth MVP catalog asset.

---

## 8. What this file does not do

- Does not catalog the whole fictional organization
- Does not add CDEs or MVP domains
- Does not use real personal data
- Does not claim Purview, Collibra, or ETL ingestion
- Does not represent real MOH or NPHIES architecture
