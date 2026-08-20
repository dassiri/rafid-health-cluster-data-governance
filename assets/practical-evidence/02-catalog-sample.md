# Catalog Sample `[A]`

**Label:** `[A]` Fictional / illustrative Rafid assumption  
**Does not claim:** A live catalog, a catalog product, or NDMO-mandated metadata fields

---

## Purpose

Fifteen fictional **Year-1 catalog MVP** assets. Scope matches Phase 8: three domains only.

```text
Business Glossary  ↔  Metadata / Catalog  ↔  Data Assets
```

Mandatory catalog idea reused: Asset Name, Domain, Data Owner, Steward, Classification, Business Definition, System / Primary System. **System / Primary System** identifies context; it does **not** require exactly one source system.

**Certification** here is internal Rafid trust language (Phase 8), not regulatory certification.

Classification: Public / Internal / Confidential / Restricted `[A][B]` — **not** NDMO national tiers.

Steward: **Business Data Steward** only.

---

## Sample assets (15)

| ID | Data Asset | Domain | Owner | Steward | Classification | Business Definition | CDE | Source / Primary System | Criticality | Lifecycle Status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| CAT-A01 | Patient Registration Dataset | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Restricted | Synthetic extract of cluster registration identity fields | CDE-001, CDE-002 | SYN-REG | High | Active (illustrative) |
| CAT-A02 | Person Master Entity | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Restricted | Logical person master identity (not a physical hub) | CDE-001, CDE-002 | SYN-REG / SYN-EHR | High | Active |
| CAT-A03 | Patient Contact Dataset | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Confidential | Contact fields used for access (watch-item; not extra CDEs) | — | SYN-REG | Medium | Active |
| CAT-A04 | Encounter Documentation Dataset | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | Restricted | Encounter-level clinical documentation context | CDE-003, CDE-004 | SYN-EHR | High | Active |
| CAT-A05 | Diagnosis Coding Dataset | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | Restricted | Recorded diagnosis codes for in-scope encounters | CDE-003 | SYN-EHR | High | Active |
| CAT-A06 | Clinical Summary Extract | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | Restricted | Derived summary for internal quality review (multiple contributing systems) | CDE-003 | SYN-EHR (primary); SYN-QMS (contributing) | Medium | Active |
| CAT-A07 | Claim Submission Dataset | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | Confidential | Claim identifiers and billed service context | CDE-007, CDE-008 | SYN-BILL | High | Active |
| CAT-A08 | Charge Master Extract | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | Internal | Billed service / charge codes in use | CDE-008 | SYN-BILL | Medium | Active |
| CAT-A09 | Claims Analytics Dataset | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | Confidential | Aggregated claims for internal finance reporting (not a BI product) | CDE-007 | SYN-DW (derived) | Medium | Active |
| CAT-A10 | Registration-to-Encounter Link Table | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | Restricted | Conceptual join of person identity to encounter | CDE-002 | SYN-EHR | High | Active |
| CAT-A11 | Encounter-to-Claim Link Table | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | Confidential | Conceptual join of encounter to claim | CDE-007 | SYN-BILL | High | Active |
| CAT-A12 | Patient Identity Exception Log | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Restricted | Documented duplicate/exception identity cases | CDE-001 | SYN-REG | High | Active |
| CAT-A13 | Diagnosis Reference List (consumed) | Clinical / Medical Records Data | Chief Medical Officer (CMO) | Business Data Steward | Internal | Approved diagnosis code list used for validity (clinical meaning) | CDE-003 (validity) | SYN-REF | High | Active |
| CAT-A14 | Claims Dashboard Specification | Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Business Data Steward | Internal | Conceptual consumer of CAT-A09 — not implemented software | — | SYN-BI (conceptual) | Low | Draft |
| CAT-A15 | Person Master Duplicate Review Register | Patient / Person Master Data | Patient Access & Experience Director | Business Data Steward | Restricted | Review log for candidate duplicates (Phase 10 concept) | CDE-001, CDE-002 | SYN-REG | High | Active |

Assets CAT-A14 is a **consumer** in lineage terms, not a data store.

**Out of MVP:** HR, Supply Chain, Quality, and Facility as first-class catalog operating scope (framework exists in Phase 8; not these 15 rows).

**No catalog platform** is named or implemented.
