# Stakeholder Role Matrix

**Document ID:** RHC-DG-P3-WP-001  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** Named incumbents, new role types, new forums, or new DMC decision rights

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Locked sources:** [`../../03-role-catalogue.md`](../../03-role-catalogue.md) · [`../../04-enterprise-raci.md`](../../04-enterprise-raci.md) · [`../../../04-ownership-stewardship/02-enterprise-ownership-matrix.md`](../../../04-ownership-stewardship/02-enterprise-ownership-matrix.md)

---

## 1. Purpose

Apply the locked Phase 3 role catalogue to a practical stakeholder matrix: who is accountable, who decides, who is consulted, who receives escalation, and which existing forum they use.

This file does **not** rewrite the role catalogue. It does **not** invent roles. It does **not** appoint people.

---

## 2. How to read the matrix

| Column | Meaning |
| --- | --- |
| Stakeholder | Rafid working title already in the Phase 3 catalogue |
| NDMO name | Mapped name only `[C]` — not a compliance claim |
| Primary responsibility | What this stakeholder does in daily governance |
| Decision rights | Strategic / tactical / operational class already assigned in Phase 3 |
| Accountability | What they answer for if it fails |
| Consulted by | Who must seek their input before a decision |
| Receives escalations | What lands with them when the lower path cannot close |
| Governance forum | Existing Phase 3 forum only |
| Scope | Enterprise, domain, or technical |

Exactly **one** business Data Owner remains accountable for a domain. IT / Data Custodian is never the business owner of data.

---

## 3. Core stakeholder set

These are the stakeholders named in the portfolio claim. Supporting catalogue roles follow in Section 4.

### 3.1 Data Owner

| Element | Applied record `[A][B]` |
| --- | --- |
| **Stakeholder** | Data Owner |
| **NDMO name** `[C]` | Business Data Executive |
| **Primary responsibility** | Business accountability for meaning, quality, classification application, in-policy access/sharing, and issue closure in one domain across all facilities |
| **Decision rights** | **Tactical** inside the domain; **operational** acceptance of steward recommendations. Not enterprise policy. |
| **Accountability** | Domain business outcomes: definitions, dataset classification, quality rules, catalog content, in-policy residual quality risk |
| **Consulted by** | Business Data Steward (packs); DMO (cross-domain and standards); other Owners on shared flows; PDPO on personal-data sharing |
| **Receives escalations** | Steward cannot close an in-policy decision; consumer disputes an approved rule; Custodian needs a business meaning decision |
| **Governance forum** | Domain huddle (decision). Standing or invited DMC member by Phase 4 Year-1 composition. Steward Forum does not replace the Owner. |
| **Scope** | **Domain** — cluster-wide for that domain, not hospital-by-hospital |

Year-1 titles remain the eight Phase 4 Owners. Example: Patient / Person Master Data Owner = Patient Access & Experience Director `[A]`.

The Owner **approves** classification and in-policy residual risk where existing policy allows. The Owner **cannot** self-approve out-of-policy access or L3 policy exceptions.

### 3.2 Business Data Steward

| Element | Applied record `[A][B]` |
| --- | --- |
| **Stakeholder** | Business Data Steward |
| **NDMO name** `[C]` | Business Data Steward |
| **Primary responsibility** | Operational governance: definition drafts, metadata, quality coordination, classification packs, lineage coordination, issue investigation, consumer guidance |
| **Decision rights** | **Operational** within Owner-approved rules. Cannot change meaning, approve L3 policy, or act as a second Owner. |
| **Accountability** | Completeness and timeliness of packs, monitoring, and issue investigation — not domain ownership |
| **Consulted by** | Data Consumers; Custodian (business meaning); DMO (cross-domain clash detection); other domain Stewards on shared flows |
| **Receives escalations** | Consumer access/quality complaints; Custodian questions that are not technical-only |
| **Governance forum** | Domain huddle + monthly Steward Forum |
| **Scope** | **Domain** operational execution |

Example: Clinical / Medical Records Steward = Head of Health Information Management (HIM) `[A]`.

