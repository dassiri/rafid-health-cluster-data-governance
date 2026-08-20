# Stakeholder Decision Flows

**Document ID:** RHC-DG-P3-WP-010  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** New procedures, new Accountable cells, or live case outcomes

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Locked sources:** [`../../07-operating-workflow.md`](../../07-operating-workflow.md) · PRC-001–006 · Phase 4 decision matrix · Phase 9 lineage ownership

---

## 1. Purpose

Show how locked roles, forums, and RACI cells operate on **named Rafid cases**. Each flow reuses an existing procedure or Phase 3 path. None is a new SOP.

Identifiers below are fictional working-pack IDs `[A]`. They are not NDMO control IDs and not live tickets.

---

## 2. Example 1 — Data quality issue

**Case ID:** FLOW-DQ-001 `[A]`  
**Domain:** Patient / Person Master Data  
**CDE:** CDE-001 National ID / CDE-002 Patient identifier  
**Issue:** Duplicate patient registration records appearing in encounter and claims extracts.

```text
Data Quality Issue
→ Steward Review
→ Owner Decision
→ DMO Coordination (if ageing or cross-domain use)
→ Escalation if unresolved
→ Forum Decision (only if residual leaves the domain / Policy)
→ Resolution Record
```

| Step | Who | What happens |
| --- | --- | --- |
| Log | Consumer, Steward, or Custodian | Data Quality Issue Record (PRC-003) |
| Triage | DMO routing; Head of Patient Registration & Access | Confirm owning domain = Patient / Person Master |
| Investigate | Steward **R**; MPI / registration Custodian **R** for technical duplicate evidence | Match/split facts; do not invent a match threshold |
| Decide | Patient Access & Experience Director **A** | Fix, merge/split intent, or accept in-policy residual |
| Implement | Custodian in existing systems | Technical remediation only |
| Verify / close | Steward verifies; Owner **A** closes | Residual documented if accepted |
| Escalate if needed | Steward → Owner → DGO → CDO → DMC | Cross-domain claims impact: CFO Owner is **C**, not a second **A**. Care-safety or cluster-report residual → DMC. Out-of-policy → PRC-006. |

**RACI:** DG-RACI-WP-007. **A stays Data Owner.** IT does not close the business issue as Owner.

---

## 3. Example 2 — Classification dispute

**Case ID:** FLOW-CL-001 `[A]`  
**Domain:** Clinical / Medical Records Data  
**Asset:** Encounter clinical notes (catalog MVP class)  
**Dispute:** Operations propose **Internal**; HIM proposes **Restricted**.

```text
Classification Question
→ Steward Assessment
→ Data Owner Review
→ DMO completeness / PDPO consult (personal/health)
→ Decision (Owner A)
→ Record / Update
```

| Step | Who | What happens |
| --- | --- | --- |
| Identify dataset | Head of HIM; EMR Custodian **C** | Same unit as PRC-002; unlabeled ≠ Public |
| Propose | Steward | Highest-impact narrative; **no score**; PDPO **C** (health data) |
| Decide | CMO **A** | Approve Rafid tier (Public / Internal / Confidential / Restricted) `[A][B]` |
| Registry | Steward **R**; DMO completeness | Classification Registry |
| Implement handling | Custodian **R** | Does **not** pick the tier. Security block → CISO path **and** CDO |
| Reclassification | Only CMO **A** | Steward flags triggers; downward move needs explicit rationale |

If someone asks to **skip** Owner-approved classification, that is **not** this flow — it is PRC-006 (**DMC A**).

A documented combination/linkage exception **inside** STD-002 remains **Owner A** (DG-DR-WP-007).

**RACI:** DG-RACI-WP-005.

---

## 4. Example 3 — Cross-domain ownership conflict

**Case ID:** FLOW-OWN-001 `[A]`  
**Conflict:** Who is Accountable for “attending clinician recorded on the encounter” when the same identifier is used in credentialing (Provider) and billing (Claims)?

Phase 4 already names **one Owner per domain**. The encounter documentation field sits in **Clinical / Medical Records** (CMO **A**). Provider identifier as a master sits in **Provider / Clinician Data** (Medical Affairs Officer **A**). Claims use is **Financial** (CFO **A**) as a **consumer** of those fields — not a second clinical Owner.

```text
Conflict
→ Domain Stewards
→ Relevant Data Owners
→ DMO (DGO mediates)
→ CDO (process: who must produce evidence by when)
→ DMC if unresolved
→ Decision
→ Governance Record
```

