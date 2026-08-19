# Phase 6 — Policies, Standards, and Procedures

**Document ID:** RHC-DG-P6-000  
**Phase:** 6 — Policies, standards, and procedures  
**Status:** Implemented  
**Architecture:** **1 Policy + 5 Standards + 6 Procedures**, plus Templates/Records as supporting artifacts `[A][B]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Status

**Implemented** — document bodies are written for the fictional Rafid Health Cluster `[A]`. No live DMC approval is claimed. This is not NDMO compliance.

Earlier wording of **1 Policy + 4 Standards + 6 Procedures** remains **withdrawn**. MDM is **STD-005**, standalone.

---

## Architecture

```text
L3  1 Policy      Enterprise Data Governance Policy
L4  5 Standards   Ownership · Classification · Quality · Metadata & Catalog · MDM (standalone)
L5  6 Procedures  Appointment · Classification · DQ issues · Metadata registration · Access/Sharing · Exception
    Supporting    Templates / Records (not extra policies)
```

Detail: [`00-document-architecture.md`](00-document-architecture.md).

---

## Relationship to Phase 3 — Operating Model

Phase 3 defined federated-by-domain operation, CDO reporting to Cluster CEO, CEO-chaired DMC, role types, enterprise RACI, and exception **A = DMC**. This Policy **binds** that model. It does not redesign reporting lines or forums.

---

## Relationship to Phase 4 — Ownership & Stewardship

Phase 4 assigned eight domains and one Data Owner each. **STD-001** and **PRC-001** consume that map unchanged. DMO does not become a business Data Owner.

---

## Relationship to Phase 5 — Data Classification

Phase 5 defined Rafid tiers **Public / Internal / Confidential / Restricted** `[A][B]`, dataset-level application, and Owner approval. **STD-002** and **PRC-002** consume that framework. Those tiers are **not** NDMO national classification tiers `[NDMO verification required]`.

Restricted external sharing remains exactly:

**Requires Data Owner business approval + PDPO privacy compliance review where personal data is involved**

---

## Boundaries with later phases

| Phase | Boundary |
| --- | --- |
| **7 Data Quality** | STD-003 and the Data Quality Issue Management Procedure remain the governance parent. Dimensions, CDEs, rules, and measurement live in `07-data-quality/` (Phase 7 implemented). This Phase 6 folder was not redesigned. |
| **8 Metadata & Catalog** | STD-004 and the Metadata Registration Procedure remain the governance parent. Operating design (model, minimum fields, conceptual catalog, MVP) lives in `08-metadata-catalog/` (Phase 8 implemented). This Phase 6 folder was not redesigned. **No catalog product.** |
| **9 Data Lineage** | STD-004 still names conceptual source/system class. Lineage **framework** lives in `09-data-lineage/` (Phase 9 implemented). This Phase 6 folder was not redesigned. No lineage product. |
| **10 MDM** | STD-005 remains the standalone governance Standard. Conceptual MDM operating design lives in `10-master-data-management/` (Phase 10 implemented). This Phase 6 folder was not redesigned. **No matching engine, hub, or vendor MDM.** |

---

## Files

| Path | ID |
| --- | --- |
| [policy/enterprise-data-governance-policy.md](policy/enterprise-data-governance-policy.md) | RHC-DG-POL-001 |
| [standards/01-data-ownership-stewardship-standard.md](standards/01-data-ownership-stewardship-standard.md) | RHC-DG-STD-001 |
| [standards/02-data-classification-standard.md](standards/02-data-classification-standard.md) | RHC-DG-STD-002 |
| [standards/03-data-quality-standard.md](standards/03-data-quality-standard.md) | RHC-DG-STD-003 |
| [standards/04-metadata-catalog-standard.md](standards/04-metadata-catalog-standard.md) | RHC-DG-STD-004 |
| [standards/05-master-data-management-standard.md](standards/05-master-data-management-standard.md) | RHC-DG-STD-005 |
| [procedures/01-data-ownership-appointment-procedure.md](procedures/01-data-ownership-appointment-procedure.md) | RHC-DG-PRC-001 |
| [procedures/02-data-classification-procedure.md](procedures/02-data-classification-procedure.md) | RHC-DG-PRC-002 |
| [procedures/03-data-quality-issue-management-procedure.md](procedures/03-data-quality-issue-management-procedure.md) | RHC-DG-PRC-003 |
| [procedures/04-metadata-registration-procedure.md](procedures/04-metadata-registration-procedure.md) | RHC-DG-PRC-004 |
| [procedures/05-data-access-sharing-governance-procedure.md](procedures/05-data-access-sharing-governance-procedure.md) | RHC-DG-PRC-005 |
| [procedures/06-data-governance-exception-procedure.md](procedures/06-data-governance-exception-procedure.md) | RHC-DG-PRC-006 |
| [templates-records/README.md](templates-records/README.md) | Catalogue only |
| [interview-preparation.md](interview-preparation.md) | INTERNAL / INTERVIEW PREPARATION |

No NDMO control IDs are used in this folder. No compliance claim is made.
