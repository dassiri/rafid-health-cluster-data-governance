# Decision and Escalation Model

**Document ID:** RHC-DG-P3-005  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Policy exception envelopes (Phase 6) or domain SLAs (Phase 4 / 7)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved decision path and escalation hierarchy for the fictional Rafid Health Cluster `[A]`. It applies Phase 2 classes `[B]`: operational → Owner; tactical → DMO/CDO; strategic → Data Management Committee; residual → CEO.

Diagram: [`diagrams/escalation-flow.mmd`](diagrams/escalation-flow.mmd).

---

## 2. Escalation hierarchy `[B]`

```text
Operational          Business Data Steward → Data Owner
     ↓ (cross-domain, SLA breach, or Owner conflict)
Tactical             Data Governance Officer → CDO
     ↓ (policy, residual risk, material exception)
Strategic            Data Management Committee
     ↓ (unresolved / entity risk)
Executive            Cluster CEO (Executive Sponsor)
```

---

## 3. Normal decision path

Consumer or system detects an issue/request → **Business Data Steward** (intake, evidence) → **Data Owner** decides if in-policy → **Data Custodian** implements if technical → **Data Governance Officer** logs the outcome (when registers exist) → monitor.

This is operational class unless the case meets a path below.

---

## 4. Cross-domain conflict path

Two Owners disagree (for example identity vs laboratory identifiers) → **DGO** mediates with both Stewards → if unresolved, **CDO** decides **process** (who must produce evidence by when) → if meaning/risk remains contested, **Data Management Committee**.

The CDO does **not** pick a clinical definition in place of Owners unless the Committee delegates that case.

---

## 5. Policy exception path

Requester + Data Owner submit an exception pack (risk, duration, compensating control) → **DGO** completeness check → **CDO** recommend → **Data Management Committee A** for L3 policy exceptions.

Time-boxed operational waivers **inside** an approved policy envelope: **CDO A**, Committee **I** at the next meeting. The envelope itself is defined in Phase 6 — not written as policy here.

---

## 6. Unresolved data-quality issue escalation

Business Data Steward cannot close within domain SLA → **Data Owner** · if still open → **DGO** (capacity/priority) → **CDO** · if residual **care-safety or cluster-report** risk `[A]` / `[B]` → **Data Management Committee**.

IT fixes stay **R = Custodian**. **A stays Data Owner.**

---

## 7. Regulatory / compliance escalation

Anyone may raise → **parallel notify** PDPO + Compliance Officer + Legal Advisor (do not wait for the quarterly Committee) → **CDO R** coordinates.

| Case | Accountable | Responsible |
| --- | --- | --- |
| **Material** (personal-data incident, regulator inquiry, assessment dispute) | Executive Sponsor (CEO) | CDO (leads the work) |
| **Non-material** (routine query, interpretation request) | CDO | DGO / CO / PDPO / Legal as needed |

NDMO describes the CDO as leading the annual compliance exercise `[C]`. That is why the CDO **leads the work**. It is not a claim that Rafid has run the exercise.

Cybersecurity incidents follow the **CISO / NCA** path in parallel. NDMO Domain 15 is under NCA mandate `[C]`. The CDO is coordinated, not a substitute regulator.

The Data Management Committee is **informed**. It does not delay incident notification.

---

## 8. Intentionally unresolved

- Numeric SLAs for quality issues — later phases
- Written definition of “material” for incidents — Phase 6 / legal
- Sharing-regulation step-by-step procedure `[NDMO verification required]`

---

## 9. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 Implementation Brief | Paths and hierarchy |
| `[C]` | NDMO Standards v1.5 — CDO-led assessment description; Domain 15 NCA | Parallel cyber path; CDO leads assessment work |
| `[A]` | Care-safety / cluster-report risk examples | When quality issues leave the domain |
| `[NDMO verification required]` | Regulation-level procedures | Not retrieved |
