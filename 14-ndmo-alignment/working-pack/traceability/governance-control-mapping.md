# Governance Control / Artifact Mapping

**Document ID:** RHC-DG-P14-WP-006  
**Phase:** 14 — NDMO alignment (working pack)  
**Status:** Implemented (governance relationships only)

**Does not decide:** Legal requirements, NDMO-mandated controls, or NCA controls

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

**Responsible:** DMO · **Review:** CDO; PDPO (privacy rows) · **Approval:** CDO (method)

---

## 1. Purpose

Map existing Rafid **governance artifacts** to **compliance / risk considerations**.

These are **governance relationships**. They are **not** presented as direct legal requirements unless an official source is already `[C]` in this repository. Where that is not true: **verification required**.

---

## 2. Relationship map

```text
Data Classification
        ↓
Security / Privacy governance consideration
(handling band; PDPO consult if personal; NCA implements security — not this pack)

Data Ownership
        ↓
Accountability
(one business Owner per domain; Custodian is never Owner)

Metadata Management
        ↓
Data discovery / governance evidence
(mandatory fields; personal-data indicator; catalog publish)

Data Lineage
        ↓
Traceability / impact analysis
(source → transformation → target → consumer)

Data Quality
        ↓
Accuracy / reliability considerations
(seven dimensions; 13 CDEs; issues — not a PDPL accuracy certification)

Data Lifecycle
        ↓
Retention / disposal governance considerations
(purpose-driven retention; holds; no invented periods)

Access / Sharing (PRC-005)
        ↓
Dual accountability consideration
(Owner business A; PDPO privacy A where personal)

KPIs / Maturity
        ↓
Measurement discipline
(definitions without fabricated results)
```

---

## 3. Mapping table

| Rafid artifact | Governance consideration | Risk if the artifact is weak | Related evidence state | Legal / official requirement? |
| --- | --- | --- | --- | --- |
| Classification model (Phase 5) | Security / privacy handling band | Inconsistent access and sharing | Designed | No — national names `[NDMO verification required]`; PDPL overlay `[Legal / regulatory verification required]` |
| Ownership matrix (Phase 4) | Accountability | Unclear decisions and issue closure | Designed | No — BDE **name** `[C]`; duties `[NDMO verification required]` |
| Metadata working pack (Phase 8) | Discovery and evidence completeness | Assets cannot be found or governed | Operational (project) | No — `MCM` **name** `[C]`; fields `[NDMO verification required]` |
| Lineage working pack (Phase 9) | Traceability and impact analysis | Downstream effects of a change or defect are unknown | Operational (project) | No — lineage specs `[NDMO verification required]` |
| Data Quality framework (Phase 7) | Accuracy / reliability | Wrong identifiers and reports | Designed | No — domain **name** `[C]`; specs `[NDMO verification required]` |
| Lifecycle / retention (Phase 11) | Retention / disposal | Over-retention or unverifiable destruction | Designed | No — periods `[Legal / regulatory verification required]` / `[NDMO verification required]` |
| PRC-005 sharing | Access and sharing accountability | Single-signature sharing of personal data | Designed | No — Sharing Regulation `[NDMO verification required]` |
| PDPO seat (Phase 3) | Privacy review path | Privacy and business approvals collapse | Designed | PDPO **name** `[C]`; PDPL DPO equivalence verification required |
| This verification register | Regulatory honesty | Portfolio overstates alignment | Operational (project) as a gap register | Open items remain `[NDMO verification required]` |
| KPI catalogue (Phase 12) | Measured performance discipline | Fake percentages | Designed | `DG.7` **name** `[C]`; types `[NDMO verification required]` |

---

## 4. Roles on this mapping (existing only)

| Role | Duty here |
| --- | --- |
| Data Owner | **A** for domain classification, quality, sharing business approval, lifecycle |
| Business Data Steward | **R** for packs, metadata, lineage records, issue investigation |
| DMO | Method, registers, evidence discipline |
| IT / Data Custodian | Technical implementation after a business decision |
| PDPO | **A** on sharing privacy review; **C** on personal-data classification and retention |
| Compliance Officer | Reviews data-management compliance **process**; does not replace Internal Audit |
| Data Management Committee | Existing strategy / policy / material exception rights only |
| Governance forums (Steward Forum) | Practice; not a new Council |

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Rafid capability chain | Entire map |
| `[C]` | Domain and role **names** already recorded | Pointers only |
| `[NDMO verification required]` / `[Legal / regulatory verification required]` | Anything presented as a requirement | Last column |
