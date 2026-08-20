# Catalog Governance Model (Working Pack)

**Document ID:** RHC-DG-P8-WP-009  
**Version:** 1.0  
**Status:** Implemented (operating model only — not a deployed catalog)  
**Owner:** CDO / DMO — catalog **programme** `[B]`; Data Owner **A** for domain catalog **content**  
**Parent design:** [`../../06-data-catalog-design.md`](../../06-data-catalog-design.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Nature of this model

This is a **governance and operating model** for how a data catalog would be managed at Rafid.

It is **not** a deployed catalog. It is **not** Microsoft Purview, Collibra, Atlan, or Informatica. NDMO describes an automated catalog as a national **concept** `[C]`. Rafid does not have that tool in this repository `[A]`. Control-level catalog requirements remain `[NDMO verification required]`.

**Publish** means governed **metadata** is discoverable. Publish is not open release of clinical data and not access approval.

---

## 2. Catalog scope

| Included in the catalog idea | Not included |
| --- | --- |
| Described data assets in approved scope | The underlying Restricted / Confidential **data** |
| Owner, Steward, classification, definition | Access provisioning |
| Coarse lineage **references** | Automated column-level lineage (Phase 9) |
| Quality **status pointers** when Phase 7 exists | A second Data Quality scorecard product |

**Year-1 operating cut** is the catalog MVP: three domains only. The other five domains remain in the framework.

---

## 3. Catalog ownership

| Layer | Accountable |
| --- | --- |
| Catalog **programme / methodology** | CDO / DMO |
| Domain catalog **content / definitions** | Data Owner (Phase 4 row 8) |
| Classification **value** | Data Owner (Phase 4 row 3) |
| Technical metadata accuracy | IT / Data Custodian **R** (never A for meaning) |
| Policy exception to skip Owner-accepted definition | DMC via existing exception procedure |

No new DMC decision class.

---

## 4. Asset registration

Registration follows PRC-004 and the 13-step working path in [`asset-registration-workflow.md`](asset-registration-workflow.md).

Intake may come from Steward identification, Custodian system change, or DMO completeness review. DMO does not invent domain meaning to fill a gap.

---

## 5. Metadata requirements

Before an **operational** asset is published in MVP scope:

| Requirement | Rule |
| --- | --- |
| Required fields | Asset ID, Asset Name, Domain, Business Definition, Data Owner, Business Data Steward, Source System, Classification, Lifecycle Status, Approval Status |
| Classification | A Rafid tier must be present. Unlabeled is not Public |
| CDE Status | Required on Data Element rows |
| Quality status | Required when the asset is a confirmed CDE or contains confirmed CDEs |
| Lineage reference | Required on MVP Dataset and Master Data Entity rows |
| Optional / remaining conditional | May be empty; do not fabricate values |

---

## 6. Validation

Steward validation checks:

- Required fields present
- Domain, Owner, and Steward match the Phase 4 map
- Glossary links do not contradict approved terms
- No Restricted/Confidential **data** pasted into the metadata record
- Asset Type and occupancy rules followed

Failed validation returns the record (Approval Status = Returned) with a gap list. It does not silently publish.

---

## 7. Approval

| Check | Who | Decision |
| --- | --- | --- |
| Steward validation | Business Data Steward | Ready for Owner, or Returned |
| Content approval | Data Owner | Accepts definition and catalog content |
| Governance check | DMO | Record is complete as a governed object; meaning is not rewritten |
| Certified trust status | Data Owner | Optional further trust step; not required for every Registered asset |

---

## 8. Publication

After approval, Steward / DMO set Lifecycle Status = **Active** and make metadata visible to MVP users (Data Owners, Business Data Stewards, DMO).

Analyst and executive personas exist in the conceptual catalog. They are not the MVP operating user set.

---

## 9. Review

Steward reviews meaning, classification, ownership, and CDE flag periodically. No numeric SLA.

Material change (definition, classification, Owner, CDE confirmation) returns to Owner approval.

Last Reviewed is optional metadata. Absence is a metadata-quality gap, not a publish block.

---

## 10. Change management

| Change | Path |
| --- | --- |
| Typo / technical location update | Steward maintains; Custodian **C** |
| Business definition or usage | Owner approval |
| Classification change | Classification procedure (PRC-002) then catalog update |
| Domain / Owner change | Phase 4 ownership lifecycle — not a catalog-only edit |
| Out-of-policy exception | Data Governance Exception Procedure (**DMC = A**) |

---

## 11. Retirement

| Status | Meaning |
| --- | --- |
| Deprecated | Do not use for new work; still visible as a warning |
| Retired | No longer an operational catalog asset; record retained by DMO |

Owner decides. DMO keeps the record. Retired metadata is not deleted as if the asset never existed.

---

## 12. Access considerations

| Rule | Application |
| --- | --- |
| Catalog shows **metadata** | Name, Owner, classification, definition, status |
| Catalog does **not** show | Underlying Restricted or Confidential records |
| Access to data | Phase 4/5/6 sharing and access path — Owner in-policy; DMC for Policy exceptions; PDPO **A** on the privacy sharing row |
| Personal-data indicator | Recommended metadata only; not the personal data itself |

Cybersecurity architecture is not designed in this file.

---

## 13. Illustrative implementation mapping to Microsoft Purview `[A][B]`

This section is an **illustrative mapping**. Purview is **not** deployed in this project. No ingestion, scan, or screenshot is claimed.

| Rafid working concept | Illustrative Purview analogue |
| --- | --- |
| Data Catalog (governed inventory) | Microsoft Purview Data Catalog / Unified Catalog as a possible implementation target |
| Business Glossary | Glossary / term management |
| Asset registration workflow | Catalog workflow / approval (however the tenant is configured) |
| Classification (Rafid tiers) | Custom classification or governance attributes — **not** automatic equivalence to Purview system classifications |
| Data Owner / Steward | Data owner / expert roles on the asset |
| Lineage Reference | Purview lineage, if later populated — Rafid Year-1 remains conceptual (Phase 9) |
| CDE Status | Custom attribute or critical-data annotation |
| Data Quality Status | Pointer to a quality process; not a substitute for Phase 7 |

If Purview were later selected, Rafid occupancy rules and Owner **A** for meaning would still apply. The tool would not become Data Owner.

---

## 14. What this file does not do

- Does not purchase or configure a catalog product
- Does not claim NDMO catalog automation
- Does not expand MVP to all eight domains
