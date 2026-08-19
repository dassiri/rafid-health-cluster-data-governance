# Lineage Criticality

**Document ID:** RHC-DG-P9-005  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** (confirm coverage in the domain); DMO (method) `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Nine criteria; two-step candidate/confirm; no numeric scoring.

**Phase:** 9 — Data lineage  
**Does not decide:** A scored criticality index; automatic Critical Lineage

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **how a flow becomes prioritized lineage** `[A][B]`.

There is **no numeric scoring**.

---

## 2. Decision rule (locked)

> A lineage candidate is identified when one or more criteria indicate material business impact or governance value. The Data Owner, Steward, and DMO then confirm whether prioritized lineage coverage is warranted.

| Step | Who | What happens |
| --- | --- | --- |
| 1. Identify candidate | Business Data Steward (with Custodian / consumers as needed) | One or more of the nine criteria fire. That **identifies a candidate**. It does **not** auto-make Critical Lineage. |
| 2. Confirm coverage | Data Owner, Steward, and DMO | Decide whether **prioritized lineage coverage** (typically Critical Lineage Register + Levels 1–2, deeper if warranted) is warranted **now**. |

Withdrawn: any wording that a single criterion **automatically** makes a flow Critical Lineage.

---

## 3. Nine criteria (locked) `[A][B]`

1. **Critical Data Element** — flow carries a confirmed Phase 7 CDE  
2. **Patient safety**  
3. **Regulatory impact** — only where a requirement is verified; otherwise `[NDMO verification required]` and do not invent a law  
4. **Financial impact**  
5. **Executive reporting**  
6. **Cross-domain dependency**  
7. **External data sharing**  
8. **Data quality history** — recurring defects on the path  
9. **Master data dependency** — identity or reference masters on the path (**not** Phase 10 architecture)

A criterion signals **candidacy**. It does **not** automatically make a flow Critical Lineage.

---

## 4. After confirmation

Confirmed prioritized coverage is recorded on the **Critical Lineage Register** ([`15-governance-artifacts.md`](15-governance-artifacts.md)). Unconfirmed candidates may still have coarse Phase 8 lineage metadata without Year-1 deep coverage.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Nine criteria; two-step rule | Sections 2–3 |
| `[C]` | Role **names**; Quality domain **name** (CDE as a Rafid construct linked to quality) | Context |
| `[NDMO verification required]` | Official NDMO lineage-criticality mandates; unverified “regulatory” claims | Not claimed |
