# Master Data Management Standard

**Document ID:** RHC-DG-STD-005  
**Version:** 1.0  
**Status:** Implemented (documentation) — **governance-level only**; **standalone Standard**  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Standalone MDM Standard; Phase 10 technical MDM not built.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent policy:** RHC-DG-POL-001  

This Standard is **not** a subsection of STD-004. Reference and Master Data Management is an NDMO knowledge-domain **name** `[C]`. This Standard does **not** implement that domain. **No** matching algorithms, survivorship engines, hub architecture, or vendor MDM. **Phase 10 is Designed / Documented** (conceptual MDM in `10-master-data-management/`; this Standard remains the governance parent). Operational implementation and measured performance are not claimed. No control IDs. No compliance claim.

---

## 1. Purpose

State **governance** requirements for master and reference data so identity and shared lists do not fragment by hospital `[B]`.

---

## 2. Master data definition `[B]`

**Master data** is data about core business entities that must be consistent across processes (for Rafid, typically Person/Patient, Provider/Clinician, and organizational reference structures `[A]` from Phases 0 and 4). **Reference data** is permitted value lists and structural codes (for example facility hierarchy) owned under Reference / Organizational Master Data.

This Standard does not publish an MDM object model (Phase 10).

---

## 3. Master data ownership

Master-data **objects** inherit **domain** ownership from STD-001. Examples `[A]`:

| Master / reference grouping | Data Owner |
| --- | --- |
| Patient / Person | Patient Access & Experience Director |
| Provider / Clinician | Medical Affairs Officer |
| Organizational reference (facilities, org units) | Strategy & Planning Director |

IT is **not** Owner of these objects. One Owner per domain still applies; MDM does not create a second **A**.

---

## 4. Stewardship

Business Data Stewards execute identity and list hygiene under the Owner. Custodians implement MPI/EMR/ERP behaviour. DMO coordinates cross-domain clashes; DMO is not the Person Owner because a PMO analyst stewards org reference data.

---

## 5. Golden / source-of-truth principles `[B]`

- Each master entity type **shall** have an Owner-recognized **authoritative meaning**
- Systems may **store** copies; they shall not silently become a competing business definition
- “Golden record” here means **governed authority**, not a physical MDM hub (Phase 10)

---

## 6. Duplicate management `[B]`

Duplicate or split identities **shall** be treated as **data issues** (PRC-003) under the owning domain. Survivorship **rules engines** are Phase 10. Until then, the Owner decides business merge/split **intent**; Custodian implements in systems.

---

## 7. Cross-domain consistency

Joins (person–encounter–clinician–charge) **shall not** create a second Person Owner `[B]`. Clinical Owner owns record **content**; Patient Access owns **identity**; Medical Affairs owns **practitioner** master (Phase 4). Clashes escalate via DMO.

---

## 8. Change governance

Changes to master definitions or org reference structures follow Owner approval (STD-001 decision rights) and metadata registration (PRC-004) when a dataset is affected. Ownership **title** changes follow PRC-001.

---

## 9. Reference data relationship

Organizational reference data is Domain 8 (Strategy & Planning Director). Item/vendor masters remain Supply Chain (STD-001). This Standard does not move those Owners.
