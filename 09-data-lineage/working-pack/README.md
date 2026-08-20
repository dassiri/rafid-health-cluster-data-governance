# Data Catalog & Lineage — Working Pack

**Document ID:** RHC-DG-P9-WP-000  
**Phase:** 9 — Data lineage (applied working pack)  
**Status:** Implemented (documentation and synthetic records only)

**Synthetic / Illustrative / Non-production portfolio project.**

This folder is the **applied Data Catalog & Lineage module** inside the existing Rafid Health Cluster Data Governance project. It sits under Phase 9 so the repository numbering stays intact. Locked Phase 8 and Phase 9 design files are **not** rewritten.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Overview

The working pack shows how Rafid would govern **lineage** for healthcare data assets that already exist in the Phase 8 catalog: where data comes from, how it moves, who owns the description, how critical the hop is, and whether the lineage record is complete enough to publish.

It is governance operating design plus synthetic working records. It is **not** a lineage product, **not** a live graph, and **not** an organisational implementation.

```text
09-data-lineage/working-pack/
├── README.md                          (this file)
├── lineage-framework/
│   ├── lineage-governance.md
│   ├── lineage-types.md
│   ├── lineage-criticality.md
│   ├── lineage-registration-workflow.md
│   └── lineage-mvp-scope.md
├── lineage-inventory/
│   ├── lineage-register.csv
│   └── lineage-register.md
├── business-lineage/
│   └── business-lineage-examples.md
├── conceptual-lineage/
│   └── conceptual-lineage-maps.md
├── technical-lineage/
│   └── selective-technical-lineage.md
├── ownership/
│   └── lineage-ownership.md
├── quality/
│   └── lineage-quality-checks.md
└── examples/
    └── sample-lineage-assets.md
```

---

## 2. Relationship to Phase 9

Phase 9 is the **lineage governance design** (types, model, granularity, nine-criteria criticality, ownership, workflow, quality attributes, MVP).

This pack is **applied evidence**: a 13-row register, worked business and conceptual examples, selective field hops, and catalog back-references.

Locked files remain authoritative. This pack does **not** replace them.

---

## 3. Relationship to Phase 8

Phase 8 remains the source of truth for the Data Catalog, minimum metadata, asset registration, catalog MVP, and coarse lineage-as-metadata.

This pack **consumes** Phase 8 working-pack Asset IDs (`META-PAT-*`, `META-ENC-*`, `META-CLM-*`) and Lineage Reference chain IDs (`LIN-REG-PAT-001`, `LIN-ENC-001`, `LIN-CLM-001`).

It does **not** duplicate the Metadata Management working pack. Metadata field definitions stay in `08-metadata-catalog/working-pack/`.

Phase 8 boundary (unchanged): conceptual lineage and lineage metadata live in Phase 8; detailed lineage governance and this applied register live in Phase 9.

---

## 4. Purpose

Provide practical portfolio evidence that Rafid designed:

- a conceptual Data Catalog connection to lineage
- business and conceptual lineage
- selective technical / field-level lineage where justified
- lineage criticality criteria
- ownership
- a registration workflow
- lineage quality considerations
- a prioritized MVP scope

---

## 5. Lineage types

| Type | Year-1 | Working evidence |
| --- | --- | --- |
| **Business lineage** | Priority | [`business-lineage/business-lineage-examples.md`](business-lineage/business-lineage-examples.md) |
| **Conceptual lineage** | Priority | [`conceptual-lineage/conceptual-lineage-maps.md`](conceptual-lineage/conceptual-lineage-maps.md) |
| **Technical lineage** | Conceptual / selective only | [`technical-lineage/selective-technical-lineage.md`](technical-lineage/selective-technical-lineage.md) |
| **End-to-end lineage** | One locked example | Instantiated as LIN-001–LIN-004 |

See [`lineage-framework/lineage-types.md`](lineage-framework/lineage-types.md).

---

## 6. Lineage governance

Lifecycle, catalog integration, and an illustrative (not deployed) Microsoft Purview mapping:

[`lineage-framework/lineage-governance.md`](lineage-framework/lineage-governance.md)

Pattern:

```text
Data Catalog → Data Asset → Metadata → Lineage Reference → Source / Transformation / Target / Consumer
```

---

## 7. Lineage criticality

Phase 9 two-step rule and nine candidacy criteria are unchanged.

This pack adds a **Rafid illustrative lineage criticality approach** after confirmation:

| Label | Meaning |
| --- | --- |
| **Critical** | Required now; Critical Lineage Register (LIN-001–LIN-008) |
| **Important** | Strongly recommended (LIN-009–LIN-012) |
| **Standard** | Maintained where useful (LIN-013) |

These labels are **not** official NDMO criticality levels.

