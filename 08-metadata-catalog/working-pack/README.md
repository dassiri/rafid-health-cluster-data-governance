# Metadata Management — Working Pack

**Document ID:** RHC-DG-P8-WP-000  
**Phase:** 8 — Metadata and catalog (applied working pack)  
**Status:** Implemented (documentation and synthetic records only)

**Synthetic / Illustrative / Non-production portfolio project.**

This folder is the **applied Metadata Management module** inside the existing Rafid Health Cluster Data Governance project. It sits under Phase 8 so the repository numbering stays intact (`02-governance-strategy` is already Phase 2). Locked Phase 8 design files are **not** rewritten.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Overview

The working pack shows how Rafid would govern **metadata** across healthcare data assets: what an asset means, who owns it, how it is classified, whether it is a Critical Data Element, and whether the description is approved for catalog discovery.

It is governance operating design plus synthetic working records. It is **not** a catalog product, **not** a live inventory, and **not** an organisational implementation.

```text
08-metadata-catalog/working-pack/
├── README.md                          (this file)
├── framework/
│   ├── metadata-management-framework.md
│   ├── metadata-categories.md
│   ├── metadata-governance.md
│   └── metadata-lifecycle.md
├── metadata-model/
│   ├── minimum-metadata-model.md
│   ├── metadata-field-definitions.md
│   └── minimum-metadata-model.csv
├── business-glossary/
│   ├── business-glossary.md
│   └── business-glossary.csv
├── metadata-inventory/
│   ├── metadata-inventory.md
│   └── metadata-inventory.csv
├── data-catalog/
│   ├── catalog-governance-model.md
│   ├── asset-registration-workflow.md
│   └── catalog-mvp-scope.md
└── examples/
    └── sample-catalog-assets.md
```

---

## 2. Objectives

- Apply the Phase 8 metadata framework to a practical field model  
- Record a business glossary that reuses Phase 8 definitions  
- Produce a synthetic metadata inventory for priority healthcare assets  
- Document catalog governance, registration, and a limited MVP  
- Show how metadata supports Data Quality (CDEs, rules, issues) without duplicating Phase 7  

---

## 3. Project context

Rafid Health Cluster is **fictional**. This pack consumes:

| Existing design | What this pack reuses |
| --- | --- |
| Phase 3 operating model | DMO, DMC, Steward Forum, Custodian, CDO |
| Phase 4 ownership | Eight domains; Owner and Steward titles |
| Phase 5 classification | Public / Internal / Confidential / Restricted |
| Phase 6 PRC-004 | Metadata Registration Procedure |
| Phase 7 | Exactly 13 CDEs; seven quality dimensions; watch-items |
| Phase 8 locked files | Categories, minimum metadata, glossary structure, catalog MVP, registration workflow |
| Phase 9 | Coarse lineage as a pointer only |

Related recruiter samples remain in [`../../assets/practical-evidence/`](../../assets/practical-evidence/).

---

## 4. Metadata categories

Phase 8 locks **seven** categories. This pack files inventory columns into **five working categories**:

| Working category | Holds |
| --- | --- |
| Business Metadata | Definition, terms, purpose, business rules |
| Technical Metadata | System, schema, table, column, data type |
| Operational Metadata | Refresh / last reviewed |
| Governance Metadata | Owner, Steward, classification, CDE flag, lifecycle, approval |
| Data Quality Metadata | Quality status and issue pointers when Phase 7 exists |

Classification stays **mandatory** (Phase 8 Security / Classification). Lineage is stored as **Lineage Reference** (Phase 8 Lineage Metadata). The five names are a Rafid working grouping `[A][B]`, not an official NDMO taxonomy.

---

## 5. Metadata Management approach

```text
Identify → Register → Classify → Assign Owner & Steward
→ Complete Metadata → Validate → Approve → Publish → Review → Update / Retire
```

This operating sequence is consistent with the Phase 8 lifecycle and PRC-004. Classify and ownership are recorded **before** remaining metadata is completed so unlabeled assets are not treated as Public.

---

## 6. Minimum metadata model

Occupancy: **Required** / **Conditional** / **Optional**.

Required for publish includes Asset ID, Asset Name, Domain, Business Definition, Data Owner, Business Data Steward, Source System, Classification, Lifecycle Status, and Approval Status.

