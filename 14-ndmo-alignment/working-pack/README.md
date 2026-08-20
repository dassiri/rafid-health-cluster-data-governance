# Compliance & Risk — Working Pack

**Document ID:** RHC-DG-P14-WP-000  
**Phase:** 14 — NDMO alignment and evidence (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

This folder is the **applied Compliance & Risk working pack** inside the existing Rafid Health Cluster Data Governance project. It sits under Phase 14 so the repository numbering stays intact. Locked Phase 14 alignment files are **not** rewritten.

**No NDMO or PDPL compliance is claimed.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

Show how existing Rafid governance artifacts can be:

1. mapped conceptually to relevant NDMO domains already named in this repository;
2. evaluated for **project** evidence status;
3. distinguished as **Designed**, **Operational**, or **Measured**;
4. assessed for verification requirements;
5. connected to PDPL and other regulatory inputs as **governance considerations**;
6. tracked through a synthetic governance risk register.

This pack **connects** Phases 0–14. It does **not** rebuild ownership, classification, quality, metadata, catalog, lineage, MDM, lifecycle, KPIs, or the locked Phase 14 alignment files.

```text
Existing Governance Artifacts
          ↓
Compliance / Risk Mapping
          ↓
Evidence State
          ↓
Verification
          ↓
Risk / Gap
```

Pattern used throughout:

**Claim → Evidence → Verification → Status**

---

## 2. Relationship to Phase 14

Phase 14 is the locked **NDMO Alignment & Evidence** design pack:

- alignment method
- domain map
- artifact-to-domain map
- evidence inventory
- evidence status model
- control and gap verification registers

This pack is **applied evidence** of how those designs are used when later working records exist (Phase 8 metadata inventory, Phase 9 lineage register, practical-evidence samples).

Locked files remain authoritative for:

- official NDMO **names** and recorded IDs `[C]`
- organizational evidence claim (**Designed** only; Operational / Measured **not claimed** for a real organization)
- unresolved `[NDMO verification required]` and `[Legal / regulatory verification required]` items

This pack does **not** replace `01`–`20` in the parent folder. It does **not** certify compliance. It does **not** introduce new governance roles or DMC decision rights.

---

## 3. Compliance & Risk scope

In scope:

- Conceptual NDMO domain mapping of Rafid artifacts
- Project evidence-state audit (Designed / Operational / Measured)
- Evidence and verification matrix
- NDMO verification register (working-pack layer)
- PDPL as a **governance input** (not legal advice)
- Data Governance / Data Management risk register
- Gap analysis tied to actual Rafid artifacts
- Traceability from claim to evidence to verification

Out of scope:

- NDMO certification or self-assessment score
- PDPL legal interpretation or certification
- NCA control catalogue
- Invented NDMO control IDs, mandatory fields, or specification text
- Production regulatory implementation
- New Data Owner domains or new governance forums

---

## 4. NDMO mapping

Conceptual mapping lives in [`ndmo/ndmo-governance-mapping.md`](ndmo/ndmo-governance-mapping.md).

It uses **only** NDMO domain / knowledge-area **names** already recorded from Standards v1.5 (Phase 2 / Phase 14). Domain IDs appear only where already recorded (`DG`, `MCM`, `DC`). Other domain IDs remain `[NDMO verification required]`.

**20** artifact-to-domain rows. Relationship types are governance relationships (conceptual alignment, boundary, coordination, not produced). They are **not** official control mappings unless the source is already `[C]` in this repository.

---

## 5. Evidence states

This pack uses the same three names as Phase 14 [`05-evidence-status-model.md`](../05-evidence-status-model.md). They are **project evidence states**. They are **not** official NDMO maturity or compliance statuses. They are **not** the NDMO annual specification-level assessment `[C]` (which Rafid has **not** performed).

| Project evidence state | Meaning in this pack | Organizational claim (Phase 14, unchanged) |
| --- | --- | --- |
| **Designed** | The governance artifact, framework, policy, process, or model is documented in this repository | **Yes** for Phases 0–14 |
| **Operational** | The artifact has been **applied** inside this synthetic portfolio (working records, inventories, registers, sample catalog/lineage pages) | **Not claimed** for a real operating organization |
| **Measured** | Repeatable performance evidence exists (KPI results, quality trend, maturity score, before/after measurement) | **Not claimed** |

**Strongest supported project states in this repository today:**

- Most frameworks, policies, RACI, classification, MDM, lifecycle, KPIs, PDPL considerations: **Designed**
- Metadata inventory, catalog sample pages, lineage register: **Operational** (project / synthetic application only)
- **Measured:** not assigned to any major artifact (no KPI results, no maturity score, no quality trend). The Phase 7 scorecard and `assets/practical-evidence/01-data-quality-example.md` contain **illustrative** numbers only.

See [`evidence/evidence-state-audit.md`](evidence/evidence-state-audit.md).

---

## 6. Verification approach

Verification statuses used in this pack (project language — **not** “compliant”):

| Status | Meaning |
| --- | --- |
| **Verified from project source** | The statement is true of this repository (file exists; role name matches Phase 3–4; recorded NDMO **name**/ID is already `[C]`) |
| **Conceptually aligned** | Rafid design addresses the same **theme** as an NDMO domain **name** `[C]`; specification-level fit is not confirmed |
| **Verification required** | Official source text, current version, or legal overlay is not available to this project |
| **Illustrative assumption** | Fictional Rafid design `[A]` or industry practice `[B]`, labelled as such |

Evidence matrix: [`ndmo/ndmo-evidence-matrix.csv`](ndmo/ndmo-evidence-matrix.csv) (**22** rows).  
Verification register: [`ndmo/ndmo-verification-register.csv`](ndmo/ndmo-verification-register.csv) (**18** items).

Where official source-level confirmation is open, the pack writes **`[NDMO verification required]`** or **Verification required**. It does **not** invent NDMO control IDs.

---

## 7. PDPL governance considerations

[`pdpl/pdpl-governance-considerations.md`](pdpl/pdpl-governance-considerations.md) treats PDPL as an **L0 governance input** (Phase 2 policy hierarchy). It is **not** legal advice and **not** a PDPL implementation.

**11** considerations: Personal Data, Classification, Ownership, Access, Lifecycle, Retention, Minimization, Purpose / use, Sharing, Quality / accuracy, Accountability.

Evidence matrix: [`pdpl/pdpl-evidence-matrix.csv`](pdpl/pdpl-evidence-matrix.csv).

Wording used: governance consideration · conceptual control consideration · requires legal / official verification.

Wording **not** used: “PDPL compliant.”

---

## 8. Risk register

[`risk/compliance-risk-register.csv`](risk/compliance-risk-register.csv) is a **synthetic Data Governance / Data Management** risk register (**12** risks).

It is an **illustrative** qualitative method (High / Medium / Low). It is **not** an official enterprise risk methodology, **not** ISO 31000, **not** COSO, and **not** an NDMO-mandated risk catalogue.

It does **not** replace the Phase 13 implementation-roadmap risks (`13-implementation-roadmap/16-risk-register.md`). That register covers transformation delivery. This register covers governance evidence, verification, and operating-design risks.

---

## 9. Gap analysis

[`risk/governance-gap-analysis.md`](risk/governance-gap-analysis.md) records Rafid-specific gaps:

- Designed → Operational
- Operational → Measured
- Conceptual alignment → official verification

---

## 10. Traceability

[`traceability/governance-evidence-traceability.md`](traceability/governance-evidence-traceability.md) traces major claims to artifacts, working-pack evidence, and verification status.

[`traceability/governance-control-mapping.md`](traceability/governance-control-mapping.md) maps Rafid capabilities to **governance** considerations (not legal requirements).

---

## 11. File structure

```text
14-ndmo-alignment/working-pack/
├── README.md
├── ndmo/
│   ├── ndmo-governance-mapping.md
│   ├── ndmo-evidence-matrix.csv
│   └── ndmo-verification-register.csv
├── pdpl/
│   ├── pdpl-governance-considerations.md
│   └── pdpl-evidence-matrix.csv
├── risk/
│   ├── compliance-risk-register.csv
│   └── governance-gap-analysis.md
├── evidence/
│   └── evidence-state-audit.md
└── traceability/
    ├── governance-evidence-traceability.md
    └── governance-control-mapping.md
```

---

## 12. Ownership (existing roles only)

No new roles. Responsible / Review / Approval use the Phase 3 catalogue.

| Working-pack artifact | Responsible | Review | Approval (existing rights only) |
| --- | --- | --- | --- |
| Pack method and registers | DMO | CDO | CDO for method; DMC only if an existing policy/exception class is invoked |
| NDMO mapping / evidence matrix | DMO | CDO | CDO |
| Verification register | DMO | CDO; Compliance Officer (process) | CDO |
| PDPL considerations | DMO (governance design) | PDPO; Legal Advisor | Not a legal approval. CDO accepts the file as a governance input |
| Risk register | DMO | CDO; Compliance Officer | CDO; DMC for residual risk already in the Phase 3 decision-right framework |
| Domain content referenced by any row | Data Owner **A** | Business Data Steward **R** | Data Owner **A** (in-policy) |

IT / Data Custodian remains technical implementation only. Governance Forum names reused: Data Management Committee, Steward Forum. Secretariat remains DGO (non-member).

---

## 13. Limitations

- Synthetic / illustrative / non-production.
- Does not rewrite locked Phase 14 files.
- Does not populate a live Ownership, Classification, or Retention registry.
- Does not produce KPI results or a maturity score.
- Does not retrieve NDMO regulations that Phase 2 recorded as not retrieved.
- Does not interpret PDPL articles (none are copied in this repository).

---

## 14. NDMO verification limitations

Official source used in this repository `[C]`: NDMO *Data Management and Personal Data Protection Standards*, Version 1.5, January 2021 (as recorded in Phase 2).

Not retrieved: Organizational Manual; Classification Regulation; Sharing Regulation; FOI Regulation; control/specification text not already recorded.

**Do not invent NDMO control IDs.** Uncopied IDs and exact requirement text remain **`[NDMO verification required]`**.

Whether v1.5 remains the binding text for a live 2026 program remains **`[NDMO verification required]`**.

---

## 15. PDPL limitations

PDPL is named as an L0 example in the Phase 2 policy hierarchy. This pack does **not**:

- cite PDPL article numbers (not present in project sources);
- equate PDPO with a PDPL DPO (`[NDMO verification required]` / `[Legal / regulatory verification required]`);
- claim personal-data handling is lawful;
- produce a Record of Processing, DPIA, or legal basis assessment.

---

## 16. Portfolio disclaimer

This is a fictional portfolio project.

It does **not** claim legal compliance, NDMO certification, PDPL compliance, NCA compliance, a successful regulatory audit, production deployment, real patient data, or a real healthcare implementation.

Rafid Health Cluster is fictional.

**Synthetic / Illustrative / Non-production portfolio project.**  
**No NDMO or PDPL compliance is claimed.**