See [`lineage-framework/lineage-criticality.md`](lineage-framework/lineage-criticality.md).

---

## 8. Lineage ownership

Roles reused exactly: Data Owner, Business Data Steward, DMO, IT / Data Custodian. DMC stays on existing exception/escalation classes only.

See [`ownership/lineage-ownership.md`](ownership/lineage-ownership.md).

---

## 9. Registration workflow

Locked Phase 9 path is extended to a working 12-step path (identify → register → assign Owner/Steward → document source/target → transformation → consumer → criticality → validate → approve → publish → maintain → review).

No new Phase 6 procedure. Exceptions reuse the Data Governance Exception Procedure.

See [`lineage-framework/lineage-registration-workflow.md`](lineage-framework/lineage-registration-workflow.md).

---

## 10. Lineage inventory

**13 synthetic relationships** in [`lineage-inventory/lineage-register.csv`](lineage-inventory/lineage-register.csv) and [`lineage-inventory/lineage-register.md`](lineage-inventory/lineage-register.md).

Each row includes Lineage ID, source/target domain and asset, element where applicable, transformation, lineage type, criticality, Owner, Steward, quality consideration, validation status, and last reviewed date.

---

## 11. Business lineage

Four examples: Registration → Patient Master; Encounter → Clinical Reporting; Claims → Financial Reporting; Patient Claim Rejection Rate (locked KPI example).

---

## 12. Conceptual lineage

Three maps: the locked registration-to-interchange chain; patient source to clinical reporting; claims extract to financial reporting / interchange.

---

## 13. Selective technical lineage

Four field-level examples: Patient_ID; National_ID; Diagnosis_Code → claims; Claim_ID → `Claim_Count = COUNT(DISTINCT Claim_ID)`.

Clearly labelled illustrative. No ETL deployment is claimed.

---

## 14. Lineage quality

Lineage **metadata** quality uses Phase 9 attributes (Completeness, Accuracy, Timeliness, Consistency, Traceability) plus an applied Validity check on coded values.

This is **not** a second Data Quality Framework.

See [`quality/lineage-quality-checks.md`](quality/lineage-quality-checks.md).

---

## 15. Catalog integration

Sample catalog pages with lineage pointers: [`examples/sample-lineage-assets.md`](examples/sample-lineage-assets.md).

Catalog fields shown: Asset ID, Asset Name, Asset Type, Domain, Business Definition, Data Owner, Business Data Steward, System, Classification, CDE Status, Quality Status, Lineage Reference, Lifecycle Status, Catalog Status.

---

## 16. MVP scope

**Priority domains only** (same as Phase 8 catalog MVP):

1. Patient / Person Master Data  
2. Clinical / Medical Records Data  
3. Financial / Billing & Claims Data  

| Priority | Focus | Rows |
| --- | --- | --- |
| Priority 1 | Critical assets / CDE-related lineage | LIN-001–LIN-008 |
| Priority 2 | Major downstream reporting lineage | LIN-009–LIN-012 |
| Priority 3 | Additional operational lineage | LIN-013 |

See [`lineage-framework/lineage-mvp-scope.md`](lineage-framework/lineage-mvp-scope.md).

---

## 17. Limitations

- Synthetic records only; volumes are small by design  
- No lineage platform, scanner, graph database, or live ingestion  
- No real patient, encounter, or claims data  
- Field-level rows are teaching records; enterprise column-level lineage is not claimed  
- Technical lineage is described, not automated  
- Microsoft Purview is an illustrative mapping only and is **not** deployed  
- Official NDMO lineage requirements remain unverified  

---

## 18. NDMO positioning

This is Saudi-contextualized portfolio work. Data Catalog and Metadata is an NDMO knowledge-domain **name** (`MCM` as recorded in Phase 2) `[C]`. Specific lineage requirements remain `[NDMO verification required]`.

| Bucket | This pack |
| --- | --- |
| Project design `[A][B]` | Register, working criticality labels, 12-step path, selective field hops, MVP cut |
| Conceptual alignment `[C]` | Catalog domain **name**; role **names**; Trusted Data principle **name** |
| Verification required | Official NDMO lineage mandates, artifacts, and national interchange rules |
| Official requirement | **Not claimed** |

**Not NDMO compliant. Not PDPL compliant.** No certification is claimed.

---

## 19. Portfolio disclaimer

This is a fictional portfolio project.

It does **not** claim legal compliance, NDMO certification, PDPL compliance, production deployment, real patient data, a real healthcare implementation, automated lineage, or deployment of Microsoft Purview (or any other catalog/lineage tool).

Rafid Health Cluster is fictional. All names, identifiers, and attributes are fabricated.

**Synthetic / Illustrative / Non-production portfolio project.**
