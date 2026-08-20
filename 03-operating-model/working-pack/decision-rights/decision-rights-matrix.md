# Decision-Rights Matrix (Applied Working Pack)

**Document ID:** RHC-DG-P3-WP-006  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** New organizational authority, new DMC classes, or named appointments

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Locked sources:** [`../../../02-governance-strategy/decision-rights.md`](../../../02-governance-strategy/decision-rights.md) · [`../../03-role-catalogue.md`](../../03-role-catalogue.md) · [`../../05-decision-escalation-model.md`](../../05-decision-escalation-model.md) · [`../../../04-ownership-stewardship/03-ownership-decision-matrix.md`](../../../04-ownership-stewardship/03-ownership-decision-matrix.md)

Machine-readable companion: [`decision-rights.csv`](decision-rights.csv).

---

## 1. Purpose

Record **who owns** important Rafid governance decisions, which forum records the decision, and where the case goes if it cannot close.

Decision classes remain Phase 2: **Strategic / Tactical / Operational**. Phase 3 already assigned altitude. This pack applies those classes to named decisions used in later phases.

No new executive authority is created. Residual beyond the Data Management Committee remains the **Cluster CEO (Executive Sponsor)** — already in the Phase 3 catalogue.

---

## 2. How to read a row

| Column | Meaning |
| --- | --- |
| Decision owner (A) | Exactly one Accountable role |
| Responsible | Who prepares the pack or implements |
| Consulted | Two-way input before the decision |
| Approval forum | Existing Phase 3 forum only — or “none (bilateral Owner decision logged in domain huddle)” |
| Escalation path | Locked Phase 3 hierarchy |
| Evidence / record | Existing Rafid artifact type — not a live minute |

Cadence of forums is Phase 3 design. **Proposed / Illustrative** as a live rhythm. Live decisions are not claimed.

---

## 3. Decision-rights matrix

