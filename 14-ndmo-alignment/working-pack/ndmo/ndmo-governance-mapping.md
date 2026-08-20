# NDMO Governance Mapping

**Document ID:** RHC-DG-P14-WP-001  
**Phase:** 14 — NDMO alignment (working pack)  
**Status:** Implemented (conceptual mapping only)

**Does not decide:** That any Rafid artifact is NDMO-mandated, implemented, or compliant

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

**Responsible:** DMO · **Review:** CDO · **Approval:** CDO (method only)

---

## 1. Purpose

Map **existing** Rafid governance artifacts to NDMO **domain / knowledge-area names** already recorded in this repository (Phase 2; Phase 14 `02-ndmo-domain-map.md` and `03-artifact-to-domain-map.md`).

This file extends that locked map to include later **working-pack** evidence (Phase 8 metadata inventory; Phase 9 lineage register). It does **not** duplicate or replace those files.

**Alignment is not compliance.**

---

## 2. Mapping rules

1. Use only domain names from NDMO Standards v1.5 as recorded in Phase 2 `[C]`.
2. Use domain IDs only where already recorded: `DG`, `MCM`, `DC`. All others: `[NDMO verification required]`.
3. Do not invent control IDs, specification IDs, or mandatory field lists.
4. Evidence Status is a **project** evidence state (Designed / Operational / Measured). It is not an NDMO assessment score.
5. Where specification-level confirmation is open: **`[NDMO verification required]`**.

---

## 3. Relationship types (governance, not legal)

| Relationship | Meaning |
| --- | --- |
| Conceptual alignment | Rafid artifact addresses the same **theme** as the NDMO domain **name** `[C]` |
| Pointer only | Domain/control **name** is used as a pointer; Rafid design is `[A][B]` |
| Boundary | Rafid records a limit (for example Records Management not built) |
| Coordination | Rafid coordinates; another authority owns the control set (NCA for Domain 15) |
| Not produced | No Rafid artifact in this repository |

---

## 4. Mapping table (20 rows)

Evidence Status = strongest **project** state justified by files in this repository. Organizational Operational / Measured remain **not claimed** (Phase 14).

