# Workstream Deliverables

**Document ID:** RHC-DG-P13-012  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (catalogue of workstreams)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Twelve workstreams; eight Owner titles only.

**Phase:** 13 — Implementation roadmap  
**Does not decide:** Named incumbents

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

Per-workstream pack. **Primary Owner** is a **role type**.

**Eight Phase 4 Data Owner titles only:** Patient Access & Experience Director; Chief Medical Officer (CMO); Medical Affairs Officer; Chief Financial Officer (CFO); HR Director; Supply Chain Director; Chief Quality & Patient Safety Officer (CQPSO); Strategy & Planning Director.

Steward: **Business Data Steward**.

Evidence of completion below is **illustrative exit intent** — **not** current Rafid evidence.

---

## 2. WS1 — Governance Mobilization (Phase 3)

| Field | Content |
| --- | --- |
| Objective | Stand up forums and DMO routing |
| Activities | Confirm CEO chair; schedule DMC/Steward Forum/huddles; DMO intake |
| Deliverables | Forum calendar; intake log schema |
| Dependencies | None (hard start) |
| Primary Owner | CDO |
| Supporting roles | DGO secretariat; CIO; PDPO; Compliance Officer |
| Evidence of completion | Minutes exist; huddles logged |
| Risks | Executive sponsorship weakness |
| Exit criteria | Gate 1 |

---

## 3. WS2 — Ownership & Stewardship (Phase 4)

| Field | Content |
| --- | --- |
| Objective | Activate one Owner per domain and **Business Data Steward** coverage |
| Activities | Appoint to the eight titles; populate Ownership/Steward Registries |
| Deliverables | Occupied registries; onboarding |
| Dependencies | WS1 |
| Primary Owner | CDO / DMO (registry); each Data Owner **A** in domain |
| Supporting roles | Business Data Steward; Custodian |
| Evidence of completion | DG-KPI-001/002 occupancy (when measured — not claimed now) |
| Risks | Unclear ownership; steward capacity |
| Exit criteria | Gate 2 |

---

## 4. WS3 — Policy / Standards / Procedures Adoption (Phase 6)

| Field | Content |
| --- | --- |
| Objective | Adopt the existing 1+5+6 stack as organizational documents |
| Activities | DMC Policy approval (existing **A**); CDO Standards/Procedures; awareness |
| Deliverables | Approval/publication/review records (**potential** — not claimed) |
| Dependencies | WS1; parallel with WS4/WS5 |
| Primary Owner | CDO; DMC **A** for POL-001 (existing) |
| Supporting roles | DMO; PDPO **C** where personal data |
| Evidence of completion | Controlled copies; exception path used not invented |
| Risks | Resistance to governance |
| Exit criteria | M3; contributes to Gate 3 |

---

## 5. WS4 — Data Classification (Phase 5)

| Field | Content |
| --- | --- |
| Objective | Apply Rafid Public / Internal / Confidential / Restricted `[A][B]` |
| Activities | Classify in-scope datasets; Registry occupancy; unlabeled ≠ Public |
| Deliverables | Classification Registry occupancy |
| Dependencies | WS2 (hard); before WS10 |
| Primary Owner | Data Owner **A** (domain) |
| Supporting roles | Business Data Steward **R**; DMO method |
| Evidence of completion | Classified MVP datasets |
| Risks | Treating Rafid tiers as NDMO national names |
| Exit criteria | Gate 3 (with policy); M4 |

---

## 6. WS5 — Data Quality (Phase 7)

| Field | Content |
| --- | --- |
| Objective | Operate the **13 illustrative CDEs** only — **do not add CDEs** |
| Activities | Issue procedure; scorecards conceptual; no enterprise index |
| Deliverables | Issue/RCA/remediation records (when live) |
| Dependencies | WS1; soft WS6; parallel WS3 |
| Primary Owner | Data Owner **A** of the CDE’s domain |
| Supporting roles | Business Data Steward **R**; Custodian technical |
| Evidence of completion | MVP CDE process running |
| Risks | Poor data quality; fake enterprise score |
| Exit criteria | Gate 4; M5 |

MVP CDE domains include the eight Phase 4 titles as already listed in Phase 7 — **no new CDEs**.

---

## 7. WS6 — Metadata & Catalog (Phase 8)

| Field | Content |
| --- | --- |
| Objective | Catalog MVP for **three domains only** |
| Activities | Register Dataset / Master Data Entity with mandatory fields |
| Deliverables | Conceptual catalog occupancy — **no platform named** |
| Dependencies | WS2 + WS4 (hard) |
| Primary Owner | Patient Access & Experience Director; CMO; CFO (MVP domains) |
| Supporting roles | Business Data Steward; DMO |
| Evidence of completion | Mandatory metadata complete on MVP assets |
| Risks | Incomplete metadata; tool-first |
| Exit criteria | Gate 5; M6 |

