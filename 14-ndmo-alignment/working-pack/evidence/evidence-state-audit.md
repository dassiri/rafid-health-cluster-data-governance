# Evidence State Audit

**Document ID:** RHC-DG-P14-WP-004  
**Phase:** 14 — NDMO alignment (working pack)  
**Status:** Implemented (audit of repository evidence only)

**Does not decide:** Organizational Operational or Measured status (Phase 14 remains **not claimed**)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

**Responsible:** DMO · **Review:** CDO · **Approval:** CDO (method)

---

## 1. Purpose

Apply the three **project evidence states** to major Rafid artifacts **as they exist in this repository**.

These states are **not** official NDMO maturity or compliance statuses.  
They are **not** the NDMO annual specification-level assessment `[C]`.

Organizational layer (locked in [`../../05-evidence-status-model.md`](../../05-evidence-status-model.md)):

| State | Organizational claim |
| --- | --- |
| Designed | **Yes** (Phases 0–14) |
| Operational | **Not claimed** |
| Measured | **Not claimed** |

This audit does **not** change that lock. It only records which **portfolio files** justify Designed vs applied working records (Operational) vs performance evidence (Measured).

**Rule:** use the strongest state **justified by files**. Do not promote on aspiration.

---

## 2. State definitions (project)

| State | Used when |
| --- | --- |
| **Designed** | Framework, policy, process, model, or schema is documented |
| **Operational** | Synthetic working records apply that design (inventory, register, sample catalog/lineage pages, this pack’s matrices) |
| **Measured** | Repeatable results exist (KPI value, quality trend, maturity score, before/after). Illustrative one-off numbers **do not** qualify |

---

## 3. Audit table

| Artifact | Evidence State | Evidence Location | Why This State | Verification Needed? |
| --- | --- | --- | --- | --- |
| Data Governance Framework | Designed | `02-governance-strategy/`; `06-policies-standards-procedures/policy/enterprise-data-governance-policy.md`; Phase 3 operating model | Vision, principles, policy, and RACI are documented. No approved live Policy, appointments, or minutes | Yes — `DG.1` / `DG.2` / `DG.4` completeness `[NDMO verification required]` |
| Data Ownership | Designed | `04-ownership-stewardship/` (matrix, RACI, lifecycle, controls) | Eight Owner titles and Steward types are designed. Ownership Registry is schema-level, not occupied working records | Yes — duty-level mapping `[NDMO verification required]` |
| Data Classification | Designed | `05-data-classification/`; STD-002; PRC-002 | Four-tier model, process, and examples exist. No occupied Classification Registry for the catalog MVP | Yes — official national **names** `[NDMO verification required]` |
| Data Quality Framework | Designed | `07-data-quality/` | Dimensions, 13 CDEs, rules, issue path, and scorecard **structure** exist. Scorecard cells are illustrative. `01-data-quality-example.md` is an 8-row teaching extract labelled **not a Rafid score** — that does **not** raise this artifact to Operational or Measured | Yes — official dimensions/thresholds `[NDMO verification required]` |
| Metadata Management | Operational | `08-metadata-catalog/` (design) plus `08-metadata-catalog/working-pack/` (inventory CSV/MD, field model, 25-term glossary) | Design is applied to **20** synthetic assets and glossary terms inside the portfolio | Yes — official MCM fields `[NDMO verification required]` |
| Data Catalog | Operational | Phase 8 catalog design plus `08-metadata-catalog/working-pack/examples/sample-catalog-assets.md` and catalog governance/MVP files | Sample catalog pages and registration path are applied working records. No catalog product is deployed | Yes — catalog control-level requirements `[NDMO verification required]` |
| Data Lineage | Operational | `09-data-lineage/` (design) plus `09-data-lineage/working-pack/` (13-row register, business/conceptual examples, selective field hops) | Design is applied to a synthetic Critical / Important / Standard register | Yes — official lineage mandates `[NDMO verification required]` |
| MDM | Designed | `10-master-data-management/`; `assets/practical-evidence/04-mdm-golden-record-example.md` | Conceptual MDM and one golden-record **example**. Example is not an operating hub, matching engine, or occupied master registry | Yes — official MDM specifications `[NDMO verification required]` |
| Data Lifecycle | Designed | `11-data-lifecycle/` | Create→Dispose principles, ownership, holds, archive, disposal, and retention **chain** exist. Periods are placeholders. No occupied Retention Schedule | Yes — `[NDMO verification required]` / `[Legal / regulatory verification required]` |
| Governance KPIs | Designed | `12-kpis-maturity/` (`DG-KPI-001`–`012`) | Metric definitions exist. **No results, baselines, or targets presented as Rafid performance** | Yes — official `DG.7` types `[NDMO verification required]` |
| Stakeholder Governance | Designed | `03-operating-model/` (roles, RACI, forums, escalation) | Forums and decision rights are documented. Cadence is design-only; no meeting evidence | Yes — Organizational Manual `[NDMO verification required]` |
| NDMO Mapping | Designed (locked Phase 14 map); Operational (project) for this pack’s mapping table and CSVs | `14-ndmo-alignment/02-ndmo-domain-map.md`; `03-artifact-to-domain-map.md`; `working-pack/ndmo/` | Locked files are the design map. This pack applies that map to later working packs as working records | Yes — uncopied IDs and regulations `[NDMO verification required]` |
| PDPL Considerations | Designed | `working-pack/pdpl/` plus existing PDPO / dual-A / personal-data indicator files | Governance considerations are documented. No legal interpretation, no operational privacy programme, no PDPL articles in sources | Yes — `[Legal / regulatory verification required]` / `[NDMO verification required]` |

**Measured:** not assigned.

---

## 4. Counts

| Project evidence state | Major artifacts in §3 |
| --- | --- |
| **Designed** | Data Governance Framework; Data Ownership; Data Classification; Data Quality Framework; MDM; Data Lifecycle; Governance KPIs; Stakeholder Governance; PDPL Considerations (**9**) |
| **Operational** | Metadata Management; Data Catalog; Data Lineage (**3**) |
| **Split** | NDMO Mapping — locked Phase 14 map remains **Designed**; this pack’s mapping table and CSVs are **Operational** (project working records) (**1** row) |
| **Measured** | None (**0**) |

---

## 5. What would be required to change a state

| From → To | Required evidence in this repository | Not sufficient |
| --- | --- | --- |
| Designed → Operational | Synthetic working register/inventory that applies the design | Another framework document |
| Operational → Measured | Repeatable result with method, date, and Owner; labelled synthetic if not live | One-off teaching extract; illustrative scorecard cell |
| Any → organizational Operational | Out of scope for a fictional cluster | This entire repository |

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Three-state project model | Entire audit |
| `[C]` | Domain/control **names** already recorded | Verification column |
| Phase 8–9 working packs; `assets/practical-evidence/` | Justification for Operational vs Designed | §3 |