| Artifact | Rafid Governance Area | Relevant NDMO Domain / Knowledge Area | Relationship | Evidence Available | Evidence Status | Verification Status | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Governance strategy pack (vision, mission, objectives, principles, alignment method) | Data Governance Strategy | Data Governance (`DG`) `[C]` | Conceptual alignment to `DG.1` **name**; contents not claimed complete vs `DG.1.1` | Yes — `02-governance-strategy/` | Designed | Conceptually aligned; full `DG.1` text `[NDMO verification required]` | Phase 14 `RHC-VER-001`–`002` remain open |
| Federated operating model, forums, enterprise RACI | Stakeholder Governance | Data Governance (`DG`) `[C]` | Conceptual alignment to `DG.4` **names**; Rafid RACI is `[A][B]` | Yes — `03-operating-model/` | Designed | Conceptually aligned; Organizational Manual `[NDMO verification required]` | DMC composition is `[A]`, not claimed NDMO-mandated |
| Enterprise Data Governance Policy + 5 Standards + 6 Procedures | Policies and Standards | Data Governance (`DG`) `[C]` | Pointer to `DG.2` **name**; stack shape is `[A][B]` | Yes — `06-policies-standards-procedures/` | Designed | Conceptually aligned; `DG.2.1` / `DG.2.2` full text `[NDMO verification required]` | `DG.2.1` gap analysis was not produced as an official NDMO file |
| Domain ownership matrix (8 domains, 8 Owner titles) | Data Ownership | Data Governance (`DG`) `[C]` | Conceptual alignment to Business Data Executive / Steward **names** `[C]` | Yes — `04-ownership-stewardship/` | Designed | Conceptually aligned; duty-level mapping `[NDMO verification required]` | Ownership Registry schema exists; named appointments not claimed |
| Rafid Public / Internal / Confidential / Restricted model | Data Classification | Data Classification (`DC`) `[C]` | Pointer to four-level **concept** `[C]`; Rafid **names** are `[A][B]` | Yes — `05-data-classification/` | Designed | Conceptually aligned; official national **names** `[NDMO verification required]` | Do not equate Rafid Restricted with any NDMO tier name |
| Data Quality Framework, 7 dimensions, 13 CDEs | Data Quality | Data Quality `[C]` (domain ID not copied) | Conceptual alignment to domain **name** | Yes — `07-data-quality/`; illustrative sample in `assets/practical-evidence/01-data-quality-example.md` | Designed | Conceptually aligned; official dimensions/thresholds `[NDMO verification required]` | Sample scores are illustrative; **Measured** is not assigned |
| Metadata Management working pack (inventory, field model, glossary) | Metadata Management | Data Catalog and Metadata (`MCM`) `[C]` | Conceptual alignment to `MCM` **name** | Yes — `08-metadata-catalog/working-pack/` (20-asset inventory; 25-term glossary) | Operational (project) | Conceptually aligned; official MCM fields `[NDMO verification required]` | Synthetic records only; not a production catalog |
| Data Catalog design + sample catalog pages | Data Catalog | Data Catalog and Metadata (`MCM`) `[C]` | Conceptual alignment to `MCM` **name** | Yes — Phase 8 design + `working-pack/examples/sample-catalog-assets.md` | Operational (project) | Conceptually aligned; catalog control IDs not copied `[NDMO verification required]` | Publish is not an access grant |
| Data Lineage working pack (13-row register, business/conceptual maps) | Data Lineage | Data Catalog and Metadata (`MCM`) `[C]` | Conceptual alignment as lineage **metadata**; lineage is not a separate NDMO domain name in the Phase 2 list | Yes — `09-data-lineage/working-pack/` | Operational (project) | Conceptually aligned; specific lineage requirements `[NDMO verification required]` | Do not invent a lineage control ID |
| MDM Standard, entity model, golden-record example | Master Data Management | Reference and Master Data Management `[C]` (domain ID not copied) | Conceptual alignment to domain **name** | Yes — `10-master-data-management/`; sample in `assets/practical-evidence/04-mdm-golden-record-example.md` | Designed | Conceptually aligned; official MDM specifications `[NDMO verification required]` | Golden-record file is a worked example, not an operating hub |
| Lifecycle framework; retention decision chain; holds | Data Lifecycle | Data Governance — `DG.6` **name** `[C]`; Document and Content Management **boundary** `[C]` | Pointer to `DG.6` **name** (plan review / communications — not treated as a retention spec pack); Records Management **not built** | Yes — `11-data-lifecycle/` | Designed | Conceptually aligned; retention/archive specs `[NDMO verification required]` | Periods are placeholders; not invented |
| Access / Sharing procedure (two Accountable decisions) | Access Governance | Data Sharing and Interoperability `[C]` (domain ID not copied) | Conceptual alignment to domain **name**; Owner business **A** + PDPO privacy **A** | Yes — `06-policies-standards-procedures/procedures/05-data-access-sharing-governance-procedure.md` | Designed | Conceptually aligned; Sharing Regulation `[NDMO verification required]` | Dual **A** is Rafid design `[A][B]` using PDPO **name** `[C]` |
| PDPO role and personal-data sharing review | Privacy Governance | Personal Data Protection `[C]` (domain ID not copied) | Conceptual alignment to domain **name** and PDPO **name** `[C]` | Yes — Phase 3 role catalogue; PRC-005; this pack `pdpl/` | Designed | Conceptually aligned; PDPL overlay `[NDMO verification required]` / `[Legal / regulatory verification required]` | PDPO ≠ claimed PDPL DPO |
| KPI catalogue (`DG-KPI-001`–`012`) and empty maturity template | Governance KPIs | Data Governance — `DG.7` **name** `[C]` | Pointer to Performance Management **name**; Rafid KPIs are `[A]` | Yes — `12-kpis-maturity/` | Designed | Conceptually aligned; official KPI types `[NDMO verification required]` | No live KPI results; `DG-KPI-00n` are not NDMO IDs |
| Illustrative three-year roadmap | Implementation Planning | Data Governance — `DG.1.3` **name** `[C]` | Pointer only | Yes — `13-implementation-roadmap/` | Designed | Conceptually aligned; 3-year plan specifications `[NDMO verification required]` | Documentation/design only; not an NDMO-required sequence |
| Phase 14 alignment pack + this working pack | NDMO Alignment / Evidence | Data Governance (`DG`) `[C]` | Conceptual alignment of method; this pack is not `DG.5` | Yes — `14-ndmo-alignment/` | Designed (locked pack); Operational (project) for this pack’s working records | Conceptually aligned; assessment evidence rules `[NDMO verification required]` | This pack ≠ Compliance Audit Framework (`DG.5` **name**) |
| Open by Default principle **name**; ODIA named | Open Data (principle only) | Open Data `[C]` (domain ID not copied) | Pointer to principle and domain **names** | Partial — principle adopted as **name** in Phase 1–3 | Designed | Conceptually aligned; Open Data regulation `[NDMO verification required]` | Not a Year-1 standing DMC operating programme |
| Custodian **R** and operational forums | Data Operations (partial theme) | Data Operations `[C]` (domain ID not copied) | Partial theme only; no dedicated operations phase | Partial — Phase 3–4 design | Designed | Verification required for the full control set `[NDMO verification required]` | Not claimed as Domain coverage |
| Conceptual dashboard specification | Measurement presentation | Business Intelligence and Analytics `[C]` (domain ID not copied) | Not a BI programme | Partial — Phase 12 dashboard spec only | Designed | Verification required for the domain `[NDMO verification required]` | Dashboard spec ≠ BI/analytics operating model |
| Security coordination statement (no NCA catalogue) | Security coordination | Data Security and Protection (NCA) `[C]` | Coordination only | Boundary statement in Phases 2–5, 14 | Designed (boundary) | NCA control set `[NDMO verification required]` — do not invent NCA IDs | Domain 15 is NCA, not a Rafid control list |

**Not produced in this repository (recorded so they are not implied):** Freedom of Information; Data Architecture and Modeling; Data Value Realization. Domain **names** are `[C]`; entire control sets remain `[NDMO verification required]`.

---

## 5. What this mapping is not

- Not a specification-level control matrix
- Not an NDMO self-assessment
- Not a claim that Rafid artifacts are NDMO-mandated artifacts
- Not permission to invent `MCM.n`, quality control IDs, or MDM control IDs

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | Phase 2 / Phase 14 domain and control **names** already recorded | Domain column |
| `[A][B]` | Rafid artifact list and working packs | Artifact column |
| `[NDMO verification required]` | Uncopied IDs; regulations not retrieved; specification text | Verification Status |
