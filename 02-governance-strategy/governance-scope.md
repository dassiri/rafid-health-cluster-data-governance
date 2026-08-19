# Governance Scope

**Document ID:** RHC-DG-P2-001  
**Phase:** 2 — Governance Design Boundaries  
**Status:** Documented  
**Does not decide:** Year-1 rollout sites, tool scope, or partner-contract language

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document sets the **standing boundary** of Rafid’s data governance: which organization units, data, and NDMO knowledge domains the framework is meant to cover. It is a design-boundary artifact `[B]`, distinct from program-scope (what this **documentation project** will produce) in [`../01-project-foundation/project-scope.md`](../01-project-foundation/project-scope.md).

---

## 2. Organizational scope `[A]`

**In:** All facilities and corporate functions listed in the organization profile (hospitals, PHCs, specialty centers, cluster corporate).

**In (directional):** Business partners that handle Rafid/government data (EMR vendor support, outsourced billing, and similar) `[A]`, because NDMO Purpose and Scope extends the Standards to business partners handling government data `[C]`. Partner operating procedures are not written here.

**Out (for governance operations until a later decision):** Other MOH clusters’ internal data that Rafid does not hold or process `[A]`.

**Unresolved:** Whether specific research affiliates or university staff using cluster data are “partners” or internal users — Phase 3/6 `[NDMO verification required]` for sharing-regulation treatment.

---

## 3. Data scope

| Include | Basis |
| --- | --- |
| All recorded forms (electronic, paper, email, images, voice, and other recorded data) | NDMO Purpose and Scope `[C]`; Rafid is assumed to hold these forms `[A]` |
| Clinical, administrative, workforce, financial, quality, and reporting data in the landscape | Landscape `[A]` |
| Personal data and health-related data | Landscape `[A]`; NDMO Personal Data Protection domain exists `[C]`; PDPL detail `[NDMO verification required]` |
| Shadow copies on shared drives and mailboxes | Landscape issue `[A]`; still in the **governance** boundary even if hard to inventory |

| Exclude from **this framework’s design work** (not “data that may be ignored operationally”) | Basis |
| --- | --- |
| Classified national-security datasets Rafid is not assumed to hold | Not in the fictional landscape `[A]` |
| Employee personal devices as a full BYOD control program | Cybersecurity / NCA coordination later; Domain 15 is NCA-mandated `[C]` |

---

## 4. Decision scope vs. execution scope `[B]`

**Governance decides** (later, through the operating model): policy intent, classification method, quality expectations, sharing rules, ownership, and exception handling.

**Governance does not, in this program, execute:** EMR configuration, NCA technical security control implementation, or MOH statistical-definition changes.

NDMO Domain 15 (Data Security and Protection) is under the mandate of the National Cybersecurity Authority `[C]`. Rafid governance **coordinates** with cybersecurity; it does not replace NCA control design.

---

## 5. NDMO knowledge-domain coverage `[C]`

The national framework spans **15 domains**. Rafid’s enterprise framework is **intended to cover all 15 as alignment targets** over the life of the program `[A]` intent + `[C]` domain list.

Naming below is official `[C]` (NDMO Standards v1.5, Section 6). This table is **coverage intent**, not implementation status.

| # | Domain | Phase 2 status |
| --- | --- | --- |
| 1 | Data Governance | Strategy artifacts in progress; operating design not started |
| 2 | Data Catalog and Metadata | Not started |
| 3 | Data Quality | Not started |
| 4 | Data Operations | Not started |
| 5 | Document and Content Management | Not started |
| 6 | Data Architecture and Modeling | Not started |
| 7 | Reference and Master Data Management | Not started |
| 8 | Business Intelligence and Analytics | Not started |
| 9 | Data Sharing and Interoperability | Not started |
| 10 | Data Value Realization | Not started |
| 11 | Open Data | Not started |
| 12 | Freedom of Information | Not started |
| 13 | Data Classification | Not started |
| 14 | Personal Data Protection | Not started |
| 15 | Data Security and Protection | NCA-mandated domain `[C]`; not designed in this program |

P1/P2/P3 specification timing is an official NDMO planning input `[C]` (Section 8). Mapping Rafid initiatives to those priorities is Phase 13, not Phase 2.

---

## 6. Time horizon `[C]` + `[A]`

NDMO describes a three-year implementation pattern for specifications: Year 1 — P1; Year 2 — P1+P2; Year 3 — P1+P2+P3 `[C]` (Section 8.2).

Rafid **records that pattern as a planning constraint** for later roadmap work `[A]` intent. This document does **not** set Rafid’s start date, does not declare which calendar year is “Year 1,” and does not claim that NDMO’s original national rollout calendar still applies unchanged. Current applicability of that three-year clock to a health cluster is `[NDMO verification required]`.

---

## 7. Intentionally unresolved

- Phased geographic rollout (which hospital first).
- Which of the 15 domains are in the first operating-model release beyond Domain 1 strategy.
- FOI and Open Data operating procedures for a healthcare cluster `[NDMO verification required]`.
- Exact boundary between cluster governance and MOH national program data that only transits Rafid systems.

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5, Purpose and Scope; Section 6 (15 domains); Section 8 (priorities and three-year plan); Domain 15 NCA note | Boundary language; domain list; security mandate |
| `[A]` | Organization profile and data landscape | What Rafid holds |
| `[B]` | Governance-scope vs. program-scope split | Document design |
