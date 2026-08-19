# Phase 8 — Metadata Management and Data Catalog

**Document ID:** RHC-DG-P8-000  
**Phase:** 8 — Metadata and catalog  
**Status:** Implemented  
**Does not decide:** Catalog platform, UI, search architecture, automated or column-level lineage (Phase 9), or live inventory

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Status

**Implemented** — conceptual metadata and catalog **governance design** for the fictional Rafid Health Cluster `[A]`. No catalog product is implemented. No NDMO compliance is claimed.

This is **not** Microsoft Purview, Collibra, Atlan, Informatica, or any other tool build.

---

## Purpose

Phase 8 defines **how data is described, registered, discovered, and trusted as metadata** — without becoming a software implementation.

It consumes Phase 4 ownership, Phase 5 Rafid classification, Phase 6 **Metadata & Catalog Standard** and **Metadata Registration Procedure**, and Phase 7 quality concepts (for metadata-quality application only). It does **not** redesign those phases.

Data Catalog and Metadata is an NDMO knowledge-domain **name** (domain ID `MCM` as recorded in Phase 2) `[C]`. This phase is an entity design `[A][B]`. Specification-level NDMO metadata fields, categories, and catalog requirements remain `[NDMO verification required]`. **No control IDs are invented. No compliance is claimed.**

---

## Metadata lifecycle (locked)

```text
Identify data asset
→ Register
→ Describe
→ Classify
→ Assign ownership
→ Validate
→ Publish
→ Maintain
→ Review
→ Retire
```

Registration uses the existing Phase 6 procedure (not redesigned):

**Metadata Registration Procedure** — `06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`

---

## Metadata categories `[A][B]`

Seven Rafid categories. **Not** claimed as NDMO-required names.

| Group | Categories |
| --- | --- |
| **Mandatory** | Business; Governance; Security / Classification; Technical (minimum) |
| **Capability-dependent** | Quality; Operational; Lineage |

---

## Data asset model (locked)

```text
Data Domain → Data Asset → Data Structure / Object → Data Element
```

**Year-1 asset types:** Dataset · Table · Report · Dashboard · Master Data Entity  

**Deferred (not first-class Year-1 types):** API · Data Product

---

## Minimum metadata

**Mandatory / Recommended / Capability-dependent** `[A][B]`.

**System / Primary System** is **mandatory**. It identifies the primary or authoritative system **context where one applies**. It does **not** require exactly one source system. Derived, aggregated, or virtual assets may reference multiple contributing systems or none directly.

---

## Glossary and catalog

- **Business Glossary** holds terms (seven illustrative terms `[A]`).
- **Data Catalog** holds assets and governed metadata for discovery.
- Relationship: Glossary ↔ Catalog ↔ Data Assets.

Conceptual catalog only: purpose, personas, search dimensions, asset pages, certification. **No UI or technical search architecture.**

---

## Registration workflow (consistent with Phase 6)

```text
Identify → Submit metadata → Steward validation → Owner approval where required
→ DMO governance check → Publish → Maintain
```

---

## Metadata quality

**Data quality** asks whether the **data** is correct (Phase 7).  
**Metadata quality** asks whether the **description** is correct, complete, current, and governed.

Illustrative checks reuse Phase 7 names for **metadata** only: Completeness, Accuracy, Consistency, Timeliness, Validity. **Not** a second Data Quality Framework.

---

## Certification (internal trust)

Statuses: Registered · Reviewed · Certified · Deprecated · Retired.

**Proposed Rafid internal trust mechanism** `[A][B]`. **Not** regulatory, NDMO, or external compliance certification.

---

## Search / discovery

Dimensions: business term, domain, Owner, classification, quality/certification status, asset type, system, tags/keywords.

The catalog may expose **governed metadata** (name, Owner, classification, business definition). It must **not** expose underlying Restricted or Confidential **data**. Access remains Phase 4/5. No cybersecurity architecture in this phase.

---

## Lineage (conceptual)

```text
Source → Transformation → Target → Consumer
```

Coarse lineage may appear as metadata. Detailed, automated, and column-level lineage are designed in Phase 9 as a **governance framework** (not a tool). This Phase 8 folder was not redesigned.

---

## Domain application and MVP

All **eight** Phase 4 domains are covered. Steward examples use only **Business Data Steward** (no named operational titles).

**MVP scope:** Patient / Person Master; Clinical / Medical Records; Financial / Billing & Claims. Asset types: Dataset and Master Data Entity. Users: Data Owners, Business Data Stewards, DMO. Success indicators are **qualitative** (no numeric targets).

---

## Governance artifacts (proposed `[A][B]`)

Metadata Registry · Data Asset Registry · Business Glossary · Metadata Quality Report · Catalog Certification Register · Metadata Change Record · Metadata Exception Record

**Not** claimed as NDMO-mandated. Exceptions reuse the Phase 6 **Data Governance Exception Procedure** (no new exception procedure).

---

## Relationship to Phase 6

STD-004 remains the governance Standard. The Metadata Registration Procedure remains the registration path. Phase 8 adds operating design (model, minimum fields, catalog concept, MVP). **Owner A for domain meaning is unchanged.**

---

## Boundary with Phase 9

Phase 9 lineage framework lives in `09-data-lineage/`. This Phase 8 folder was **not** redesigned. Phase 8 still supplies Lineage Metadata fields and the asset hierarchy. Phase 9 does **not** implement automated or column-level tooling. **Phase 10 is Designed / Documented** as conceptual MDM (`10-master-data-management/`); operational implementation and measured performance are not claimed.

---

## NDMO verification limitations

Specific NDMO metadata fields, categories, and control-level catalog requirements remain `[NDMO verification required]`.

---

## Files

| Path | ID |
| --- | --- |
| [01-framework-overview.md](01-framework-overview.md) | RHC-DG-P8-001 |
| [02-metadata-categories.md](02-metadata-categories.md) | RHC-DG-P8-002 |
| [03-data-asset-model.md](03-data-asset-model.md) | RHC-DG-P8-003 |
| [04-minimum-metadata-standard.md](04-minimum-metadata-standard.md) | RHC-DG-P8-004 |
| [05-business-glossary.md](05-business-glossary.md) | RHC-DG-P8-005 |
| [06-data-catalog-design.md](06-data-catalog-design.md) | RHC-DG-P8-006 |
| [07-asset-registration-workflow.md](07-asset-registration-workflow.md) | RHC-DG-P8-007 |
| [08-metadata-quality.md](08-metadata-quality.md) | RHC-DG-P8-008 |
| [09-certification-trust-model.md](09-certification-trust-model.md) | RHC-DG-P8-009 |
| [10-search-discovery.md](10-search-discovery.md) | RHC-DG-P8-010 |
| [11-lineage-conceptual.md](11-lineage-conceptual.md) | RHC-DG-P8-011 |
| [12-metadata-ownership.md](12-metadata-ownership.md) | RHC-DG-P8-012 |
| [13-metadata-by-domain.md](13-metadata-by-domain.md) | RHC-DG-P8-013 |
| [14-catalog-mvp.md](14-catalog-mvp.md) | RHC-DG-P8-014 |
| [15-governance-artifacts.md](15-governance-artifacts.md) | RHC-DG-P8-015 |
| [16-interview-defensibility.md](16-interview-defensibility.md) | RHC-DG-P8-016 |
| [17-ndmo-alignment.md](17-ndmo-alignment.md) | RHC-DG-P8-017 |
