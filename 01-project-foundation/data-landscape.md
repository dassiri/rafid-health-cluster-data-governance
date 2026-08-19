# Data Landscape

**Document ID:** RHC-DG-P0-003  
**Phase:** 0 — Project Foundation  
**Status:** Documented  
**Does not decide:** Classification labels for datasets, golden-record design, catalog tool, or quality rules

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document describes **what data Rafid is assumed to hold**, where it lives, and which landscape issues motivate governance. It is a current-state sketch `[A]` / `[B]`, not a data catalog and not an NDMO data-identification exercise (`DC.3.1` is later `[C]`).

NDMO requires entities to identify and inventory datasets and artifacts as part of classification `[C]` (NDMO Standards v1.5, `DC.3.1`). This landscape is **not** that inventory. It is a Phase 0 input so later inventory work has a bounded starting map.

---

## 2. Landscape principles for this sketch `[B]`

- Describe domains and systems, not a field-level model.
- Prefer healthcare-typical domains; do not invent NDMO dataset IDs.
- Record pain points as assumptions `[A]`, not audit findings.
- Flag candidate master data **objects** without designing MDM (Phase 10).

---

## 3. Data domains `[A]` / `[B]`

Domain names below are cluster working names. They are **not** NDMO’s 15 knowledge domains. NDMO domain names are listed in [`../02-governance-strategy/ndmo-alignment-approach.md`](../02-governance-strategy/ndmo-alignment-approach.md).

| Working domain | Examples of data | Typical systems (generic) | Sensitivity (informal as-is) |
| --- | --- | --- | --- |
| Patient identity and encounter | Demographics, identifiers, visits, ADT events | EMR, registration, MPI (incomplete) | High — personal and health data |
| Clinical documentation | Notes, orders, results, meds, allergies, problems | EMR | High |
| Diagnostics | Lab results, imaging studies and reports | LIS, RIS/PACS | High |
| Pharmacy and medication | Dispense, administration, formulary | Pharmacy system, EMR MAR | High |
| Scheduling and referrals | Appointments, cluster referrals | EMR, scheduling | Medium–high |
| Revenue cycle | Charges, claims, eligibility | Billing / HIS financial | Medium–high (financial + identity) |
| Workforce | Staff identity, roster, credentials, payroll keys | HRIS | High (personal) |
| Supply and assets | Items, vendors, equipment | ERP / inventory | Lower–medium |
| Quality and safety | Incidents, indicators, accreditation evidence | Quality databases, spreadsheets | High (often patient-linked) |
| Public health / MOH reporting | Notifiable conditions, statistical returns | Extracts, files, portals | High |
| Corporate | Contracts, policy files, email, scanned records | File shares, email, ECM (limited) | Mixed |
| Research / teaching (limited) | De-identified extracts, limited identifiable studies | Isolated shares | High if identifiable |

Informal sensitivity in the last column is **not** NDMO classification. Official NDMO levels are Top Secret, Secret, Confidential, and Public, assigned via impact assessment `[C]` (NDMO Standards v1.5, `DC.3.2`). Applying those levels is Phase 5.

---

## 4. System landscape `[A]`

Names are generic on purpose (no vendor lock-in in the case study).

| System class | Role | Notes |
| --- | --- | --- |
| Cluster EMR | Core clinical and encounter record | Deployed cluster-wide; older sites still dual-running paper for some units |
| Master patient index | Intended unique patient key | Present but not enforced; duplicates persist |
| LIS | Laboratory | Two instances (tertiary vs. general hospitals), different code sets |
| RIS/PACS | Imaging | Central PACS; one hospital still on a local archive |
| Pharmacy | Inpatient and outpatient dispense | Interface to EMR incomplete at two hospitals |
| Billing / revenue | Claims and patient billing | Separate from EMR; manual reconciliation |
| HRIS | Workforce | Cluster corporate; facility shadow spreadsheets remain |
| ERP | Finance and supply | Partial roll-out |
| Integration engine | HL7 and file drops | Limited monitoring; little documented lineage |
| Shared drives / email | Unstructured content | Significant shadow data |
| External portals | MOH and other national reporting | File upload and form-based |

