# Governance Evidence Traceability

**Document ID:** RHC-DG-P14-WP-005  
**Phase:** 14 — NDMO alignment (working pack)  
**Status:** Implemented (traceability only)

**Does not decide:** Compliance, certification, or closure of verification items

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

**Responsible:** DMO · **Review:** CDO · **Approval:** CDO (method)

---

## 1. Purpose

Show **Claim → Evidence → Verification → Status** for the statements this working pack is meant to support.

Every major claim traces to:

1. an existing Rafid artifact, and/or
2. a working-pack evidence item, and/or
3. an official source already recorded as `[C]`, or
4. an explicit **verification required** label.

Unsupported statements are not used.

---

## 2. CV-supporting claims (wording unchanged; evidence only)

These rows support existing CV statements. They do **not** rewrite the CV.

### Claim 1 — Conceptual NDMO mapping with open verification

*Mapped governance artifacts conceptually to relevant NDMO domains and documented verification requirements where official source-level confirmation remains open.*

| Step | Pointer |
| --- | --- |
| Claim | Conceptual mapping to NDMO **domain names** already in this repository; not specification-level compliance |
| Evidence | [`../ndmo/ndmo-governance-mapping.md`](../ndmo/ndmo-governance-mapping.md) (**20** rows); [`../ndmo/ndmo-evidence-matrix.csv`](../ndmo/ndmo-evidence-matrix.csv) (**22** evidence IDs) |
| Locked source | [`../../03-artifact-to-domain-map.md`](../../03-artifact-to-domain-map.md); [`../../02-ndmo-domain-map.md`](../../02-ndmo-domain-map.md) |
| Verification | [`../ndmo/ndmo-verification-register.csv`](../ndmo/ndmo-verification-register.csv) (**18** items); Phase 14 `RHC-VER-*` and `RHC-GAP-*` |
| Status | Conceptually aligned where domain **names** are `[C]`; **`[NDMO verification required]`** where official text, IDs, or regulations were not retrieved |

### Claim 2 — Designed / Operational / Measured evidence model

*Designed an evidence and verification approach distinguishing Designed, Operational, and Measured states.*

| Step | Pointer |
| --- | --- |
| Claim | Three project evidence states, distinct from NDMO assessment scoring |
| Evidence | This pack README §5; [`../evidence/evidence-state-audit.md`](../evidence/evidence-state-audit.md); evidence matrix column **Evidence State** |
| Locked source | [`../../05-evidence-status-model.md`](../../05-evidence-status-model.md) |
| Verification | Audit rule: Measured not assigned; Operational only where working records exist |
| Status | Model **Designed** and **applied** to 13 major artifacts; organizational Operational/Measured remain **not claimed** |

### Claim 3 — PDPL as governance input without compliance claim

*Incorporated PDPL and regulatory considerations as governance inputs without claiming legal or regulatory compliance.*

| Step | Pointer |
| --- | --- |
| Claim | PDPL is an L0 input; Personal Data Protection is an NDMO domain **name**; no legal compliance asserted |
| Evidence | [`../pdpl/pdpl-governance-considerations.md`](../pdpl/pdpl-governance-considerations.md) (**11** considerations); [`../pdpl/pdpl-evidence-matrix.csv`](../pdpl/pdpl-evidence-matrix.csv) |
| Locked source | Phase 2 policy hierarchy L0; PDPO **name** `[C]`; PRC-005 dual **A** |
| Verification | `RHC-WP-VER-012`; Phase 14 `RHC-GAP-009` |
| Status | Designed considerations; **`[Legal / regulatory verification required]`**; **no PDPL compliance claimed** |

---

## 3. Artifact-level traceability

| Claim (governance, not legal) | Rafid artifact | Working-pack evidence | Official source (if any) | Status |
| --- | --- | --- | --- | --- |
| Federated ownership exists as design | Phase 4 ownership matrix | `RHC-WP-EVD-003`; risk `RHC-WP-RSK-001` | BDE / Steward **names** `[C]` | Designed; verification required for duties |
| Four-tier classification exists as entity design | Phase 5 model | `RHC-WP-EVD-004`; `RHC-WP-RSK-002` | Four-level **concept**; `DC` `[C]` | Designed; national **names** `[NDMO verification required]` |
| Quality framework exists; performance is not measured | Phase 7 | `RHC-WP-EVD-006`–`007`; `RHC-WP-RSK-007` | Data Quality domain **name** `[C]` | Designed |
| Metadata is applied in a synthetic inventory | Phase 8 working pack | `RHC-WP-EVD-008`; `RHC-WP-RSK-003` | `MCM` **name** `[C]` | Operational (project); fields `[NDMO verification required]` |
| Lineage is applied in a synthetic register | Phase 9 working pack | `RHC-WP-EVD-010`; `RHC-WP-RSK-004` | None beyond catalog domain **name** | Operational (project); lineage specs `[NDMO verification required]` |
| Sharing uses two Accountable decisions | PRC-005; POL-001 | `RHC-WP-EVD-013`; `RHC-WP-PDPL-004` / `009`; `RHC-WP-RSK-008` | PDPO **name**; Sharing domain **name** `[C]` | Designed; regulation `[NDMO verification required]` |
| Retention periods are not invented | Phase 11 retention governance | `RHC-WP-EVD-012`; `RHC-WP-PDPL-006`; `RHC-WP-RSK-006` | `DG.6` **name** `[C]` only as pointer | Designed; periods verification required |
| KPIs are definitions only | Phase 12 catalogue | `RHC-WP-EVD-014`–`015`; `RHC-WP-RSK-011` | `DG.7` **name** `[C]` | Designed; no results |
| This pack is not `DG.5` | Phase 14 `RHC-VER-008` | `RHC-WP-VER-018`; `RHC-WP-RSK-010` | `DG.5` **name** `[C]` | Verification required; pack ≠ audit framework |
| PDPL is not claimed complete | L0 watchlist | `RHC-WP-EVD-019`; PDPL considerations | Domain **name** `[C]`; no articles in repo | Verification required |

---

## 4. Identifier families (do not confuse)

| Family | Meaning |
| --- | --- |
| `RHC-WP-EVD-*` | This pack’s evidence IDs `[A]` |
| `RHC-WP-VER-*` | This pack’s verification IDs `[A]` |
| `RHC-WP-PDPL-*` | This pack’s PDPL evidence IDs `[A]` |
| `RHC-WP-RSK-*` | This pack’s risk IDs `[A]` |
| `RHC-EVD-*` / `RHC-VER-*` / `RHC-GAP-*` | Locked Phase 14 IDs `[A]` |
| `DG.1`, `MCM`, `DC.3.2`, … | Official NDMO IDs **only** where already recorded `[C]` |
| `DG-KPI-00n` | Rafid KPI IDs `[A]` — **not** NDMO IDs |

---

## 5. What remains untraceable (by design)

| Topic | Why it has no `[C]` evidence row |
| --- | --- |
| Uncopied NDMO control IDs | Not in Phase 2 extract — **do not invent** |
| PDPL article obligations | Not in project sources |
| NCA control IDs | Not in this repository |
| Live Rafid performance | Fictional cluster; Measured not assigned |

Those items are labelled **verification required**, not filled.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | Recorded NDMO names/IDs | Official source column |
| `[A][B]` | Rafid artifacts and this pack | Evidence column |
| `[NDMO verification required]` / `[Legal / regulatory verification required]` | Open confirmation | Status column |
