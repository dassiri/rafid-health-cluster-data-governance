# Stakeholder Management — Working Pack

**Document ID:** RHC-DG-P3-WP-000  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

This folder is the **applied Stakeholder Management working pack** inside the existing Rafid Health Cluster Data Governance project. It sits under Phase 3 so the repository numbering stays intact. Locked Phase 3 design files (`01`–`09` and diagrams) are **not** rewritten.

**No live stakeholder programme is claimed.**  
**No officers are appointed. No forums have met.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

Show how the locked Rafid governance model operates across:

- Data Owners
- Business Data Stewards
- Data Management Committee
- DMO (CDO and Data Governance Officer)
- IT / Data Custodian
- Existing governance forums

The pack demonstrates, as applied records:

1. Stakeholder roles  
2. Decision responsibilities  
3. Decision rights  
4. RACI  
5. Governance forums  
6. Escalation mechanisms  
7. Stakeholder decision flows  
8. Federated-by-domain operating model  
9. Interaction between central governance and domain governance  

```text
Existing Governance Framework
          ↓
Roles
          ↓
Decision Rights
          ↓
RACI
          ↓
Forums
          ↓
Escalation
          ↓
Federated Decision Flow
```

This pack **connects** existing Rafid artifacts. It does **not** rebuild the operating model, ownership map, policies, quality, catalog, lineage, MDM, lifecycle, KPIs, or NDMO evidence.

---

## 2. Relationship to existing Phase 3

Phase 3 is the locked **Data Governance Operating Model**:

- federated-by-domain (not by hospital)
- reporting lines (CDO to Cluster CEO; CIO as peer)
- role catalogue
- enterprise RACI (one **A** per row)
- decision and escalation paths
- four forums
- end-to-end workflow
- NDMO name mapping

This pack is **applied evidence** of how those designs are used when later phases name real activities (classification, CDE, lineage, MDM, KPIs, exceptions, NDMO/PDPL).

Locked files remain authoritative for:

- federated-by-domain as the headline model
- role **types** and NDMO name mapping
- enterprise RACI cells
- four forums and their cadences
- escalation hierarchy ending at Cluster CEO
- **No new DMC decision right**

This pack does **not** replace `01`–`09` in the parent folder. It does **not** invent a new Phase. It does **not** invent governance roles or forums.

Phase 4 remains authoritative for the eight domains and Owner / Steward **titles**. Phase 6 remains authoritative for POL/STD/PRC text.

---

## 3. Stakeholder Roles

[`stakeholders/stakeholder-role-matrix.md`](stakeholders/stakeholder-role-matrix.md) applies the Phase 3 catalogue.

**Core set:** Data Owner; Business Data Steward; DMO; Data Management Committee; IT / Data Custodian; plus the four existing forums as decision venues.

**Supporting catalogue roles reused (not invented):** Executive Sponsor (Cluster CEO); CDO; Data Governance Officer; CIO; PDPO; Compliance Officer; Legal Advisor; ODIA; Data Consumer.

Year-1 examples use the Phase 4 titles for Patient / Person Master, Clinical / Medical Records, and Financial / Billing & Claims.

IT is **not** the business owner of data. DMO does **not** become Data Owner of a business domain.

---

## 4. Accountability

[`stakeholders/stakeholder-accountability.csv`](stakeholders/stakeholder-accountability.csv) connects eleven governance areas to Owner, Steward, DMO, DMC, and IT / Custodian:

Ownership · Classification · Metadata · Data Quality · Lineage · MDM · Lifecycle · Governance KPIs · Exceptions · NDMO evidence · PDPL governance considerations

Each cell points at a locked Phase 3–14 source. PDPO remains **A** only for sharing **privacy compliance review** (Phase 4 row 7). That is not a PDPL compliance claim.

---

## 5. RACI

[`raci/governance-raci.md`](raci/governance-raci.md) and [`raci/governance-raci.csv`](raci/governance-raci.csv) apply the locked RACI to **18** activities.

The required fifteen activities are covered. Three extra rows preserve locked splits that must not be collapsed (catalog programme vs content is already in the fifteen; lineage programme vs business registration; in-policy waiver vs Policy exception).

**Rules reused:** exactly one **A** per row; IT not **A** for business meaning.

Authoritative sources remain [`../04-enterprise-raci.md`](../04-enterprise-raci.md) and [`../../04-ownership-stewardship/03-ownership-decision-matrix.md`](../../04-ownership-stewardship/03-ownership-decision-matrix.md).

---

## 6. Decision Rights

[`decision-rights/decision-rights-matrix.md`](decision-rights/decision-rights-matrix.md) and [`decision-rights/decision-rights.csv`](decision-rights/decision-rights.csv) record **16** decisions.

Classes remain Strategic / Tactical / Operational (Phase 2). Residual beyond DMC remains Cluster CEO. CDO does not pick clinical definitions. Owner cannot self-approve out-of-policy access.

---

## 7. Governance Forums

