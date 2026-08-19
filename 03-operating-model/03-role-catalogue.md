# Role Catalogue

**Document ID:** RHC-DG-P3-003  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Named incumbents or job-description text from NDMO’s Organizational Manual. Year-1 **domain Owner titles** and **DMC standing membership** are recorded in Phase 4 and reflected in Section 2.2 below.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This catalogue defines **role types** for the fictional Rafid Health Cluster `[A]`. It does not appoint named people. Year-1 domain Owner **titles** and DMC **standing membership** are in Phase 4 and Section 2.2.

NDMO names the structures and roles listed in the mapping column `[C]`. Specification-level control IDs and Organizational Manual duties are `[NDMO verification required]`.

---

## 2. Core catalogue

### 2.1 Executive Sponsor — Cluster CEO `[B]`

| Element | Design |
| --- | --- |
| **Purpose** | Give data authority equal to clinical and financial authority. Unblock cross-facility decisions. |
| **Authority** | Chairs the Data Management Committee; can escalate unresolved strategic risk; does not run daily governance. |
| **Responsibilities** | Appoint CDO; resource the DMO; require Owners to participate; receive regulatory/material-risk escalation. |
| **Decision rights** | **Strategic:** residual risk the Committee cannot settle; CDO appointment (with Committee). Not operational classification or quality rules. |
| **Membership / representation** | Role is the Cluster CEO `[A]` org chart. |
| **Escalation responsibilities** | Receives Committee-level and material regulatory escalations. |
| **Cadence** | Chairs the Data Management Committee. No extra CEO data meeting. |
| **NDMO map** | Sponsor title is `[B]`. NDMO requires senior-executive approval of strategy `[C]`. |

### 2.2 Data Management Committee (working name: Data Governance Council)

NDMO name: Entity Data Management Committee `[C]`.

| Element | Design |
| --- | --- |
| **Purpose** | Direction and oversight of the cluster data agenda. Approves strategy and L3 policy. |
| **Authority** | Sole **Accountable** forum for strategy and policy approval. Does not rewrite domain definitions. |
| **Responsibilities** | Approve/refresh strategy; approve policies; accept material exceptions; accept residual sharing/openness risk; review KPI and alignment status; compel Owner participation. |
| **Decision rights** | **Strategic.** Tactical standards are **endorsed** only when they change risk appetite or conflict with policy. |
| **Membership / representation** | **Year-1 composition finalized in Phase 4** `[A]` (fictional organizational design). **Chair:** Cluster CEO. **Standing members:** CDO; CIO; PDPO; Compliance Officer; Patient/Person Master Data Owner; Clinical/Medical Records Data Owner; Financial/Billing & Claims Data Owner. **By invitation when relevant:** Provider/Clinician Data Owner; HR/Workforce Data Owner; Supply Chain & Asset Data Owner; Quality & Patient Safety Data Owner; Reference/Organizational Master Data Owner. **Secretariat (non-member, Phase 3 operating design `[B]`):** Data Governance Officer. Owner titles: [`../04-ownership-stewardship/02-enterprise-ownership-matrix.md`](../04-ownership-stewardship/02-enterprise-ownership-matrix.md). |
| **Escalation responsibilities** | Unresolved cross-domain or material risk → CEO as Chair. Regulatory material risk → CEO + Legal + PDPO in parallel. |
| **Cadence** | Quarterly, plus extraordinary session for material regulatory or patient-safety data incidents. |

Committee duties in NDMO’s Organizational Manual remain `[NDMO verification required]`.

### 2.3 Data Management Office (working name: Data Governance Office)

NDMO name: Data Management Office `[C]`. Headed by the CDO `[C]`; Data Governance Officer reports to the CDO `[C]` names / `[B]` line.

Small **central coordination** function, not a second IT department.

| Element | Design |
| --- | --- |
| **Purpose** | Run the operating system of governance: process, standards pack, issues, forums, evidence, training coordination. |
| **Authority** | Tactical **process** authority (how issues move, what a complete request looks like). No authority to override a Data Owner on business meaning. |
| **Responsibilities** | Maintain RACI, decision log, issue register (later artifacts — not built in this phase); prepare Committee packs; coach stewards; coordinate NDMO alignment work; draft policy **for** Committee approval; report KPIs. |
| **Decision rights** | **Tactical** on methods and enterprise standards **proposals**; **operational** on triage routing. Cannot approve L3 policy. Cannot reassign domain ownership (CDO + Committee). |
| **Membership / representation** | CDO (head of office); Data Governance Officer; analyst/coordinator capacity `[A]` sizing later. PDPO, Compliance Officer, ODIA, Legal Advisor are **aligned** to the agenda; they are not all DMO line reports (see [`02-reporting-lines.md`](02-reporting-lines.md)). |
| **Escalation responsibilities** | DGO → CDO → Committee. |
| **Cadence** | Weekly DMO operations huddle (triage, not a governance board). |

### 2.4 Data Owner (Business Data Executive)

NDMO name: Business Data Executive `[C]`.

A **domain** is a business data subject area — **not** a hospital. Year-1 domain-to-Owner **titles** are in [`../04-ownership-stewardship/`](../04-ownership-stewardship/). This section defines the Owner **role**, not the eight-row map.