| ID | Decision | Class | Decision owner (A) | Responsible | Consulted | Approval forum | Escalation path | Evidence / record |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| DG-DR-WP-001 | Approve Data Governance Framework / strategy | Strategic | DMC | CDO, DGO | ESC, DO, PDPO, CO, LEG, ODIA | Data Management Committee | DMC → Cluster CEO (unresolved / entity risk) | Strategy pack; DMC decision (designed — not live minutes) |
| DG-DR-WP-002 | Approve L3 Policy (POL-001) | Strategic | DMC | CDO, DGO | ESC, DO, CUST, PDPO, CO, LEG, ODIA | Data Management Committee | DMC → Cluster CEO | POL-001 approval record (designed) |
| DG-DR-WP-003 | Approve an enterprise Standard that does **not** change Policy intent | Tactical | CDO | DGO | DMC, DO, BDS, CUST | Steward Forum **recommends**; CDO approves | If the Standard would change Policy intent → DMC **A** (DG-DR-WP-002) | STD-001–005 approval (CDO) |
| DG-DR-WP-004 | Assign / ratify a Data Owner for a domain | Strategic | DMC | CDO, DGO | Proposed Owner | Data Management Committee | Unassigned domain / DMC deadlock → Cluster CEO (STD-001 / PRC-001) | Ownership Registry; Ownership Change Record |
| DG-DR-WP-005 | Accept a Business Data Steward nomination for a domain | Tactical / operational | Data Owner | DMO (registry completeness) | BDS (proposed), CUST (I) | Domain huddle; DMO records | Owner silent → DGO → CDO → DMC (Owner non-participation) | Steward Registry |
| DG-DR-WP-006 | Approve dataset classification or reclassification | Tactical (domain) | Data Owner | BDS | PDPO (if personal), CUST, DMO, LEG, ODIA† | Domain huddle | Owner silent → DMO → CDO → DMC. Security block on handling → CISO path **and** CDO (IT still not classification A) | Classification Registry; PRC-002 |
| DG-DR-WP-007 | Classification handling exception **inside** STD-002 (e.g. documented combination / linkage exception) | Tactical (domain) | Data Owner | BDS | PDPO, CUST, DMO | Domain huddle | If the request is **outside** Policy (skip Owner-approved classification) → PRC-006, DMC **A** | Classification Registry rationale |
| DG-DR-WP-008 | Resolve a cross-domain ownership or meaning dispute that Owners cannot settle | Strategic (when residual) | DMC (if meaning/risk remains contested) | DGO mediates; CDO decides **process** (who produces evidence by when) | Relevant DOs, BDS, CUST | DGO mediation → CDO process → Data Management Committee if still contested | DMC → Cluster CEO | Decision log; both Owners recorded; CDO does **not** pick a clinical definition unless the Committee delegates that case |
| DG-DR-WP-009 | Approve a governance exception to L3 Policy | Strategic | DMC | CDO, DGO | ESC, DO, PDPO, CO, LEG, CUST | Data Management Committee | Residual → Cluster CEO | Exception Request; DMC decision; Policy Exception Register; review/expiry date |
| DG-DR-WP-010 | Time-boxed waiver **inside** an already approved Policy envelope | Tactical | CDO | DGO | DO, PDPO, LEG, CUST | DMO / CDO (not a fifth forum); DMC **I** at next meeting | If outside Policy → DG-DR-WP-009 | Register entry; DMC information paper |
| DG-DR-WP-011 | Confirm Critical / prioritized lineage coverage for a flow in a domain | Tactical (domain) | Data Owner | BDS | DMO (method), CUST (technical facts) | Domain huddle; Steward Forum for cross-domain clash | Unresolved cross-domain hop → DGO → CDO → DMC (existing path only) | Lineage Registry / Critical Lineage Register (Phase 9 working pack) |
| DG-DR-WP-012 | Review governance KPIs (pack completeness and interpretation) | Tactical | CDO | DGO, BDS | DO, CUST, CO | DMO huddle (intake); Steward Forum (operational pack); DMC **reviews** executive pack as existing input | Missing evidence stays **not evidenced** — no invented result. Material ageing themes → DMC existing issue/exception path | KPI pack; Phase 12 working pack definition sheet |
| DG-DR-WP-013 | Accept in-policy residual data-quality risk | Operational / tactical | Data Owner | BDS, CUST | DMO, CON, PDPO (if personal-data quality) | Domain huddle | Care-safety or cluster-report residual, or Owner cannot accept within Policy → DMC (existing escalation). Out-of-policy → PRC-006 | Data Quality Issue Record; residual documented |
| DG-DR-WP-014 | Accept residual sharing / openness risk (novel, external, high-risk) | Strategic | DMC | CDO, DGO, DO | PDPO, LEG, CUST, ODIA | Data Management Committee | Residual DMC cannot settle → Cluster CEO. Material personal-data incident uses the **parallel** PDPO + CO + Legal path (CEO **A**) | Share decision; PRC-005; exception register if Policy is waived |
| DG-DR-WP-015 | Privacy compliance review of personal-data sharing | Tactical | PDPO | PDPO (review); BDS/DGO prepare the pack as **C** | DO, CDO, LEG | Not a fifth forum — recorded on the share pack; DMC I | Privacy incident → parallel notify; do not wait for quarterly DMC | PRC-005 privacy-review record. **Not** a PDPL compliance claim. |
| DG-DR-WP-016 | Confirm or decline CDE status | Tactical (domain) | Data Owner | BDS | CUST, DMO, PDPO‡ | Domain huddle | Owner non-participation or cross-domain deadlock → DMC (existing) | CDE Registry / Phase 7 catalogue row |

† ODIA consulted when the likely outcome is Public / open data.  
‡ PDPO consulted when privacy/security impact is material.

---

## 4. Decisions this pack does **not** reassign

| Decision | Stays with | Not moved to |
| --- | --- | --- |
| Business meaning / definition | Data Owner | DMO, IT, DMC (routine) |
| In-policy access | Data Owner | IT (IT provisions only) |
| Out-of-policy access | DMC | Data Owner self-exception |
| Catalog **programme** | CDO | Data Owner |
| Catalog **content** | Data Owner | CDO |
| Lineage **programme** | CDO | Data Owner |
| Lineage **business correctness** | Data Owner | CDO |
| NCA-aligned security control design | Cybersecurity / CISO path | DMO as substitute regulator |

---

## 5. What this matrix is not

- Not a new committee charter
- Not a voting scheme for DMC
- Not an invented executive (no extra “data council”)
- Not evidence that any decision has been taken live

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Phase 2 classes; Phase 3 decision/escalation model; Phase 4/6 rights | Rows |
| `[A]` | Illustrative Rafid decision labels | IDs |
| `[C]` | NDMO role **names** | Role column |
| `[NDMO verification required]` | Organizational Manual voting/duties; Sharing Regulation; PDPL | Not designed here |