[`forums/governance-forum-register.md`](forums/governance-forum-register.md) registers the **four** approved cadences only:

| Forum | Frequency (Phase 3) |
| --- | --- |
| Data Management Committee | Quarterly + extraordinary |
| Steward Forum | Monthly |
| Domain huddles | Biweekly or monthly by domain risk |
| DMO operations huddle | Weekly |

Cadence is **Proposed / Illustrative** as a live operating rhythm. Live meetings are not claimed.

No Privacy Committee, Data Council, or hospital board is added.

---

## 8. Escalation

[`escalation/governance-escalation-model.md`](escalation/governance-escalation-model.md) applies the locked path:

```text
Business Data Steward → Data Owner → DGO → CDO → Data Management Committee → Cluster CEO
```

Triggers covered: cross-domain conflict; ageing quality issue; classification dispute; governance exception; unresolved lineage; NDMO/regulatory verification; repeated overdue action; privacy incident; Custodian security refusal.

Parallel paths unchanged: PDPO + CO + Legal for material regulatory; CISO / NCA for cyber. Numeric SLAs are **not** invented.

---

## 9. Decision Flows

[`decision-flows/stakeholder-decision-flows.md`](decision-flows/stakeholder-decision-flows.md) contains **six** synthetic examples:

1. Data quality issue (duplicate Patient ID)  
2. Classification dispute (encounter notes Internal vs Restricted)  
3. Cross-domain ownership conflict (attending clinician on the encounter)  
4. Governance exception (catalog publish without Owner-accepted definition)  
5. Data Owner appointment (PRC-001)  
6. Critical lineage confirmation (Patient → Encounter → Claims)

---

## 10. Communication

[`stakeholders/stakeholder-communication-matrix.csv`](stakeholders/stakeholder-communication-matrix.csv) maps audience, information, purpose, owner, frequency, channel/forum, and escalation trigger.

Channels are existing forums and registers only. No collaboration product is invented.

---

## 11. Federated Governance Model

[`federated-model/federated-governance-operating-model.md`](federated-model/federated-governance-operating-model.md) applies the locked split:

| Layer | Who | Holds |
| --- | --- | --- |
| Enterprise / central | DMC / CDO / DMO | Framework, policy, standards, methods, cross-domain escalation, evidence, enterprise reporting |
| Domain | Data Owner + Business Data Steward | Meaning, ownership, stewardship, domain quality / metadata / lineage / classification / in-policy decisions |
| Technical | IT / Data Custodian | Systems, provisioning, technical metadata/lineage, platform controls |

Facilities participate through domains. The model is **not** federated-by-hospital.

---

## 12. Limitations

- Synthetic / illustrative / non-production.
- Does not rewrite locked Phase 3 files.
- Does not appoint named incumbents.
- Does not claim live forums, SLAs, or measured KPI results.
- Does not invent roles, committees, or DMC decision classes.
- Does not make IT or DMO a business Data Owner.
- Specific NDMO organization-control duties remain `[NDMO verification required]`.
- PDPL overlay remains `[Legal / regulatory verification required]`.

---

## 13. Portfolio disclaimer

This is a fictional portfolio project.

It does **not** claim a real stakeholder engagement programme, a live governance operating model, appointed officers, NDMO or PDPL compliance, or a real healthcare implementation.

Rafid Health Cluster is fictional.

**Synthetic / Illustrative / Non-production portfolio project.**  
**No live organizational operation is claimed unless explicitly supported.**

---

## File structure

```text
03-operating-model/working-pack/
├── README.md
├── stakeholders/
│   ├── stakeholder-role-matrix.md
│   ├── stakeholder-accountability.csv
│   └── stakeholder-communication-matrix.csv
├── raci/
│   ├── governance-raci.md
│   └── governance-raci.csv
├── decision-rights/
│   ├── decision-rights-matrix.md
│   └── decision-rights.csv
├── forums/
│   └── governance-forum-register.md
├── escalation/
│   └── governance-escalation-model.md
├── decision-flows/
│   └── stakeholder-decision-flows.md
└── federated-model/
    └── federated-governance-operating-model.md
```

---

## Ownership (existing roles only)

No new roles. Responsible / Review / Approval use the Phase 3 catalogue.

| Working-pack artifact | Responsible | Review | Approval (existing rights only) |
| --- | --- | --- | --- |
| Pack method, matrices, forum register, flows | DMO | CDO | CDO for method; DMC only if an existing policy/exception class is invoked |
| Domain interpretation of a worked example | Data Owner **A** | Business Data Steward **R** | Data Owner **A** (in-policy) |
| Privacy-review occupancy in flows | PDPO **A** for the privacy review | DMO (record completeness) | Dual-A sharing rows unchanged |
| Policy-level exception example | DMC remains **A** (existing) | DMO register **R** | No new DMC class |

IT / Data Custodian remains technical implementation only. Forum names reused: Data Management Committee, Steward Forum, Domain huddles, DMO operations huddle. Secretariat remains DGO (non-member).
