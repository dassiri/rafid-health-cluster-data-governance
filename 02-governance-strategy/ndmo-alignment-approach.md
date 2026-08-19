# NDMO Alignment Approach

**Document ID:** RHC-DG-P2-004  
**Phase:** 2 — Governance Design Boundaries  
**Status:** Documented **method** (not a compliance matrix)  
**Does not decide:** Control implementation, evidence, scores, or a three-year initiative plan

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document states **how** Rafid will align to NDMO without pretending alignment is finished.

Folder `14-ndmo-alignment/` holds the **Designed** alignment and evidence pack. That pack is **not** a compliance matrix and does **not** invent control numbers. The **method** remains this file.

NDMO is the national regulator of data in the Kingdom and issued Data Management and Personal Data Protection Standards based on the national framework `[C]` (NDMO Standards v1.5, Introduction). The Standards cover **15 domains**, **77 controls**, and **191 specifications** `[C]` (Section 8.1).

This program **aligns to** that structure. It does **not** claim a compliance score.

---

## 2. Official source used in this repository `[C]`

| Item | Value |
| --- | --- |
| Document | *Data Management and Personal Data Protection Standards* |
| Issuer | National Data Management Office (NDMO) |
| Version used | **1.5, January 2021** (document control also shows June 2021 incorporation of comments; the title block used here is Version 1.5 January 2021) |
| Access path used | SDAIA-hosted PDF (`PoliciesEN.pdf`) |
| What was **not** retrieved | NDMO Organizational Manual; Data Classification Regulation; Data Sharing Regulation; FOI Regulation; other NDMO policies named by the Standards |

If a later official version exists, Phase 14 must re-verify IDs before use `[NDMO verification required]`.

---

## 3. Alignment principles (program rules) `[A]` / `[B]`

1. **Cite or do not claim.** A requirement is `[C]` only when traced to the official text (or another official NDMO/SDAIA publication cited in the file).
2. **No invented IDs.** Control IDs follow NDMO’s pattern `DomainID.Number` (example given in the Standards: `DG.2`). Specification IDs follow `ControlID.Number` (example: `DG.2.2`) `[C]` (Section 7). If an ID is not in the retrieved text, it is not used.
3. **No fake completeness.** Partial work is labeled incomplete. Binary NDMO scoring (100% implemented vs 0% if partial) is described by NDMO for entity assessments `[C]` (Compliance and Enforcement). This repo will not self-award 100%.
4. **Domain 15 is NCA.** Data Security and Protection controls and specifications are addressed by the National Cybersecurity Authority `[C]`. Rafid alignment for Domain 15 is “coordinate / do not duplicate / do not invent NCA controls.”
5. **Partners are in the conversation.** Standards extend to business partners handling government data `[C]`. Contract language is later.
6. **Healthcare does not create a parallel NDMO.** Sector rules sit in the policy hierarchy (L2), they do not replace L1 `[B]`.

---

## 4. What NDMO says the Standards are `[C]`

Summaries; official PDF prevails.

| Topic | Official position (summary) |
| --- | --- |
| Audience | Public Entities; also business partners handling government data |
| Data coverage | Government data regardless of form or type |
| Structure | Domain → Control → Specification |
| Data Governance domain | Domain ID `DG`; 8 controls; 28 specifications |
| Priorities | P1, P2, P3 — implementation order |
| National planning pattern | Three-year path: P1 by end of year 1; P1+P2 by end of year 2; all by end of year 3 (Section 8.2) |
| Entity assessment | Annual, specification-level, binary implemented vs not; evidence; CDO-led; submit in Q3 as described in the Standards |
| DAMA | DAMA DMBOK is cited as a key reference for the Kingdom’s national data management standards (Introduction) |

**Rafid use of the three-year pattern:** planning **input** for Phase 13 only. This file does not start Rafid’s Year 1 clock `[A]`. Whether the original national calendar still binds a health cluster today is `[NDMO verification required]`.

---

## 5. Fifteen domains — alignment backbone `[C]`

Official names from NDMO Standards v1.5, Section 6. Domain IDs below are those used in the Standards text retrieved for this drop.

| Domain | Domain ID (as in Standards) | Controls / specs (Section 8.1) | This program |
| --- | --- | --- | --- |
| Data Governance | `DG` | 8 / 28 (18 P1, 9 P2, 1 P3) | Phase 1–2 strategy **documentation** only |
| Data Catalog and Metadata | `MCM` | 6 / 20 | Later |
| Data Quality | (see official PDF) | 4 / 13 | Later |
| Data Operations | (see official PDF) | 5 / 14 | Later |
| Document and Content Management | (see official PDF) | 5 / 12 | Later |
| Data Architecture and Modeling | (see official PDF) | 7 / 13 | Later |
| Reference and Master Data Management | (see official PDF) | 6 / 18 | Later |
| Business Intelligence and Analytics | (see official PDF) | 5 / 10 | Later |
| Data Sharing and Interoperability | (see official PDF) | 8 / 16 | Later |
| Data Value Realization | (see official PDF) | 4 / 8 | Later |
| Open Data | (see official PDF) | 5 / 10 | Later |
| Freedom of Information | (see official PDF) | 4 / 9 | Later |
| Data Classification | `DC` | 5 / 10 | Later |
| Personal Data Protection | (see official PDF) | 5 / 10 | Later |
| Data Security and Protection | — | Addressed by NCA | Out of design scope except coordination |