### 3.3 Data Management Office (DMO)

DMO is the **central coordination function**, not a second Data Owner and not a second IT department. Locked seats inside the office: **CDO** (head) and **Data Governance Officer** (reports to CDO; DMC secretariat, non-member).

| Element | Applied record `[A][B]` |
| --- | --- |
| **Stakeholder** | Data Management Office (CDO + Data Governance Officer) |
| **NDMO name** `[C]` | Data Management Office / Chief Data Officer / Data Governance Officer |
| **Primary responsibility** | Governance coordination; standards and methods; frameworks; monitoring; evidence; reporting; escalation coordination; issue/exception register completeness |
| **Decision rights** | **Tactical** on methods and enterprise standard **proposals**; **operational** on triage routing. CDO **A** for catalog programme, lineage programme, KPI reporting, and alignment self-assessment (Phase 3). Cannot approve L3 policy. Cannot reassign domain ownership. Cannot override a Data Owner on business meaning. |
| **Accountability** | Operating system of governance: process integrity, packs, registries, KPI method, NDMO alignment evidence design |
| **Consulted by** | Data Owners and Stewards (method); DMC (secretariat packs); Custodian (tooling vs programme split); PDPO / Compliance Officer / Legal (aligned agenda) |
| **Receives escalations** | Owner unresponsive (qualitative ageing); cross-domain conflict (DGO mediates); SLA-breach list for CDO; completeness failures on exception/classification/metadata packs |
| **Governance forum** | Weekly DMO operations huddle (triage). Prepares Steward Forum and DMC packs. CDO sits on DMC; DGO is secretariat (non-member). |
| **Scope** | **Enterprise** coordination |

### 3.4 Data Management Committee (DMC)

| Element | Applied record `[A][B]` |
| --- | --- |
| **Stakeholder** | Data Management Committee (working name: Data Governance Council) |
| **NDMO name** `[C]` | Entity Data Management Committee |
| **Primary responsibility** | Enterprise governance decisions: strategy; L3 policy; material exceptions; residual sharing/openness risk; Owner non-participation; KPI and alignment **review** as an existing input |
| **Decision rights** | **Strategic.** Tactical standards are **endorsed** only when they change risk appetite or conflict with policy. **No new DMC class is created in this pack.** |
| **Accountability** | Sole **A** for strategy, L3 policy, and material exceptions (Phase 3) |
| **Consulted by** | CDO / DMO (packs); Owners (exception papers); Compliance Officer (alignment status) |
| **Receives escalations** | Unresolved cross-domain meaning/risk; policy exceptions; care-safety or cluster-report residual; Owner non-participation |
| **Governance forum** | This forum **is** the strategic board. Chair: Cluster CEO. CDO does **not** chair. |
| **Scope** | **Enterprise** |

Year-1 standing members (Phase 4, unchanged): Cluster CEO (Chair); CDO; CIO; PDPO; Compliance Officer; Patient/Person Master Data Owner; Clinical/Medical Records Data Owner; Financial/Billing & Claims Data Owner. Other Owners by invitation. Secretariat: Data Governance Officer (non-member).

### 3.5 IT / Data Custodian

| Element | Applied record `[A][B]` |
| --- | --- |
| **Stakeholder** | Data Custodian (IT Data Steward) |
| **NDMO name** `[C]` | IT Data Steward |
| **Primary responsibility** | Technical implementation: systems, access provisioning, technical metadata, technical lineage, operational/platform controls, quality-rule implementation in systems |
| **Decision rights** | **Operational-technical.** May refuse an implementation that violates NCA-aligned security, with dual escalation to the CISO path **and** CDO. Cannot approve what data means. Cannot classify. Cannot close a business quality issue as Owner. |
| **Accountability** | Faithful technical implementation of approved business decisions; technical metadata/lineage accuracy |
| **Consulted by** | Steward and Owner (measurability, system location, provisioning); DMO (catalog tool operations; lineage capture) |
| **Receives escalations** | Technical defects; provisioning after Owner approval; security block (does not become classification **A**) |
| **Governance forum** | Domain huddle for the systems they run; Steward Forum as needed. CIO sits on DMC as a **peer** of the CDO, not as Data Owner. |
| **Scope** | **Technical** |

