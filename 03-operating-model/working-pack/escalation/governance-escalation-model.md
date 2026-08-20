# Governance Escalation Model (Applied Working Pack)

**Document ID:** RHC-DG-P3-WP-009  
**Phase:** 3 — Operating model (applied working pack)  
**Status:** Implemented (documentation and synthetic working records only)

**Synthetic / Illustrative / Non-production portfolio project.**

**Does not decide:** Numeric SLAs, a new executive authority, or a rewritten Phase 3 hierarchy

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Locked sources:** [`../../05-decision-escalation-model.md`](../../05-decision-escalation-model.md) · [`../../diagrams/escalation-flow.mmd`](../../diagrams/escalation-flow.mmd) · [`../../../04-ownership-stewardship/05-stewardship-operating-model.md`](../../../04-ownership-stewardship/05-stewardship-operating-model.md)

---

## 1. Purpose

Apply the locked Phase 3 escalation hierarchy to practical triggers used across ownership, classification, quality, lineage, exceptions, and NDMO/PDPL verification.

This file does **not** invent a new path. The Cluster CEO remains the residual executive. There is no extra “executive data council.”

Numeric SLAs were considered in Phase 4 and **rejected**. Ageing is qualitative.

---

## 2. Locked hierarchy (unchanged)

```text
Operational          Business Data Steward → Data Owner
     ↓ (cross-domain, qualitative ageing / Owner conflict)
Tactical             Data Governance Officer → CDO
     ↓ (policy, residual risk, material exception)
Strategic            Data Management Committee
     ↓ (unresolved / entity risk)
Executive            Cluster CEO (Executive Sponsor)
```

Parallel paths that **do not wait** for the quarterly Committee:

- Material regulatory / personal-data incident → parallel notify **PDPO + Compliance Officer + Legal Advisor**; CDO **R** coordinates; **CEO A** if material
- Cybersecurity incident → **CISO / NCA** path in parallel `[C]` Domain 15; CDO is coordinated, not a substitute regulator

---

## 3. Applied working path

```text
Domain issue / request
        ↓
Business Data Steward
        ↓
Data Owner
        ↓
DMO (Data Governance Officer mediate / completeness)
        ↓
CDO (process, in-policy waiver, programme)
        ↓
Data Management Committee
        ↓
Cluster CEO (existing residual / material regulatory A)
```

IT / Data Custodian implements **after** the business decision. A business-rule dispute returns to the **Data Owner**, not “IT decides.”

---

## 4. Escalation matrix

| Trigger | First hop | Then | Accountable if it leaves the domain | Record |
| --- | --- | --- | --- | --- |
| Cross-domain ownership or meaning conflict | Domain Stewards compare packs | Relevant Data Owners; **DGO mediates** | CDO decides **process**; **DMC A** if meaning/risk remains contested | Decision log. CDO does not pick a clinical definition unless the Committee delegates that case. |
| Critical / ageing data-quality issue (qualitative) | Steward cannot close | Data Owner | DGO (capacity/priority) → CDO → **DMC** if residual **care-safety or cluster-report** risk `[A]` / `[B]` | Data Quality Issue Record (PRC-003). **A stays Data Owner** until a Policy exception is invoked. |
| Classification dispute or unlabeled operational dataset | Steward assessment | Data Owner **A** for the tier | Owner silent → DMO → CDO → DMC. Security block on **handling** → CISO path **and** CDO (IT still not classification A) | Classification Registry (PRC-002) |
| Governance exception (outside Policy) | Requestor + Data Owner | DMO completeness; CDO recommend | **DMC A** (PRC-006) | Exception Request; register; review date |
| Time-boxed waiver **inside** Policy envelope | DMO completeness | **CDO A** | DMC **I** at next meeting | Register entry |
| Unresolved lineage issue (business meaning of a hop) | Steward of the asset’s domain | Data Owner **A** for business correctness | Cross-domain hop → DGO → CDO → DMC (existing only). Programme gaps stay CDO **A** | Lineage Registry |
| Regulatory / NDMO verification issue | Anyone may raise | Parallel PDPO + CO + Legal where personal/regulatory; DMO records the verification gap | **Material:** CEO **A**, CDO **R**. **Non-material:** CDO **A**. DMC **I** | Phase 14 verification register (project). Not an NDMO compliance claim. |
| Repeated overdue governance action / Owner unresponsive | Steward → DGO ageing list | CDO | **DMC** (Owner non-participation — existing DMC decision type) | Ageing list; DMC action. No numeric SLA. |
| Out-of-policy access request | Steward pack | **Not** Owner self-approval | **DMC A** (Phase 4 row 5; PRC-006) | Exception register |
| Privacy incident | Parallel notify — do not wait for DMC | CDO coordinates work | **CEO A** if material | Incident path; Committee informed |
| Custodian security refusal | Custodian | CISO path **and** CDO (dual) | Business meaning still returns to Data Owner | Implementation refusal note |

---

## 5. What does **not** escalate to DMC

| Case | Stays with |
| --- | --- |
| Routine definition, in-policy access, routine share, classification application | Data Owner |
| Catalog/lineage **content** completeness | Data Owner (content) / CDO (programme method) |
| In-policy quality residual the Owner accepts | Data Owner (PRC-006: not an exception) |
| Intake routing | DMO operations huddle |
| Standard proposal that does not change Policy | CDO (Steward Forum recommends) |

---

## 6. Illustrative Rafid examples `[A]`

Examples are synthetic. They are **not** live tickets.

| Example | Trigger | Path |
| --- | --- | --- |
| Duplicate Patient identifier (CDE-001 / CDE-002) ageing across registration and claims | Ageing quality issue with cross-domain use | HIM/Registration Stewards → Patient Access Owner **A** → if claims residual remains, DGO mediates with CFO Owner → CDO process → DMC only if care-safety or cluster-report residual |
| Encounter notes proposed Internal by operations, Restricted by HIM | Classification dispute | HIM Steward pack → CMO **A** → PDPO **C** (personal/health) → Custodian implements handling. No IT classification A. |
| Patient Access and CMO disagree who owns “attending clinician on the encounter” | Cross-domain ownership | Both Stewards → both Owners → DGO mediate → CDO sets evidence deadline → DMC if still contested. Phase 4 consulted extras remain **C**, not a second **A**. |

---

## 7. What this file does not do

- Does not add a hospital board hop
- Does not give CDO domain meaning **A**
- Does not invent numeric SLAs
- Does not claim forums have met

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Phase 3 decision and escalation model | Hierarchy and paths |
| `[A]` | Care-safety / cluster-report examples; CDE illustrations | Section 6 |
| `[C]` | Domain 15 NCA note; CDO-led assessment description | Parallel cyber and regulatory paths |
| `[NDMO verification required]` | Regulation-level procedures; definition of “material” | Phase 6 / legal — not invented here |
