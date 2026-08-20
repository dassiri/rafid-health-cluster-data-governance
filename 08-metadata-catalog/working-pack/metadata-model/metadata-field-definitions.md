# Metadata Field Definitions

**Document ID:** RHC-DG-P8-WP-006  
**Version:** 1.0  
**Status:** Implemented (working design only)  
**Parent design:** [`minimum-metadata-model.md`](minimum-metadata-model.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

All examples are synthetic `[A]`.

---

## Asset ID

| Attribute | Value |
| --- | --- |
| **Field Name** | Asset ID |
| **Description** | Stable Rafid identifier for the catalog record. Not an NDMO control ID. |
| **Metadata Category** | Governance |
| **Data Type** | String |
| **Occupancy** | Required |
| **Example** | META-PAT-003 |
| **Owner / Responsible Role** | DMO (ID method); Steward assigns on register |

## Asset Name

| Attribute | Value |
| --- | --- |
| **Field Name** | Asset Name |
| **Description** | Business-usable name of the asset or element. |
| **Metadata Category** | Business |
| **Data Type** | String |
| **Occupancy** | Required |
| **Example** | Patient_ID |
| **Owner / Responsible Role** | Business Data Steward (draft); Data Owner (accepts) |

## Asset Type

| Attribute | Value |
| --- | --- |
| **Field Name** | Asset Type |
| **Description** | Year-1 catalog type, plus Data Element for teaching rows in this pack. |
| **Metadata Category** | Technical |
| **Data Type** | String (controlled list) |
| **Occupancy** | Optional (filled in all working-pack rows) |
| **Example** | Data Element |
| **Owner / Responsible Role** | Business Data Steward; Custodian **C** for technical type |

## Business Domain

| Attribute | Value |
| --- | --- |
| **Field Name** | Business Domain |
| **Description** | One of the eight Phase 4 ownership domains. |
| **Metadata Category** | Governance |
| **Data Type** | String (controlled list) |
| **Occupancy** | Required |
| **Example** | Patient / Person Master Data |
| **Owner / Responsible Role** | Data Owner (domain assignment already exists); Steward records it |

## Business Definition

| Attribute | Value |
| --- | --- |
| **Field Name** | Business Definition |
| **Description** | Owner-accepted meaning in business language. Not a technical schema comment. |
| **Metadata Category** | Business |
| **Data Type** | Text |
| **Occupancy** | Required |
| **Example** | The cluster patient identifier (MRN) used to locate the person in operational systems. |
| **Owner / Responsible Role** | Data Owner **A**; Steward **R** |

## Business Owner

| Attribute | Value |
| --- | --- |
| **Field Name** | Business Owner |
| **Description** | Phase 4 Data Owner title. Same role as Data Owner. |
| **Metadata Category** | Governance |
| **Data Type** | String |
| **Occupancy** | Required |
| **Example** | Patient Access & Experience Director |
| **Owner / Responsible Role** | Already assigned at domain level (Phase 4) |

## Business Data Steward

| Attribute | Value |
| --- | --- |
| **Field Name** | Business Data Steward |
| **Description** | Phase 4 appointed steward title for the domain. |
| **Metadata Category** | Governance |
| **Data Type** | String |
| **Occupancy** | Required |
| **Example** | Head of Patient Registration & Access |
| **Owner / Responsible Role** | Nominated by Data Owner; recorded by DMO |

## Source System

| Attribute | Value |
| --- | --- |
| **Field Name** | Source System |
| **Description** | Primary or authoritative system context where one applies. Derived assets may list contributors or “derived / none directly.” |
| **Metadata Category** | Technical |
| **Data Type** | String |
| **Occupancy** | Required |
| **Example** | Registration / MPI (SYN-REG) |
| **Owner / Responsible Role** | IT / Data Custodian **R** for technical accuracy; Steward records |

## Source Dataset

| Attribute | Value |
| --- | --- |
| **Field Name** | Source Dataset |
| **Description** | Parent dataset or master entity when the row is a table or element. |
| **Metadata Category** | Technical |
| **Data Type** | String |
| **Occupancy** | Conditional — required for Table and Data Element rows |
| **Example** | Patient Registration Dataset (META-PAT-002) |
| **Owner / Responsible Role** | Business Data Steward |

## Database / Schema

| Attribute | Value |
| --- | --- |
| **Field Name** | Database / Schema |
| **Description** | Illustrative technical location. Not a live schema. |
| **Metadata Category** | Technical |
| **Data Type** | String |
| **Occupancy** | Optional |
| **Example** | mpi.patient |
| **Owner / Responsible Role** | IT / Data Custodian |

## Table

| Attribute | Value |
| --- | --- |
| **Field Name** | Table |
| **Description** | Illustrative table or object name inside the asset. |
| **Metadata Category** | Technical |
| **Data Type** | String |
| **Occupancy** | Conditional — required for Table and Data Element rows |
| **Example** | patient_master |
| **Owner / Responsible Role** | IT / Data Custodian |

## Column

| Attribute | Value |
| --- | --- |
| **Field Name** | Column |
| **Description** | Illustrative column name. Used only on Data Element rows. |
| **Metadata Category** | Technical |
| **Data Type** | String |
| **Occupancy** | Conditional — required for Data Element rows |
| **Example** | patient_id |
| **Owner / Responsible Role** | IT / Data Custodian |

## Data Type

| Attribute | Value |
| --- | --- |
| **Field Name** | Data Type |
| **Description** | Logical type of the element (String, Date, Integer, Boolean). |
| **Metadata Category** | Technical |
| **Data Type** | String |
| **Occupancy** | Conditional — required for Data Element rows |
| **Example** | String |
| **Owner / Responsible Role** | IT / Data Custodian |

## Classification

| Attribute | Value |
| --- | --- |
| **Field Name** | Classification |
| **Description** | Rafid working tier. Dataset-level in Phase 5; elements inherit parent context in this pack. Not an NDMO national tier. |
| **Metadata Category** | Governance |
| **Data Type** | String (controlled list) |
| **Occupancy** | Required |
| **Example** | Restricted |
| **Owner / Responsible Role** | Data Owner **A**; Steward prepares the pack |

## Criticality

| Attribute | Value |
| --- | --- |
| **Field Name** | Criticality |
| **Description** | Working High / Medium / Low for catalog attention. Not a numeric CDE ranking. Phase 7 CDE selection remains qualitative. |
| **Metadata Category** | Governance |
| **Data Type** | String |
| **Occupancy** | Optional |
| **Example** | High |
| **Owner / Responsible Role** | Data Owner (accepts); Steward proposes |

## CDE Status

| Attribute | Value |
| --- | --- |
| **Field Name** | CDE Status |
| **Description** | Whether the element is one of the 13 catalogue CDEs, a watch-item, or neither. Does not add CDEs. |
| **Metadata Category** | Governance |
| **Data Type** | String |
| **Occupancy** | Conditional — required for Data Element rows |
| **Example** | Yes — CDE-002 |
| **Owner / Responsible Role** | Data Owner confirms CDEs (Phase 7); Steward records |

## Business Rules

| Attribute | Value |
| --- | --- |
| **Field Name** | Business Rules |
| **Description** | Short Owner-relevant constraint (format, uniqueness, relationship). Not a Phase 7 rule engine. |
| **Metadata Category** | Business |
| **Data Type** | Text |
| **Occupancy** | Optional |
| **Example** | Must be unique in the governed person population; must not be blank for Active patients. |
| **Owner / Responsible Role** | Data Owner **A**; Steward **R** |

## Data Quality Status

| Attribute | Value |
| --- | --- |
| **Field Name** | Data Quality Status |
| **Description** | Whether Phase 7 quality design applies. Not a measured Rafid score. |
| **Metadata Category** | Data Quality |
| **Data Type** | String |
| **Occupancy** | Conditional — required when the asset is a CDE or contains confirmed CDEs |
| **Example** | CDE — quality rules designed (Phase 7) |
| **Owner / Responsible Role** | Business Data Steward (monitor); Data Owner (quality outcomes) |

## Refresh Frequency

| Attribute | Value |
| --- | --- |
| **Field Name** | Refresh Frequency |
| **Description** | Governance-level statement of how often the dataset is expected to change. Not an SLA number. |
| **Metadata Category** | Operational |
| **Data Type** | String |
| **Occupancy** | Conditional — when a useful frequency is known for a Dataset |
| **Example** | Event-driven (registration create/update) |
| **Owner / Responsible Role** | IT / Data Custodian; Steward records |

## Lifecycle Status

| Attribute | Value |
| --- | --- |
| **Field Name** | Lifecycle Status |
| **Description** | Operational catalog state of the record. |
| **Metadata Category** | Governance |
| **Data Type** | String (controlled list) |
| **Occupancy** | Required |
| **Example** | Active |
| **Owner / Responsible Role** | Business Data Steward; Owner for Deprecated / Retired |

## Approval Status

| Attribute | Value |
| --- | --- |
| **Field Name** | Approval Status |
| **Description** | Where the record sits in validation / Owner / DMO approval. |
| **Metadata Category** | Governance |
| **Data Type** | String (controlled list) |
| **Occupancy** | Required |
| **Example** | Approved |
| **Owner / Responsible Role** | Steward, then Data Owner, then DMO check |

## Last Reviewed

| Attribute | Value |
| --- | --- |
| **Field Name** | Last Reviewed |
| **Description** | Date the Owner or Steward last confirmed the record. Governance date, not a system SLA. |
| **Metadata Category** | Operational |
| **Data Type** | Date |
| **Occupancy** | Optional |
| **Example** | 2026-08-01 |
| **Owner / Responsible Role** | Business Data Steward |

## Related Business Terms

| Attribute | Value |
| --- | --- |
| **Field Name** | Related Business Terms |
| **Description** | Glossary terms that the asset uses or represents. |
| **Metadata Category** | Business |
| **Data Type** | String (list) |
| **Occupancy** | Optional |
| **Example** | Patient ID; Patient |
| **Owner / Responsible Role** | Business Data Steward |

## Lineage Reference

| Attribute | Value |
| --- | --- |
| **Field Name** | Lineage Reference |
| **Description** | Coarse pointer to conceptual lineage (Source → Transformation → Target → Consumer). Not automated column-level lineage. |
| **Metadata Category** | Governance (holds Phase 8 Lineage Metadata) |
| **Data Type** | String |
| **Occupancy** | Conditional — required for MVP Dataset and Master Data Entity rows |
| **Example** | LIN-REG-PAT-001 (Registration → Person master → Encounter / billing consumers) |
| **Owner / Responsible Role** | Business Data Steward; detail remains Phase 9 |
