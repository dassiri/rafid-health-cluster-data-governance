# Governance RACI (Applied Working Pack)

**Document ID:** RHC-DG-P3-WP-004  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** New Accountable cells, dual-A rows, or a replacement enterprise RACI

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Authoritative sources (do not contradict):**  
[`../../04-enterprise-raci.md`](../../04-enterprise-raci.md) · [`../../../04-ownership-stewardship/03-ownership-decision-matrix.md`](../../../04-ownership-stewardship/03-ownership-decision-matrix.md) · Phase 6 procedures PRC-001–006

Machine-readable companion: [`governance-raci.csv`](governance-raci.csv).

---

## 1. Purpose

Apply the locked Phase 3 enterprise RACI and Phase 4 domain RACI to the Rafid governance activities used across Phases 5–14.

This file **extends** those matrices to named activities (classification packs, CDE confirmation, lineage registration, MDM, KPI review, NDMO evidence, PDPL privacy review). It does **not** replace `04-enterprise-raci.md`. Where a cell could be read two ways, the locked Phase 3 / Phase 4 **A** wins.

---

## 2. Legend and rules `[B]`

| Letter | Meaning |
| --- | --- |
| **R** | Responsible — does the work |
| **A** | Accountable — exactly **one** per row |
| **C** | Consulted — two-way input before the decision |
| **I** | Informed — told after the decision |

Rules reused from Phase 3:

- Exactly **one A per row**.
- Data Owners remain accountable for business meaning and quality of their domains.
- Business Data Stewards primarily execute and coordinate operational governance.
- IT / Data Custodians are responsible for technical implementation, not business ownership.
- IT is not Accountable for business data ownership by default.

Role codes match Phase 3: ESC, DMC, CDO, DGO, DO, BDS, CUST, PDPO, CO, LEG, ODIA, CON.

DMO in narrative = CDO + DGO. They are separate columns so CDO programme **A** is not silently moved onto DGO.

---

## 3. Applied RACI (18 activities)

Activities 1–15 are the required working-pack set. Activities 16–18 preserve locked splits that must not be collapsed (catalog content, lineage programme, in-policy waiver).