| Element | Design |
| --- | --- |
| **Purpose** | One accountable Owner per domain across all facilities using that data. |
| **Authority** | Accountable for meaning, quality rules, dataset classification, and access/sharing **within policy** for that domain. |
| **Responsibilities** | Appoint/support Business Data Steward(s); accept definitions and quality rules; accept classification of domain datasets; decide in-policy access and routine sharing; own issue closure for the domain. |
| **Decision rights** | **Tactical** inside the domain; **operational** acceptance of steward recommendations. **Not** enterprise policy. |
| **Membership / representation** | Owner is a **cluster** role, not “Director of Lab at Hospital X only,” unless Phase 4 documents a split. Facility SMEs may be stewards later. |
| **Escalation responsibilities** | Cross-domain or policy conflict → DGO/CDO → Committee. |
| **Cadence** | Domain huddle. |

If two executives share a domain, Phase 4 must still name **one** Accountable Owner.

### 2.5 Business Data Steward

NDMO name: Business Data Steward `[C]`.

| Element | Design |
| --- | --- |
| **Purpose** | Execute and coordinate operational governance in the domain. |
| **Authority** | Recommend; implement agreed rules; raise issues; **do not** own the domain. |
| **Responsibilities** | Definitions drafts; quality monitoring; classification packs; catalog content; issue investigation; consumer guidance. |
| **Decision rights** | **Operational** within Owner-approved rules. Cannot approve new enterprise policy or change meaning without the Owner. |
| **Membership / representation** | Named by the Owner. Year-1 steward titles are in [`../04-ownership-stewardship/02-enterprise-ownership-matrix.md`](../04-ownership-stewardship/02-enterprise-ownership-matrix.md). |
| **Escalation responsibilities** | → Data Owner; if Owner unresponsive past SLA → DGO. |
| **Cadence** | Domain huddle + monthly Steward Forum. |

### 2.6 Data Custodian (IT Data Steward)

NDMO name: IT Data Steward `[C]`. “Custodian” is DAMA-style working language `[B]`.

| Element | Design |
| --- | --- |
| **Purpose** | Technical implementation and system-of-record operation — not business ownership. |
| **Authority** | Change systems, interfaces, and access **provisioning** after a business decision. Cannot approve “what the data means.” |
| **Responsibilities** | Implement quality rules in systems; technical lineage; catalog scan/tooling; backups per policy; apply security controls with cybersecurity. |
| **Decision rights** | **Operational-technical.** May refuse an implementation that violates NCA-aligned security, with escalation to the CISO path **and** CDO (dual). |
| **Membership / representation** | Application owners, integration, EMR technical team — titles only. |
| **Escalation responsibilities** | Security block → CISO + CDO; business-rule dispute → Data Owner, not “IT decides.” |
| **Cadence** | Domain huddle (for the systems they run) and Steward Forum as needed. |

NCA mandate for NDMO Domain 15 `[C]`: governance coordinates; it does not replace NCA.

### 2.7 Data Consumer `[B]`

Not an NDMO-named role in the Standards role list. Working title only.

| Element | Design |
| --- | --- |
| **Purpose** | Use data under policy; surface defects; not a governance authority. |
| **Authority** | Request access/extracts; raise issues. No authority to copy data off-platform as a personal store. |
| **Responsibilities** | Use approved sources; complete request forms; report quality issues. |
| **Decision rights** | None on meaning, classification, or sharing. |
| **Membership / representation** | Clinicians, analysts, quality, finance, researchers as applicable `[A]`. |
| **Escalation responsibilities** | Denied access or bad data → Steward for that domain. |
| **Cadence** | None. Invited to domain huddles when needed. |

---

## 3. NDMO-named supporting roles `[C]`

These seats are in the catalogue because NDMO names them. They are **not** extra Councils. Duty-level text is `[NDMO verification required]`.

| Role (NDMO name) `[C]` | Operating placement `[B]` |
| --- | --- |
| **Personal Data Protection Officer** | Solid line to CEO; dotted working relationship to CDO. Consulted on classification of personal/health data, access, and sharing; parallel path on privacy incidents. PDPL DPO equivalence `[NDMO verification required]`. |
| **Compliance Officer** (data management agenda) | Solid line to Legal/Internal Control; dotted to CDO. Designs/monitors data-management compliance process; does **not** replace Internal Audit independence `[NDMO verification required]`. |
| **Open Data and Information Access Officer** | Consulted when a decision is open data or public-information access. Healthcare operating depth `[NDMO verification required]`. Seat kept; year-1 operating model remains thin. |
| **Legal Advisor** | Consulted on sharing, retention, regulatory escalation, and exceptions. |

---

## 4. Decision authority (summary)

| Role | Decision authority |
| --- | --- |
| Executive Sponsor (CEO) | Strategic residual risk; CDO appointment |
| Data Management Committee | **A** for strategy, L3 policy, material exceptions |
| Data Management Office / CDO + DGO | Tactical methods; CDO **A** for catalog programme, lineage programme, KPI reporting, maturity assessment |
| Data Owner | **A** for domain business decisions listed in the RACI |
| Business Data Steward | Operational within Owner rules |
| Data Custodian | Technical how; security veto only with CISO+CDO path |
| Data Consumer | None |

Full RACI: [`04-enterprise-raci.md`](04-enterprise-raci.md).

---

## 5. Intentionally unresolved

- Domain-to-Owner map — Phase 4
- Steward names and counts — Phase 4
- Organizational Manual job-content alignment `[NDMO verification required]`

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 Implementation Brief | Working titles, cadences, authority split |
| `[C]` | NDMO Standards v1.5 — role and structure **names** | Mapping column |
| `[A]` | Organization profile | CEO and facility context |
| `[NDMO verification required]` | Organizational Manual; PDPL; FOI/ODIA operating model | Duty-level and statutory mapping |