Not every field is mandatory. Quality, operational, and lineage fields are filled when the capability exists. Fake scores are not invented.

---

## 7. Business glossary

**25 terms.** Phase 8 definitions for Patient, Encounter, Provider, Claim, Facility, Department, and Diagnosis are reused unchanged.

Includes Patient ID (CDE-002), National ID (CDE-001), Encounter Date (CDE-004), Diagnosis (CDE-003), Claim Identifier (CDE-007), Charge Code (CDE-008), Provider Identifier (CDE-005), and Facility / Department Code (CDE-013).

Date of Birth, Gender, Encounter ID, Admission Date, and Discharge Date are glossary/inventory items. They are **not** additional CDEs.

The glossary is not SNOMED, ICD, or a national terminology standard.

---

## 8. Metadata inventory

**20 synthetic assets:** Patient, Encounter, and Claim in MVP scope; Provider and Facility as framework-only rows because Encounter depends on them.

Element rows include Patient_ID, National_ID, Date_of_Birth, Gender, Encounter_ID, Encounter_Date, Admission_Date, Discharge_Date, Diagnosis_Code, Claim_ID, Charge_Code, Provider_ID, and Facility_ID.

All values are fabricated. No real personal data.

---

## 9. Data Catalog governance

The catalog is the governed inventory of **described** assets. CDO / DMO own the programme. Data Owners own domain content. DMC does not approve every asset.

Publishing metadata is not an access grant and not a PDPL determination.

An illustrative Microsoft Purview mapping is included as a possible implementation target only. **Purview is not deployed.**

---

## 10. Asset registration workflow

Thirteen steps from identify through update/retire, with actor, input, action, output, and decision at each step. Alignment to PRC-004 is explicit. No second procedure is created.

---

## 11. MVP scope

**Priority domains only:**

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Financial / Billing & Claims Data  

The MVP does not catalog the whole fictional organization. Provider and Facility stay outside Year-1 operating scope. A completion checklist is in [`data-catalog/catalog-mvp-scope.md`](data-catalog/catalog-mvp-scope.md).

---

## 12. Governance roles

| Role | Metadata duty (summary) |
| --- | --- |
| Data Owner | **A** for definition, classification, catalog content, Certified status |
| Business Data Steward | **R** for draft, maintain, validate, Registered/Reviewed |
| DMO | Method, governance check, programme; cannot rewrite meaning |
| IT / Data Custodian | Technical metadata; never business Owner |
| Data Management Committee | Existing escalation/exception classes only |
| Steward Forum / Domain huddle | Practice and in-domain decisions — not a new Council |

---

## 13. Relationship to Data Quality

```text
Metadata asset
      ↓
CDE identification (13 catalogue CDEs)
      ↓
Quality rules (Phase 7)
      ↓
Quality results / issues (when monitoring exists)
      ↓
Governance monitoring
```

This pack points at Phase 7. It does **not** copy rules, thresholds, or the issue procedure. Quality metadata is capability-dependent.

A complementary operational scorecard exists as a **separate** portfolio repository. This framework does not import its measured figures.

---

## 14. NDMO / PDPL positioning

Data Catalog and Metadata is an NDMO knowledge-domain **name** (`MCM` as recorded in Phase 2) `[C]`. This pack is conceptually aligned with relevant data management governance considerations.

| Bucket | This pack |
| --- | --- |
| Project design `[A][B]` | Working categories, occupancy, inventory, MVP cut, registration steps |
| Conceptual alignment `[C]` | Domain **name** MCM; role **names** |
| Verification required | Official NDMO metadata fields and categories; PDPL operational application |
| Official requirement | **Not claimed** |

**Not NDMO compliant. Not PDPL compliant.** No certification is claimed.

---

## 15. Limitations

- Synthetic records only; volumes are small by design  
- No catalog platform and no live ingestion  
- No real patient, provider, or claims data  
- Element-level rows are teaching records; Year-1 publish does not require every column  
- Retention, access control products, and automated lineage are out of scope  
- Official NDMO field lists remain unverified  

---

## 16. Portfolio disclaimer

This is a fictional portfolio project.

It does **not** claim legal compliance, NDMO certification, PDPL compliance, production deployment, real patient data, a real healthcare implementation, or deployment of Microsoft Purview (or any other catalog tool).

Rafid Health Cluster is fictional. All names, identifiers, and attributes are fabricated.