| Step | Who | What happens |
| --- | --- | --- |
| Surface clash | HIM Steward + Credentialing Coordinator + Revenue Cycle Manager | Steward Forum clash detection (recommend only) |
| Domain positions | CMO; Medical Affairs Officer; CFO | Each Owner speaks only for their domain. Consulted extras (Phase 4) remain **C**, never a second **A**. |
| Mediate | DGO | Completeness of evidence; no rewrite of clinical meaning |
| Process | CDO | Deadline and pack standard — **not** a picked clinical definition |
| Residual | DMC **A** if meaning/risk remains contested | Existing DMC class only |
| Record | DMO | Decision log; Ownership Registry unchanged unless PRC-001 is invoked |

The CDO does **not** become Data Owner of laboratory or encounter meaning.

**RACI:** DG-RACI-WP-004 only if ownership **reassignment** is required; otherwise Phase 3 cross-domain path (DG-DR-WP-008).

---

## 5. Example 4 — Governance exception

**Case ID:** FLOW-EX-001 `[A]`  
**Request:** Publish a Year-1 catalog Dataset without an Owner-accepted business definition, to unblock a management dashboard.

Catalog publish rules require Owner-accepted definition (Phase 8 working pack / PRC-004). Skipping that rule is **outside** POL-001 / STD-004 — not an in-policy waiver.

```text
Exception Request
→ Steward
→ Data Owner
→ DMO Review
→ Existing Approval Authority (DMC A)
→ Record
→ Review Date
```

| Step | Who | What happens |
| --- | --- | --- |
| Request | Requestor + Data Owner (CMO for a clinical Dataset) | Governance Exception Request: risk, duration, compensating control, classification |
| Justification | Requestor | Why the definition cannot be completed; compensating discovery limits |
| DMO review | DGO completeness; CDO recommend | PDPO **C** if personal; Legal **C** if legal risk. Not a substitute DMC vote. |
| Decide | **DMC A** (CEO chairs) | Approve, deny, or approve time-boxed |
| Register / monitor | DMO register; Steward / DMO monitor | Compensating controls still in place |
| Close / renew | DMC **A** to renew; DMO closes when expired and not renewed | Change Record |

If the request were a **time-boxed waiver inside** an already approved Policy envelope, **CDO A** and DMC **I** at the next meeting (DG-RACI-WP-018). This example is outside Policy, so DMC remains **A**.

The Owner **cannot** self-approve the skip.

**RACI:** DG-RACI-WP-014. Procedure: PRC-006.

---

## 6. Example 5 — Data Owner appointment (supporting)

**Case ID:** FLOW-AP-001 `[A]`  
**Need:** Record the Year-1 Patient / Person Master Owner seat (design map already in Phase 4).

```text
Nomination → DMO Review → DMC ratification → Registry update
```

| Step | Who | What happens |
| --- | --- | --- |
| Nominate | CDO or CEO for a vacant seat | Title: Patient Access & Experience Director; Steward: Head of Patient Registration & Access; confirm no second **A**; IT not proposed as Owner |
| Review | DMO | Domain exists on the Phase 4 list; DMO not proposed as business Owner |
| Ratify | **DMC A** | Approve or deny |
| Registry | DMO | Ownership Registry; Steward Registry; Ownership Change Record |

Live minutes are not claimed. Year-1 eight assignments in STD-001 remain the **approved design map**.

**RACI:** DG-RACI-WP-004. Procedure: PRC-001.

---

## 7. Example 6 — Critical lineage confirmation (supporting)

**Case ID:** FLOW-LIN-001 `[A]`  
**Flow:** Patient identity → Encounter → Claims (Phase 9 working-pack hops).

```text
Lineage candidate
→ Steward draft
→ Owner confirms business meaning / coverage
→ DMO method / register
→ Custodian technical facts
→ Record (Critical vs Important vs Standard label)
```

| Hop | Source Owner (A for source) | Target Owner (row primary) |
| --- | --- | --- |
| Patient → Encounter | Patient Access & Experience Director | CMO |
| Encounter → Claims | CMO | CFO |

One Owner **per asset**, not one Owner for the whole chain. DMO coordinates. No shared **A**. DMC does **not** approve every lineage record.

**RACI:** DG-RACI-WP-008 (business meaning) + DG-RACI-WP-017 (programme).

---

## 8. What these flows do not do

- Do not invent a new procedure ID
- Do not give IT classification or ownership **A**
- Do not merge PDPO privacy **A** with Owner business-sharing **A**
- Do not treat synthetic cases as operational evidence of a live organization

---

## 9. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Phase 3 workflow; Phase 6 procedures | Step order |
| `[A]` | CDE IDs; Owner titles; catalog/lineage MVP domains | Cases |
| `[C]` | Role **names** | Actors |
| `[NDMO verification required]` | Sharing regulation; PDPL overlay | Not used as flow law |
