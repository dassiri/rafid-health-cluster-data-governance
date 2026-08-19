# Metadata & Catalog Standard

**Document ID:** RHC-DG-STD-004  
**Version:** 1.0  
**Status:** Implemented (documentation) — **governance-level only**  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Governance requirements only; Phase 8 catalog design not built.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent policy:** RHC-DG-POL-001  
**Procedure:** RHC-DG-PRC-004  

Data Catalog and Metadata is an NDMO knowledge-domain **name** `[C]`. This Standard does **not** implement that domain, select a platform, or define a technical metadata model. **Do not** implement Microsoft Purview, Collibra, Atlan, or any other catalog product in this programme drop. **Phase 8 is Designed / Documented** (conceptual catalog in `08-metadata-catalog/`; this Standard remains the governance parent). Operational implementation and measured performance are not claimed. No control IDs. No compliance claim.

---

## 1. Purpose

Require that operational datasets have **governed business metadata** and are **registered** `[B]`.

---

## 2. Metadata ownership

| Subject | A | R |
| --- | --- | --- |
| Domain **meaning** / business definition | Data Owner | Steward |
| Catalog **programme and methodology** | CDO / DMO | DMO |
| Catalog **tool** (when one exists) | CDO (programme) | Custodian (platform) — Phase 8 |
| Dataset classification **value** | Data Owner | Steward (STD-002) |

DMO does not own clinical or finance meaning by running the register.

---

## 3. Business definitions

Each registered dataset **shall** have a business definition the Owner accepts `[B]`. Definitions are not system field lists (Phase 8). PDPO is **C** when the definition is personal/health-identifying (Phase 4).

---

## 4. Metadata registration

Operational datasets **shall** be registered per PRC-004 and linked to domain, Owner, Steward, and Rafid classification `[A][B]`. Registration is evidence; it is not a catalog product.

---

## 5. Catalog governance `[B]`

- One governed list of datasets is the aim; shadow spreadsheets are not the catalogue of record
- DMO oversees completeness and consistency
- Consumers should be directed to registered sources (POL-001)

---

## 6. Minimum governance expectations

For a dataset in operational use: name, domain, Owner, Steward, business definition, Rafid classification, related system class, registration status. Fine-grained technical metadata is Phase 8.

---

## 7. Relationship to lineage

Stewards **should** record, at a conceptual level, the **system or source class** that produces the dataset `[B]`. End-to-end technical lineage, tooling, and critical-flow graphs are **Phase 9 — not this Standard**.

---

## 8. Relationship to PRC-004 and Phase 8

PRC-004 is the registration process. Phase 8 may add a catalog operating model **without** changing Owner **A** for meaning.