NDMO’s Data Catalog and Metadata domain expects an automated catalog as a single point of reference for metadata `[C]` (Domain 2 definition). Rafid is assumed **not** to have this tool `[A]`. Tool selection is out of Phase 0–2.

---

## 5. Data movement (conceptual) `[A]` / `[B]`

High-level flows only. No lineage diagrams are approved as operational lineage (Phase 9).

1. **Registration → EMR → clinical ancillaries** (orders/results).
2. **EMR → billing** (charges; often delayed or incomplete).
3. **EMR / LIS / quality files → MOH and cluster reports** (extracts).
4. **HRIS → access provisioning** (not fully joined to EMR user identity).
5. **Partner / vendor** processing (billing outsource, EMR vendor support, cloud components) — contracts uneven `[A]`.

NDMO Purpose and Scope includes business partners handling government data `[C]`. Partner control design is later.

---

## 6. Candidate master and reference data (observation only)

These are **landscape observations**, not an MDM operating model `[B]`. Phase 10 will decide scope.

| Candidate object | Why it appears in the landscape `[A]` |
| --- | --- |
| Patient / Person | Duplicate MRNs; inconsistent National ID and mobile numbers |
| Provider / Practitioner | Same physician, multiple EMR IDs across sites |
| Location / Facility / Department | Inconsistent department codes; PHC naming drift |
| Service / Charge item | Billing vs. clinical catalogs diverge |
| Medication / formulary item | Local vs. cluster formulary mismatch |
| Payer / contract | Multiple codes for the same insurer |

NDMO Domain 7 is Reference and Master Data Management `[C]`. No Rafid MDM policy is issued here.

---

## 7. Known landscape issues driving governance `[A]`

| Issue | Operational effect | Governance implication (not a design) |
| --- | --- | --- |
| Duplicate patients | Safety and reporting risk | Ownership of identity data is unclear |
| Dual clinical systems | Conflicting results and med lists | Need for system-of-record decisions later |
| Shadow spreadsheets | Unclassified personal data on shares | Lifecycle and classification later |
| Unclear partner processing | Unknown copies of patient data | Sharing and processor governance later |
| No catalog | Analysts cannot find authoritative data | Metadata program later |
| No issue log | Repeat incidents | NDMO later expects a data-issue register (`DG.8.2`) `[C]` — not implemented here |

---

## 8. Personal data and health data `[A]` + `[NDMO verification required]`

The landscape includes data that would enable identification of individuals (patients, staff, visitors) and data concerning health `[A]`.

NDMO defines Personal Data in the Standards (identification of a Saudi citizen, in the extracted definitions) `[C]`. NDMO Domain 14 addresses Personal Data Protection `[C]`. Saudi PDPL and health-sector rules may also apply to a real cluster `[NDMO verification required]`.

Phase 0 records that **personal and health data are in the landscape**. It does not define lawful bases, consent operationalization, or DPIA procedures.

---

## 9. Forms of data in scope for later governance `[C]` + `[A]`

NDMO Purpose and Scope states that the Standards apply to government data regardless of form, including paper records, emails, electronic data, voice recordings, videos, maps, photos, scripts, handwritten documents, or any other recorded form `[C]`.

Rafid is assumed to hold all of these forms `[A]`. Unstructured and paper records are therefore **not** out of the future governance boundary, even though Phase 0 only sketches systems.

---

## 10. Intentionally unresolved

- Authoritative system-of-record per domain (Phase 3+ / architecture, NDMO Domain 6).
- Official classification of any dataset (Phase 5).
- Inventory completeness and catalog IDs (Phase 8 / `DC.3.1`).
- Which domains are year-1 MDM priorities (Phase 10 and 13).
- Data residency and cross-border processing facts `[A]` not specified; any real cluster would need `[NDMO verification required]` against current national rules.

---

## 11. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Portfolio fiction | Systems, issues, volumes implied by the org profile |
| `[B]` | Healthcare data-landscape / domain-grouping practice | Section structure |
| `[C]` | NDMO Standards v1.5 — Purpose and Scope; Domain 2 definition; Domain 7; Domain 14; `DC.3.1`, `DC.3.2`; `DG.8.2` | Inventory/classification later; forms of data; MDM domain name; personal data domain; issue register exists as a later control |