Where a domain ID is not copied in the “Domain ID” column, this drop **does not guess**. Use the official PDF `[NDMO verification required]` before citing those IDs in Phase 14. IDs that **were** clearly present in the retrieved text (`DG`, `MCM`, `DC`) may be used as `[C]`.

---

## 6. Data Governance controls — reference map only `[C]`

Official `DG` controls from NDMO Standards v1.5, Section 9.1. This is a **map**, not an implementation register.

| Control ID | Control name | Phase 0–2 documentation relevance |
| --- | --- | --- |
| `DG.1` | Strategy and Plan | Vision/mission/objectives/principles started; full `DG.1.1` contents, `DG.1.3` plan, `DG.1.4` approval **not done** |
| `DG.2` | Policy and Guidelines | Hierarchy only; gap analysis and policy **not done** |
| `DG.3` | Training and Awareness | Not started |
| `DG.4` | Data Management Organization | Role **names** recorded; office, committee, appointments **not done** |
| `DG.5` | Compliance Audit Framework | Not started |
| `DG.6` | Data Lifecycle Governance (plan review and communications) | Not started |
| `DG.7` | Performance Management | Phase 12 documents a **conceptual** Rafid KPI/maturity framework; NDMO KPI types are **not** copied as Rafid targets; **`DG.7` is not claimed implemented** |
| `DG.8` | Data Governance Artifacts | Not started (decision register, issue register, version control) |

---

## 7. Classification levels — cited for later work, not applied `[C]`

NDMO defines four classification levels. Impact mapping in `DC.3.2` (summary): High → Top Secret; Medium → Secret; Low → Confidential; None/Insignificant → Public `[C]`. `DC.3.3` describes a further assessment that may classify some low-impact data as Public instead of Confidential `[C]`.

**Phase 2 does not classify Rafid datasets.** Informal “high/medium” notes in the data landscape are not NDMO levels.

---

## 8. Method for later phases (to be executed in folders 03–14) `[B]`

| Step | Action | Output location |
| --- | --- | --- |
| 1 | Keep a controlled copy of the official Standards version in use | `14-ndmo-alignment/` (later) |
| 2 | For each workstream, list **only** official control IDs in that domain | Domain folder + Phase 14 |
| 3 | Record implementation status as Not started / Partial / Evidenced — never “compliant” without evidence | Phase 14 |
| 4 | If the Standards point to another NDMO regulation, fetch that regulation before designing the procedure | `[NDMO verification required]` until fetched |
| 5 | Healthcare overlays sit in L2 of the policy hierarchy; they are tagged separately | Phase 6 |
| 6 | DAMA or other `[B]` practices may fill *how* Rafid operates **only if** labeled `[B]` and not presented as extra NDMO controls | All folders |

---

## 9. What Phase 0–2 already is — and is not — against `DG.1` `[C]` / `[A]`

| `DG.1` element (official) | This repo |
| --- | --- |
| Current data management challenges | Qualitative as-is in organization profile and landscape `[A]` — not a formal challenge register |
| Internal + national strategic requirements | National: NDMO framework `[C]`; internal: fictional cluster goals `[A]` — not a full requirements file |
| Vision, mission, goals/objectives | Working statements exist |
| Metrics and 3–5 year targets | **Not set** |
| Initiative budget | **Not set** |
| Guiding principles adopted | NDMO set adopted; Rafid candidates optional |
| 3-year plan (`DG.1.3`) covering all domains, prioritized, with quick wins | **Not created** |
| Formal approval and socialization (`DG.1.4`) | **Not performed** |

---

## 10. Intentionally unresolved

- Whether a newer NDMO Standards version supersedes v1.5 for a real 2026 program `[NDMO verification required]`.
- Domain IDs not copied in Section 5.
- Full specification text (not reproduced here; copyright and scope).
- Organizational Manual role descriptions.
- Annual assessment methodology details beyond the Standards’ summary.
- Applicability and any health-sector exemptions `[NDMO verification required]`.

---

## 11. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO, *Data Management and Personal Data Protection Standards*, v1.5, January 2021 | All official structure, counts, `DG`/`MCM`/`DC` IDs, priorities, assessment, classification levels, NCA note |
| `[B]` | Alignment-method / traceability practice | Section 3 and 8 |
| `[A]` | Rafid program rules and as-is | Application without a Year-1 clock or compliance claim |
