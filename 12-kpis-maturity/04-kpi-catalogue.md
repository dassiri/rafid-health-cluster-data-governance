# KPI Catalogue

**Document ID:** RHC-DG-P12-004  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (catalogue method); Data Owner **A** for domain interpretation  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual catalogue; fictional Rafid IDs; no live values.

**Phase:** 12 — KPIs and maturity  
**Does not decide:** Measured Rafid results

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document is the **conceptual KPI Catalogue** `[A]`.

**`DG-KPI-00n` identifiers are fictional Rafid IDs `[A]`. They are not NDMO control IDs.** Do not brief them as `DG.7.x`.

No value in this catalogue is real Rafid performance. Target Status uses exactly **To be established after baseline measurement.** unless an example is labeled **`[A] Illustrative Rafid target`**.

Evidence sources are **proposed artifacts**, not claimed live systems.

---

## 2. Catalogue fields (locked)

KPI ID · Name · Purpose · Definition · Calculation Logic · Unit · Frequency · Owner · Evidence Source · Domain · Leading/Lagging · Target Status · Notes/Limitations

---

## 3. Index

| KPI ID | Name | Set | Domain |
| --- | --- | --- | --- |
| DG-KPI-001 | Data Owner Assignment Coverage | Executive | Ownership |
| DG-KPI-002 | Business Data Steward Assignment Coverage | Executive | Stewardship |
| DG-KPI-003 | Classification Coverage Rate | Executive | Classification |
| DG-KPI-004 | Mandatory Metadata Completeness | Executive | Metadata / Catalog |
| DG-KPI-005 | CDE Quality Composite | Executive | Data Quality |
| DG-KPI-006 | Data Quality Issue Closure Rate | Executive | Issue / Exception |
| DG-KPI-007 | Critical Lineage Coverage | Executive | Lineage |
| DG-KPI-008 | Master Data Duplicate Resolution Rate | Executive | MDM |
| DG-KPI-009 | Retention Schedule Coverage | Executive | Lifecycle |
| DG-KPI-010 | Sharing Requests with Completed Privacy Review | Executive | Access / Sharing |
| DG-KPI-011 | Open Governance Exceptions | Executive | Issue / Exception |
| DG-KPI-012 | Critical Issue Aging | Executive | Issue / Exception |
| DG-KPI-013 | Governance Action Closure Rate | Supporting | Governance operating model |
| DG-KPI-014 | Year-1 Catalog Publication Coverage | Supporting | Metadata / Catalog |
| DG-KPI-015 | Critical Lineage Record Completeness | Supporting | Lineage |
| DG-KPI-016 | Master Entity Registry Occupancy | Supporting | MDM |
| DG-KPI-017 | Disposal Evidence Completeness | Supporting | Lifecycle |
| DG-KPI-018 | Restricted External Sharing Dual-A Completeness | Supporting | Access / Sharing |
| DG-KPI-019 | Exception Review Occupancy | Supporting | Issue / Exception |
| DG-KPI-020 | Executive KPI Evidence Pack Completeness | Supporting | Measurement / Improvement |

Executive set is **exactly 12** (DG-KPI-001–012). Supporting KPIs are catalogue-only unless CDO later proposes a swap under [25](25-kpi-change-management.md).

---

## 4. Executive definitions

### DG-KPI-001 Data Owner Assignment Coverage `[A]`

| Field | Content |
| --- | --- |
| Purpose | Confirm each Phase 4 domain has exactly one Data Owner title assigned |
| Definition | Share of the eight approved domains with a recorded Data Owner title on the Ownership Registry |
| Calculation Logic | (Domains with Owner title recorded ÷ 8) × 100 |
| Unit | Percent of domains |
| Frequency | Quarterly (DMC pack); exception path if vacant (existing Phase 4) |
| Owner | DMO **R** (registry); CDO oversight; DMC **I** — **no new A** |
| Evidence Source | Ownership Registry |
| Domain | Ownership |
| Leading/Lagging | Lagging (assignment state) |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | Titles only — not named incumbents. Does not prove the Owner is participating |