---

## 8. WS7 — Data Lineage (Phase 9)

| Field | Content |
| --- | --- |
| Objective | Priority / Critical Lineage for Year-1 focus |
| Activities | Confirm candidates (nine criteria ≠ auto-critical); coarse records |
| Deliverables | Critical Lineage Register occupancy |
| Dependencies | Soft WS6; WS2 |
| Primary Owner | Data Owner **A** for confirmed flows |
| Supporting roles | Business Data Steward; DMO |
| Evidence of completion | M7 |
| Risks | Scanner-first; fake MOH/NPHIES architecture |
| Exit criteria | Gate 6 (lineage portion) |

---

## 9. WS8 — Master Data Management (Phase 10)

| Field | Content |
| --- | --- |
| Objective | MDM MVP: Patient + Provider **primary**; Facility **supporting only** |
| Activities | Logical golden record; conceptual match; duplicate review — **no engine** |
| Deliverables | Master Entity Registry occupancy; Duplicate Review Register |
| Dependencies | Soft WS6; WS2 |
| Primary Owner | Patient Access & Experience Director; Medical Affairs Officer |
| Supporting roles | Business Data Steward; Custodian; Strategy & Planning Director (Facility supporting) |
| Evidence of completion | M8 |
| Risks | Third full MDM workstream; match-score vanity |
| Exit criteria | Gate 6 (MDM portion) |

---

## 10. WS9 — Data Lifecycle (Phase 11)

| Field | Content |
| --- | --- |
| Objective | Lifecycle foundation on three MVP domains; **no invented retention periods** |
| Activities | Register Retention Rules with verification placeholders; hold/archive/disposal **schemas** |
| Deliverables | Retention Schedule occupancy (period still `[NDMO verification required]` / `[Legal / regulatory verification required]`) |
| Dependencies | WS2; WS4 does **not** set duration |
| Primary Owner | Patient Access & Experience Director; CMO; CFO (MVP) |
| Supporting roles | Business Data Steward; DMO; PDPO **C** if personal data |
| Evidence of completion | M9 |
| Risks | Inventing clocks; archive = backup |
| Exit criteria | Gate 6 (lifecycle portion) |

---

## 11. WS10 — Data Access / Sharing Governance (Phase 4 / 6)

| Field | Content |
| --- | --- |
| Objective | Operate two **A**s: Owner business; PDPO privacy where personal data |
| Activities | Sharing records; Restricted external dual-A wording unchanged |
| Deliverables | Access/Sharing Records occupancy |
| Dependencies | WS4 (hard); WS2 |
| Primary Owner | Data Owner **A** (business); PDPO **A** (privacy review) |
| Supporting roles | Business Data Steward; DMO completeness of the record |
| Evidence of completion | Dual-A completeness on personal-data shares |
| Risks | Merging the two **A**s |
| Exit criteria | Contributes to Gate 3/7 as sharing evidence |

---

## 12. WS11 — KPI / Maturity Measurement (Phase 12)

| Field | Content |
| --- | --- |
| Objective | Baseline Phase 12 executive KPIs; no fake results |
| Activities | Evidence Register; “not evidenced” until real occupancy; optional maturity narrative |
| Deliverables | Baseline pack **or** explicit gaps |
| Dependencies | Parallel from Day 1 |
| Primary Owner | DMO / CDO |
| Supporting roles | Data Owners; Business Data Steward |
| Evidence of completion | M10; M11 (`[A]` Illustrative assessment only) |
| Risks | Lack of baseline; KPIs used as auto-maturity |
| Exit criteria | Gate 7 |

---

## 13. WS12 — NDMO Evidence & Alignment (cross-phase)

| Field | Content |
| --- | --- |
| Objective | Keep verification discipline; prepare evidence **without** claiming compliance |
| Activities | Maintain gap register hygiene; do not invent IDs |
| Deliverables | Updated verification notes (Designed) |
| Dependencies | Continuous |
| Primary Owner | DMO / CDO |
| Supporting roles | PDPO; Compliance Officer; Legal Advisor (as Phase 3 types) |
| Evidence of completion | Gaps still labeled `[NDMO verification required]` where unresolved |
| Risks | Weak evidence discipline; fake compliance |
| Exit criteria | Ongoing; M12 includes alignment status |

This workstream **does not modify Phase 14 files**. It does **not** create new NDMO controls.

---

## 14. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Workstream packs | Sections 2–13 |
| `[C]` | Role **names** | Supporting roles |
| `[NDMO verification required]` | Official WS12 requirements | WS12 |
