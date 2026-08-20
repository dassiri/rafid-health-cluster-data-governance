# Governance Gap Analysis

**Document ID:** RHC-DG-P14-WP-003  
**Phase:** 14 — NDMO alignment (working pack)  
**Status:** Implemented (gap record only)

**Does not decide:** Closure of official NDMO/PDPL items by assumption

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

**Responsible:** DMO · **Review:** CDO; Compliance Officer · **Approval:** CDO (method). DMC only for residual risk already in the Phase 3 decision-right framework.

---

## 1. Purpose

Record **Rafid-specific** gaps between:

1. what is **Designed** in Phases 0–14;
2. what has been **applied** as synthetic working records;
3. what would be **Measured**;
4. what remains **verification required** against official sources.

This is not a generic consulting maturity report. Every gap points at an existing Rafid file.

Illustrative qualitative method only. **Not** an official enterprise risk methodology.

Related register: [`compliance-risk-register.csv`](compliance-risk-register.csv) (**12** risks).  
Locked Phase 14 gaps remain in [`../07-gap-and-verification-register.md`](../../07-gap-and-verification-register.md) (**RHC-GAP-001**–**020**). This file does **not** close them.

---

## 2. Risk method (illustrative)

Likelihood and impact use **High / Medium / Low** only (same qualitative language as Phase 13).

| Impact → Likelihood | High | Medium | Low |
| --- | --- | --- | --- |
| **High** | High | High | Medium |
| **Medium** | High | Medium | Low |
| **Low** | Medium | Low | Low |

No probabilities. No residual-risk scoring model is claimed.

---

## 3. Designed → Operational

These capabilities exist as documentation. They do **not** have synthetic working registers comparable to the Phase 8 inventory or Phase 9 lineage register.

| Gap | Current evidence | What Operational (project) would require | Owner |
| --- | --- | --- | --- |
| Ownership occupancy | Eight Owner **titles** (`04-ownership-stewardship/02-enterprise-ownership-matrix.md`) | Populated Ownership Registry with occupancy dates (still synthetic if produced; named people not required) | DMO; Data Owner **A** |
| Classification occupancy | Model + illustrative examples (`05-data-classification/`) | Dataset-level Classification Registry rows for MVP assets | Data Owner **A**; Business Data Steward **R** |
| Data quality operations | Framework + illustrative scorecard + one 8-row sample | Repeatable issue register and scorecard rows tied to the 13 CDEs (still synthetic) | Data Owner **A** |
| Sharing evidence | PRC-005 **design** | Completed dual-A request records (Owner business; PDPO privacy) | Data Owner **A**; PDPO **A** |
| MDM operations | Conceptual model + one golden-record **example** | Registry occupancy for Patient/Provider — **not** a platform | Data Owner **A** |
| Lifecycle schedule | Decision chain; empty period field | Retention Schedule rows **without inventing periods** (placeholder + source citation) | Data Owner **A**; DMO |
| Forums | Cadence **design** (Phase 3) | Minutes / packs — not claimed | DGO secretariat; DMC |

**Already at Operational (project):** Metadata inventory and catalog samples (Phase 8 working pack); lineage register (Phase 9 working pack); this pack’s matrices and registers.

Organizational Operational evidence (real appointments, live systems) remains **not claimed** (Phase 14 lock).

---

## 4. Operational → Measured

No major artifact is assigned **Measured**.

| Gap | Why Measured is not justified | What Measured would require |
| --- | --- | --- |
| Metadata completeness | Inventory exists; `DG-KPI-004` has **no result** | Evidenced mandatory-field occupancy rate after a baseline |
| Lineage coverage | 13-row register exists; lineage KPI has **no result** | Evidenced Critical Lineage coverage vs MVP scope |
| Data quality | Sample pass/fail counts are labelled **not a Rafid score**; scorecard cells are illustrative | Repeated CDE results and a trend — still would be synthetic if produced; not claimed now |
| Ownership / stewardship coverage | Titles designed; `DG-KPI-001` / `002` have **no result** | Occupancy percentages after a baseline |
| Maturity | Empty template (`12-kpis-maturity/`) | A completed assessment with occupancy evidence — **not** an NDMO 100%/0% score |

---

## 5. Conceptual alignment → official verification

These items stay open. They are **not** resolved in this pack.

| Gap ID (Phase 14) | Theme | Working-pack pointer |
| --- | --- | --- |
| RHC-GAP-001 | Binding Standards version | `RHC-WP-VER-001` |
| RHC-GAP-002 | Uncopied controls / specifications | `RHC-WP-VER-004` |
| RHC-GAP-003 | Organizational Manual | `RHC-WP-VER-002` |
| RHC-GAP-004 | Official classification **names** | `RHC-WP-VER-005` |
| RHC-GAP-005 | Sharing Regulation | `RHC-WP-VER-011` |
| RHC-GAP-007 / 016 | Retention / legal clocks | `RHC-WP-VER-010` |
| RHC-GAP-008 / 015 | Healthcare overlay | `RHC-WP-VER-015` |
| RHC-GAP-009 | PDPL overlay | `RHC-WP-VER-012` |
| RHC-GAP-010 | NCA catalogue | `RHC-WP-VER-013` |
| RHC-GAP-019 | `DG.5` audit framework | `RHC-WP-VER-018` |

**Do not close these by assumption.**

---

## 6. Governance maturity gaps (portfolio, not NDMO levels)

| Area | Strongest project state | Maturity gap |
| --- | --- | --- |
| Strategy / operating model / policy | Designed | Approval and occupancy not claimed |
| Ownership / classification / DQ / MDM / lifecycle / KPIs | Designed | Working registers incomplete or absent |
| Metadata / catalog / lineage | Operational (project) | No measured KPI results |
| NDMO / PDPL | Designed mapping + verification registers | Official source confirmation open |
| Security (NCA) | Boundary only | Out of this pack except coordination |

---

## 7. What this analysis is not

- Not an NDMO gap analysis under `DG.2.1`
- Not a PDPL gap assessment
- Not a score
- Not permission to invent evidence to fill a row