### DG-KPI-002 Business Data Steward Assignment Coverage `[A]`

| Field | Content |
| --- | --- |
| Purpose | Confirm Steward coverage for in-scope domains |
| Definition | Share of in-scope domains with at least one **Business Data Steward** recorded on the Steward Registry |
| Calculation Logic | (Domains with Steward recorded ÷ in-scope domains) × 100 |
| Unit | Percent of domains |
| Frequency | Quarterly |
| Owner | DMO **R**; Data Owner **A** for accepting Steward in the domain (Phase 4) |
| Evidence Source | Steward Registry |
| Domain | Stewardship |
| Leading/Lagging | Lagging |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | Role type is **Business Data Steward** only in this catalogue. No numeric steward FTE SLA |

### DG-KPI-003 Classification Coverage Rate `[A]`

| Field | Content |
| --- | --- |
| Purpose | Reduce unlabeled operational datasets |
| Definition | Share of in-scope catalog Datasets with an Owner-approved Rafid tier |
| Calculation Logic | (Classified in-scope Datasets ÷ in-scope Datasets) × 100 |
| Unit | Percent of datasets |
| Frequency | Monthly Steward Forum; quarterly DMC summary |
| Owner | Data Owner **A** (Phase 4 row 3); Business Data Steward **R**; DMO registry |
| Evidence Source | Classification Registry |
| Domain | Classification |
| Leading/Lagging | Lagging |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | Unlabeled is **not** Public (Phase 5). Tiers are **not** NDMO national names `[NDMO verification required]`. Classification does **not** set retention duration |

### DG-KPI-004 Mandatory Metadata Completeness `[A]`

| Field | Content |
| --- | --- |
| Purpose | Publish only assets that meet Phase 8 mandatory occupancy |
| Definition | Share of published operational catalog assets with all locked mandatory fields populated |
| Calculation Logic | (Published assets with mandatory fields complete ÷ published operational assets) × 100 |
| Unit | Percent of assets |
| Frequency | Monthly |
| Owner | Data Owner **A** for content; Business Data Steward **R**; DMO method |
| Evidence Source | Metadata Catalog |
| Domain | Metadata / Catalog |
| Leading/Lagging | Leading (enables discovery and other KPIs) |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | Mandatory fields as Phase 8 (including System / Primary System rule). Capability-dependent fields are **not** in this denominator |

### DG-KPI-005 CDE Quality Composite `[A]`

| Field | Content |
| --- | --- |
| Purpose | Give DMC a **CDE-level** quality signal without a cluster-wide index |
| Definition | For each in-scope measured CDE, the Phase 7 **optional unweighted average** of applicable dimensions. Executive reporting is the **set / status distribution** of those composites — **not** one enterprise quality number |
| Calculation Logic | Per CDE: unweighted mean of applicable dimension percentages (baseline always; dependents only if confirmed). A CDE is **not** “composite-acceptable” if any baseline dimension is in breach (Phase 7 mask prohibition). Executive rollup: (in-scope CDEs in acceptable composite status ÷ in-scope measured CDEs) × 100 |
| Unit | Percent of CDEs (status rollup); per-CDE composite remains a separate view |
| Frequency | Monthly domain huddle; quarterly DMC themes |
| Owner | Data Owner **A** for the CDE’s domain; Business Data Steward **R** |
| Evidence Source | Data Quality Scorecards |
| Domain | Data Quality |
| Leading/Lagging | Lagging (quality state) with leading use if used to prevent unsafe use |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | **No enterprise-wide single score. No arbitrary weights.** Thirteen illustrative CDEs in Phase 7 are **not** measured Rafid results. Does not replace per-dimension metrics |

### DG-KPI-006 Data Quality Issue Closure Rate `[A]`

