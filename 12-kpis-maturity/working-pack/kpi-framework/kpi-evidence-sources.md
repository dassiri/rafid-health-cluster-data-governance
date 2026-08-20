# KPI Evidence Sources (Working Pack)

**Document ID:** RHC-DG-P12-WP-003  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (documentation only)

**Does not decide:** Warehouses, pipelines, BI extracts, or live systems

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Responsible:** DMO · **Review:** CDO · **Approval:** CDO (method)

**Parent design:** [`../../17-kpi-data-sources.md`](../../17-kpi-data-sources.md)

---

## 1. Purpose

Map each KPI to **existing Rafid artifacts**. Do not create duplicate source systems. Do not claim these registers are live organizational systems.

**If source occupancy is empty, the KPI is not evidenced** — not 0% success and not 100% success.

---

## 2. Source map by scorecard area

### Data Quality

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-005 | Data Quality Scorecards (structure); CDE catalogue | `07-data-quality/11-scorecard-monitoring.md`; `07-data-quality/04-cde-catalogue.md` | Designed. Scorecard **cells** are illustrative | Designed |
| DG-KPI-WP-001 | Completeness dimension on in-scope CDEs | `07-data-quality/05-quality-rules.md`; Phase 7 scoring method | Designed | Designed |
| DG-KPI-WP-002 | Data Quality Rule Registry occupancy / execution | `07-data-quality/05-quality-rules.md` | Designed (rules documented; not executed as a live pass-rate process) | Designed |

`assets/practical-evidence/01-data-quality-example.md` is an 8-row **teaching extract** labelled not a Rafid score. It does **not** raise these KPIs to Operational or Measured.

The Phase 7 scorecard remains the CDE / dimension monitoring surface. This pack does not copy it.

### Ownership

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-001 | Ownership Registry (proposed); enterprise ownership matrix | `04-ownership-stewardship/`; STD-001 templates | Designed (titles documented; registry not occupied as working records) | Designed |
| DG-KPI-002 | Steward Registry (proposed); Phase 4 stewardship operating model | `04-ownership-stewardship/` | Designed | Designed |
| DG-KPI-WP-003 | Catalog Owner field on MVP assets | `08-metadata-catalog/working-pack/metadata-inventory/` | Operational (project) inventory rows exist | Designed — occupancy in a teaching inventory is not a measured KPI |

### Classification

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-003 | Classification Registry (proposed); catalog Classification field | `05-data-classification/`; `08-metadata-catalog/working-pack/metadata-inventory/` | Classification **model** Designed; catalog field occupancy is a synthetic working record | Designed |

Rafid tiers remain Public / Internal / Confidential / Restricted `[A][B]`. They are **not** NDMO national names `[NDMO verification required]`. Restricted volume is **not** used as a vanity KPI.

### Metadata

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-004 | Metadata Catalog; minimum metadata model | `08-metadata-catalog/working-pack/` | Operational (project) inventory and field model | Designed |
| DG-KPI-014 | Year-1 published asset types in MVP domains | `08-metadata-catalog/working-pack/data-catalog/catalog-mvp-scope.md` | Operational (project) MVP cut | Designed |

Mandatory publish fields remain Phase 8 (including Owner, Steward, Classification, Lifecycle Status). Capability-dependent fields are **not** in the DG-KPI-004 denominator.

### Lineage

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-007 | Critical Lineage Register | `09-data-lineage/working-pack/lineage-inventory/` | Operational (project) 13-row register | Designed |
| DG-KPI-015 | Critical Lineage record completeness (coarse fields) | Same register; `09-data-lineage/working-pack/quality/lineage-quality-checks.md` | Operational (project) | Designed |
| DG-KPI-WP-004 | Last Reviewed occupancy on Critical rows | Lineage register `Last Reviewed` (or equivalent) | Operational (project) dates are teaching dates | Designed |

A 13-row synthetic register is **not** a lineage coverage result for the cluster.

### MDM

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-008 | Duplicate Review Register; Master Entity Registry | `10-master-data-management/`; `assets/practical-evidence/04-mdm-golden-record-example.md` | Designed. Golden-record file is a teaching example, not an operating hub | Designed |
| DG-KPI-016 | Master Entity Registry occupancy (Patient / Provider) | Phase 10 registry design | Designed | Designed |

**No match-score source.** Numeric match thresholds remain forbidden.

### Lifecycle

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-009 | Retention Schedule | `11-data-lifecycle/` | Designed. Periods are verification placeholders | Designed |
| DG-KPI-017 | Disposal Register | Phase 11 disposal artifacts | Designed | Designed |
| DG-KPI-WP-005 | Catalog Lifecycle Status field | `08-metadata-catalog/working-pack/metadata-inventory/` | Operational (project) field occupancy | Designed |

DG-KPI-009 measures **rule registration**, not legal retention clocks `[Legal / regulatory verification required]`.

### Governance Issues

| KPI | Evidence source | Location | Project source state | KPI evidence state |
| --- | --- | --- | --- | --- |
| DG-KPI-006 | Data Quality Issue records | Phase 6 DQ issue procedure; Phase 7 issue path | Designed | Designed |
| DG-KPI-011 | Policy Exception Register | Phase 6 exception procedure | Designed | Designed |
| DG-KPI-012 | Critical issue records; governance meeting records | Issue path; Phase 3 forum design | Designed (no live minutes) | Designed |
| DG-KPI-019 | Exception review / compensating-control occupancy | Exception Register | Designed | Designed |
| DG-KPI-WP-006 | Open DQ issue stock | Same issue path as DG-KPI-006 | Designed | Designed |

Phase 14 working-pack risk rows are **governance risk**, not the DQ issue register. Do not double-count them as DG-KPI-WP-006.

### Related slices (not on the eight-area face)

| KPI | Evidence source | Location | KPI evidence state |
| --- | --- | --- | --- |
| DG-KPI-010 | Access / Sharing Records | Phase 4 rows 6–7; Phase 6 sharing procedure | Designed |
| DG-KPI-013 | Governance meeting records / action log | Phase 3 forums | Designed |
| DG-KPI-018 | Restricted external sharing dual-A record | Access / Sharing Records | Designed |
| DG-KPI-020 | KPI Evidence Register (proposed Phase 12 artifact) | This working pack plus [`../../26-governance-artifacts.md`](../../26-governance-artifacts.md) | Designed |

---

## 3. What is not a source

| Not a source | Why |
| --- | --- |
| Invented warehouse or Power BI dataset | No pipeline is implemented |
| Phase 7 illustrative scorecard numbers | Teaching cells, not a baseline |
| Catalog search-hit counts | Vanity |
| Backup job success | Backup ≠ retention |
| Match-engine scores | Forbidden by Phase 10 |
| NDMO specification IDs | `DG-KPI-00n` is a Rafid ID `[A]` |

---

## 4. Future measurement (not claimed now)

To promote a KPI from Designed to Measured **inside this repository**, all of the following would be required:

1. A stated cohort and period  
2. A populated source with a defined denominator  
3. Calculation under the locked formula  
4. KPI-input quality check passed  
5. Owner acceptance of the domain interpretation  
6. Label **synthetic** if the data are still portfolio records  

That cycle has **not** been run. **Measured remains unassigned.**

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Applied source map | Entire document |
| Phase 8–9 working packs; Phase 7; Phase 4–6, 10–11 | Evidence locations | Section 2 |
| `[NDMO verification required]` | Official NDMO evidence objects | Not claimed |