**IT is not the business owner of data.**

### 3.6 Governance forums (existing set only)

Forums are stakeholders **as decision venues**, not extra role types. The approved set remains four cadences. Cadence is Phase 3 design; **Proposed / Illustrative** as a live operating rhythm. Live meetings are not claimed.

| Forum | Role in the stakeholder model |
| --- | --- |
| Data Management Committee | Strategic decisions listed in Section 3.4 |
| Steward Forum | Cross-domain tactical coordination; recommendations only; not L3 policy |
| Domain huddles | In-policy domain decisions by Owner + Steward + Custodian |
| DMO operations huddle | Intake triage and routing only; not a governance board |

Full register: [`../forums/governance-forum-register.md`](../forums/governance-forum-register.md).

---

## 4. Supporting catalogue roles (reused, not invented)

These seats already exist in Phase 3. They are included where a core activity consults or escalates to them. They are **not** new stakeholders.

| Stakeholder | Primary use in this pack | Decision rights (locked) | Forum |
| --- | --- | --- | --- |
| **Executive Sponsor (Cluster CEO)** | Chairs DMC; residual / material regulatory **A** | Strategic residual the Committee cannot settle; CDO appointment (with Committee) | DMC |
| **Chief Data Officer** | Head of DMO; DMC member; programme **A** on catalog, lineage programme, KPI reporting, alignment assessment | Tactical methods; not L3 policy; not domain meaning | DMC; DMO huddle |
| **Data Governance Officer** | DMO staff; DMC secretariat (non-member); Steward Forum chair | Operational triage; mediation; no policy **A** | Steward Forum; DMO huddle |
| **CIO** | Executive for systems and Custodians; DMC standing member; **peer** of CDO | Not Data Owner. No CDO–CIO tooling reporting line. | DMC |
| **Personal Data Protection Officer** | **A** only for sharing **privacy compliance review** (Phase 4 row 7). **C** on classification of personal/health data | Not Owner of quality, classification, or catalog meaning | DMC standing; consulted at Steward Forum as needed |
| **Compliance Officer (data)** | **R** on maturity / alignment self-assessment with CDO **A**; monitors data-management compliance process | Not Internal Audit; not policy **A** | DMC standing |
| **Legal Advisor** | **C** on sharing, retention, regulatory escalation, exceptions | No operational **A** | Consulted; not a fifth forum |
| **Open Data and Information Access Officer** | **C** when the likely outcome is Public / open data | Year-1 operating model remains thin `[NDMO verification required]` | Consulted; not a Year-1 standing DMC member |
| **Data Consumer** | Uses data under policy; raises defects; no governance authority | None on meaning, classification, or sharing | Invited to domain huddles when needed |

---

## 5. Domain Owner / Steward titles used in working examples `[A]`

| Domain | Data Owner | Business Data Steward |
| --- | --- | --- |
| Patient / Person Master Data | Patient Access & Experience Director | Head of Patient Registration & Access |
| Clinical / Medical Records Data | Chief Medical Officer (CMO) | Head of Health Information Management (HIM) |
| Financial / Billing & Claims Data | Chief Financial Officer (CFO) | Revenue Cycle Manager |

The other five Phase 4 domains remain in force. This pack does not add a ninth Owner.

---

## 6. What this matrix does not do

- Does not invent Chief Data Steward, Data Governance Manager, Privacy Committee, Data Council, or hospital governance boards
- Does not make DMO or IT a business Data Owner
- Does not create dual-**A** ownership
- Does not claim officers are appointed or forums have met

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Phase 3 role catalogue, RACI, forums | Matrix cells |
| `[A]` | Phase 4 Owner / Steward titles; Year-1 DMC composition | Examples |
| `[C]` | NDMO role and structure **names** | Mapping column |
| `[NDMO verification required]` | Organizational Manual duties; PDPL DPO equivalence; ODIA operating depth | Not treated as implemented |