| Field | Content |
| --- | --- |
| Purpose | Show whether quality issues complete the existing procedure |
| Definition | Share of DQ issues closed in the period among issues that were open or opened in that period (define cohort in the Definition Sheet) |
| Calculation Logic | (Issues closed in period ÷ (open at start + opened in period)) × 100 — cohort must be stated |
| Unit | Percent of issues |
| Frequency | Monthly Steward Forum |
| Owner | Data Owner **A** for closure in the domain (Phase 4 row 9); Business Data Steward **R** |
| Evidence Source | Data Quality Issue records (Phase 6 procedure path) |
| Domain | Issue / Exception |
| Leading/Lagging | Lagging |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | **No invented numeric SLA.** Procedure: `06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md` (title/path). Severity Critical/High/Medium/Low `[A][B]` reused |

### DG-KPI-007 Critical Lineage Coverage `[A]`

| Field | Content |
| --- | --- |
| Purpose | Confirm prioritized flows are on the Critical Lineage Register |
| Definition | Share of **confirmed** Critical Lineage candidates with a Critical Lineage Register entry |
| Calculation Logic | (Confirmed Critical Lineage items registered ÷ confirmed Critical Lineage items in scope) × 100 |
| Unit | Percent of confirmed items |
| Frequency | Monthly; quarterly DMC |
| Owner | Data Owner **A** for confirmation; Business Data Steward **R**; DMO method |
| Evidence Source | Lineage Register / Critical Lineage Register |
| Domain | Lineage |
| Leading/Lagging | Leading for change impact |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | Nine candidacy criteria do **not** auto-make Critical Lineage (Phase 9). Conceptual lineage only. Not real MOH/NPHIES architecture |

### DG-KPI-008 Master Data Duplicate Resolution Rate `[A]`

| Field | Content |
| --- | --- |
| Purpose | Show progress on duplicate **review outcomes**, not match-engine scores |
| Definition | Share of duplicate review cases closed (merged, split, or confirmed not-duplicate) in the cohort |
| Calculation Logic | (Duplicate cases resolved ÷ duplicate cases in cohort) × 100 |
| Unit | Percent of cases |
| Frequency | Monthly |
| Owner | Data Owner **A** for merge/split **intent** (Patient Access & Experience Director / Medical Affairs Officer for Core MDM); Business Data Steward **R** |
| Evidence Source | Duplicate Review Register; Master Entity Registry |
| Domain | MDM |
| Leading/Lagging | Lagging |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | **No numeric match thresholds** (Phase 10). Facility remains supporting-only. Not a physical hub KPI |

### DG-KPI-009 Retention Schedule Coverage `[A]`

| Field | Content |
| --- | --- |
| Purpose | Show in-scope assets/record types have a **registered Retention Rule** |
| Definition | Share of in-scope assets/record types with a Retention Rule ID on the Retention Schedule |
| Calculation Logic | (In-scope items with a Retention Rule ÷ in-scope items) × 100 |
| Unit | Percent of assets/record types |
| Frequency | Quarterly |
| Owner | Data Owner **A** (Phase 4 row 10); Business Data Steward **R**; DMO register |
| Evidence Source | Retention Schedule |
| Domain | Lifecycle |
| Leading/Lagging | Leading for later disposal eligibility |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | **Does not invent a retention period.** A placeholder period (`[NDMO verification required]` / `[Legal / regulatory verification required]`) may exist on the rule; coverage ≠ verified legal clock. Not a backup KPI |

### DG-KPI-010 Sharing Requests with Completed Privacy Review `[A]`

| Field | Content |
| --- | --- |
| Purpose | Protect the Phase 4 split: business approval ≠ privacy review |
| Definition | Share of personal-data sharing requests in the period with completed PDPO privacy compliance review |
| Calculation Logic | (Requests with PDPO review complete ÷ personal-data sharing requests) × 100 |
| Unit | Percent of requests |
| Frequency | Monthly |
| Owner | PDPO **A** for the privacy review (row 7); Data Owner **A** remains for business approval (row 6); DMO completeness of the **record** |
| Evidence Source | Access/Sharing Records |
| Domain | Access / Sharing |
| Leading/Lagging | Leading for lawful sharing practice |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | The two **A**s **shall not** be merged. Restricted external wording unchanged. PDPL mapping `[NDMO verification required]` |

### DG-KPI-011 Open Governance Exceptions `[A]`