| ID | Activity | Single A | R | C | I | Locked source |
| --- | --- | --- | --- | --- | --- | --- |
| DG-RACI-WP-001 | Data Governance Framework (strategy) | **DMC** | CDO, DGO | ESC, DO, PDPO, CO, LEG, ODIA | BDS, CUST, CON | Phase 3: Governance strategy |
| DG-RACI-WP-002 | Data Policy approval (L3 / POL-001) | **DMC** | CDO, DGO | ESC, DO, CUST, PDPO, CO, LEG, ODIA | BDS, CON | Phase 3: Policy approval (L3) |
| DG-RACI-WP-003 | Enterprise Standard approval (does not change Policy intent) | **CDO** | DGO | DMC, DO, BDS, CUST | ESC, PDPO, CO, LEG, CON | Phase 6 document architecture: Standard approver = CDO; DMC **A** only if the standard would change Policy intent |
| DG-RACI-WP-004 | Data Ownership assignment (Owner ratification) | **DMC** | CDO, DGO | Proposed DO | CUST, PDPO, CO, BDS | PRC-001 |
| DG-RACI-WP-005 | Data Classification (dataset application) | **DO** | BDS | CDO, DGO, CUST, PDPO, LEG, ODIA† | ESC, DMC, CO, CON | Phase 3 dataset classification; Phase 4 row 3; PRC-002 |
| DG-RACI-WP-006 | Metadata registration (domain content) | **DO** | BDS | DGO, CUST, PDPO* | DMC, ESC, CO, CON | Phase 4 row 8; PRC-004 |
| DG-RACI-WP-007 | Data Quality issue management | **DO** | BDS, CUST | DGO, CON | ESC, DMC, PDPO, CO, LEG | Phase 3 issue row; Phase 4 row 9; PRC-003. CDO becomes additional **R** only after qualitative SLA-breach escalation — not a second **A**. |
| DG-RACI-WP-008 | Data Lineage registration (business meaning of a recorded flow) | **DO** | BDS | DGO, CUST | DMC, ESC, PDPO, CO | Phase 9 working pack: Owner **A** for business lineage correctness |
| DG-RACI-WP-009 | Data Catalog governance (programme + content rules) | **CDO** | DGO, BDS, CUST§ | DO | ESC, DMC, PDPO, CO, CON | Phase 3 catalog programme row |
| DG-RACI-WP-010 | CDE management (confirm or decline CDE status) | **DO** | BDS | CUST, DGO, PDPO‡ | DMC, ESC, CO | Phase 7 CDE methodology — Phase 4 quality pattern; no new RACI row |
| DG-RACI-WP-011 | MDM governance (master meaning, golden record, survivorship, match intent) | **DO** | BDS | CUST, DGO | DMC, ESC, PDPO, CO | Phase 10 MDM ownership; Phase 4 RACI unchanged |
| DG-RACI-WP-012 | Data Lifecycle decisions (domain application) | **DO** | BDS, CUST | DGO, PDPO, LEG | ESC, DMC, CO, CON | Phase 3 retention row; Phase 4 row 10 |
| DG-RACI-WP-013 | Governance KPI review / reporting | **CDO** | DGO, BDS | DO, CUST, CO | ESC, DMC, PDPO, CON | Phase 3 KPI reporting. DMC **reviews** the pack as an existing input; **no new DMC class**. |
| DG-RACI-WP-014 | Governance exceptions (to L3 policy) | **DMC** | CDO, DGO | ESC, DO, CUST, PDPO, CO, LEG, ODIA | BDS, CON | Phase 3 exceptions; PRC-006 |
| DG-RACI-WP-015 | NDMO evidence / alignment verification (self-assessment work) | **CDO** | CO, DGO | DO, PDPO, LEG, ODIA | ESC, DMC, BDS, CUST, CON | Phase 3 maturity / alignment self-assessment |
| DG-RACI-WP-016 | PDPL governance considerations — privacy compliance review of personal-data sharing | **PDPO** | PDPO (performs the review) | DO, BDS, DGO, CDO, LEG | DMC, ESC, CUST, CO, CON | Phase 4 row 7; PRC-005. **Not** a PDPL compliance claim. Business-sharing **A** stays on the Owner (separate row). Phase 4 lists no second **R**; PDPO remains the single **A**. |
| DG-RACI-WP-017 | Data Lineage programme (method, registry, technical capture completeness) | **CDO** | CUST | DO, BDS, DGO | ESC, DMC, PDPO, CO | Phase 3 lineage programme row — not merged with WP-008 |
| DG-RACI-WP-018 | Time-boxed operational waiver **inside** an already approved Policy envelope | **CDO** | DGO | DO, PDPO, LEG, CUST | DMC, ESC, BDS, CON | Phase 3 exception path; PRC-006. If the request is **outside** Policy, use WP-014 (**DMC = A**). |

**Notes**

\* PDPO **C** when the definition or metadata is personal/health identifying; otherwise **I**.  
† ODIA **C** when the likely classification/share outcome is Public / open data.  
‡ PDPO **C** when CDE confirmation has privacy/security impact.  
§ Custodian **R** for the catalog **tool**; CDO remains **A** for the catalog **programme**. BDS **R** for domain content under Owner **A** (WP-006).

---

## 4. Single-A confirmation

| ID | Single A | Why this is not a new right |
| --- | --- | --- |
| WP-001, WP-002, WP-004, WP-014 | DMC | Existing Phase 3 / PRC-001 / PRC-006 |
| WP-003, WP-009, WP-013, WP-015, WP-017, WP-018 | CDO | Existing Phase 3 programme rows and Phase 6 Standard approver |
| WP-005, WP-006, WP-007, WP-008, WP-010, WP-011, WP-012 | Data Owner | Existing Phase 4 domain rows / Phase 7 / Phase 9 / Phase 10 / Phase 11 |
| WP-016 | PDPO | Existing Phase 4 row 7 only |

No row has two Accountable roles.

Classification **method** remains a policy/standard item (**A = DMC** on WP-002, or CDO on WP-003 if the standard does not change Policy). Dataset **application** stays **A = Data Owner** (WP-005).

---

## 5. What this RACI is not

- Not a replacement of [`../../04-enterprise-raci.md`](../../04-enterprise-raci.md)
- Not a list of named incumbents
- Not a new DMC decision class
- Not NDMO specification evidence
- Not a PDPL legal RACI

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Phase 3 enterprise RACI; Phase 4 decision matrix; Phase 6 procedures | Cells |
| `[A]` | Rafid activity names used in later phases | Activity labels |
| `[C]` | NDMO role **names** | Column titles |
| `[NDMO verification required]` | Control-level duties; PDPL operationalization | Not used as IDs |