| Field | Content |
| --- | --- |
| Purpose | Make exception load visible to DMC without a new decision class |
| Definition | Count of open entries on the Policy Exception Register at period end |
| Calculation Logic | Count (open status) |
| Unit | Count of exceptions |
| Frequency | Quarterly DMC (existing exception **A**); monthly Steward awareness |
| Owner | DMC remains **A** for Policy-level exceptions (existing); DMO register **R**; CDO recommends |
| Evidence Source | Exception Register |
| Domain | Issue / Exception |
| Leading/Lagging | Lagging |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | Procedure title/path only: `06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md`. **No new DMC decision right.** Count is not automatically “good” or “bad” without risk context |

### DG-KPI-012 Critical Issue Aging `[A]`

| Field | Content |
| --- | --- |
| Purpose | Surface stale Critical quality/governance issues |
| Definition | Age profile of open **Critical** severity issues (opened date → as-of date) |
| Calculation Logic | Report count of open Critical issues and their age in existing forum cycles (not an invented SLA clock). Optional: count still open beyond the last Domain huddle / Steward Forum at which they were due for Owner review — **cycle-based**, not a fabricated day-count target |
| Unit | Count; age described against Phase 3 forum cycles |
| Frequency | Weekly DMO triage list; monthly Steward Forum; quarterly DMC themes |
| Owner | Data Owner **A** for issue resolution; Business Data Steward **R**; DMO monitoring |
| Evidence Source | Data Quality Issue records; Governance meeting records |
| Domain | Issue / Exception |
| Leading/Lagging | Lagging with leading risk signal |
| Target Status | To be established after baseline measurement. |
| Notes/Limitations | **No invented numeric SLA** (no “close in n days”). Severity model reused from Phase 7 `[A][B]` |

---

## 5. Supporting definitions (summary)

| KPI ID | Purpose (short) | Unit | Frequency | Owner | Evidence | Leading/Lagging | Target Status |
| --- | --- | --- | --- | --- | --- | --- | --- |
| DG-KPI-013 | Closed forum actions ÷ actions due in period (not attendance) | Percent | Monthly / Quarterly by forum | CDO / DMO **R**; DMC **I** | Governance meeting records | Lagging | To be established after baseline measurement. |
| DG-KPI-014 | Published Year-1 asset types in MVP catalog domains | Percent | Monthly | Data Owner **A**; Business Data Steward **R** | Metadata Catalog | Leading | To be established after baseline measurement. |
| DG-KPI-015 | Critical Lineage records with required coarse fields | Percent | Monthly | Data Owner **A**; Business Data Steward **R** | Lineage Register | Leading | To be established after baseline measurement. |
| DG-KPI-016 | Patient and Provider master entities with required registry occupancy | Percent | Monthly | Relevant Core MDM Owner **A**; Business Data Steward **R** | Master Entity Registry | Leading | To be established after baseline measurement. |
| DG-KPI-017 | Closed disposals with a complete Disposal Record | Percent | Quarterly | Data Owner **A**; DMO register | Disposal Register | Lagging | To be established after baseline measurement. |
| DG-KPI-018 | Restricted external shares with both **A**s recorded | Percent | Monthly | Data Owner **A** + PDPO **A** (separate) | Access/Sharing Records | Leading | To be established after baseline measurement. |
| DG-KPI-019 | Open exceptions with review/compensating-control occupancy | Percent | Quarterly | DMO **R**; existing exception **A** | Exception Register | Leading | To be established after baseline measurement. |
| DG-KPI-020 | Executive KPIs with current evidence pointer in the Evidence Register | Percent | Quarterly | DMO **R** | KPI Evidence Register | Leading | To be established after baseline measurement. |

Supporting KPIs are `[A]`. They are **not** NDMO IDs. MVP catalog/lineage/MDM/lifecycle scopes remain as in Phases 8–11 (not redesigned).

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Catalogue IDs and definitions | Entire document |
| `[B]` | Evidence-based KPI practice | Fields |
| `[C]` | `DG.7` **name** as Phase 2 pointer only | Not implementation |
| `[NDMO verification required]` | Official NDMO KPI types | Not copied as Rafid formulas |
