# Ownership Governance Controls

**Document ID:** RHC-DG-P4-007  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented (design recommendations)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose and labeling rule

These are **governance design recommendations** `[B]` for the fictional Rafid Health Cluster `[A]`.

**They are not NDMO controls.**  
**They must not be given NDMO control IDs.**  
**They are not evidence of NDMO implementation.**

NDMO later describes governance artifacts (for example decision and issue registers) in its Data Governance domain narrative `[C]` at domain level. Mapping any of the following to a specification-level ID is `[NDMO verification required]`. This file does not make that mapping.

---

## 2. Ownership Registry `[B]`

| Item | Design |
| --- | --- |
| **Purpose** | Single list of domains and the one Data Owner for each |
| **Held by** | DMO |
| **Minimum content** | Domain name; Owner title; Steward title; status; last review date |
| **Authority** | DMO maintains; DMC approves Owner changes |
| **Not** | An NDMO control number |

Year-1 content is the eight-row matrix in [`02-enterprise-ownership-matrix.md`](02-enterprise-ownership-matrix.md).

---

## 3. Steward Registry `[B]`

| Item | Design |
| --- | --- |
| **Purpose** | Record who executes stewardship per domain |
| **Held by** | DMO |
| **Minimum content** | As in [`05-stewardship-operating-model.md`](05-stewardship-operating-model.md) |
| **Authority** | Owner nominates; DMO registers |
| **Not** | An NDMO control number |

---

## 4. Periodic ownership review `[B]`

| Item | Design |
| --- | --- |
| **Purpose** | Confirm each domain still has one willing, correct Owner |
| **Cadence** | Periodic (tied to DMC meetings — not a numeric SLA) |
| **Performed by** | DMO prepares; DMC reviews exceptions |
| **Outputs** | Confirm, change (Change Record), or Unassigned-Domain Escalation |
| **Not** | An NDMO control number |

---

## 5. Ownership approval `[B]`

| Item | Design |
| --- | --- |
| **Purpose** | Formal acceptance of an Owner for a domain (initial or change) |
| **Accountable forum** | Data Management Committee |
| **Responsible** | CDO / DMO prepares the paper; proposed Owner concurs |
| **Not** | An NDMO control number |

Year-1 eight Owners in this phase are the **approved design** for the portfolio. Live DMC minutes are not claimed.

---

## 6. Ownership Change Record `[B]`

| Item | Design |
| --- | --- |
| **Purpose** | Traceable record of Owner/Steward/domain boundary changes |
| **Held by** | DMO |
| **Minimum content** | What changed; from/to titles; reason; DMC decision reference; date |
| **Not** | An NDMO control number |

---

## 7. Unassigned-Domain Escalation `[B]`

| Item | Design |
| --- | --- |
| **Purpose** | Prevent data sitting with no Owner, or with IT/DMO as default Owner |
| **Trigger** | Domain with no registered Owner; abolished Owner title; split remainder |
| **Path** | DMO flags → CDO → Data Management Committee → CEO if still unresolved |
| **Rule** | DMO and CIO **must not** be recorded as business Data Owner to “close” the gap |
| **Not** | An NDMO control number |

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 4 control list | Sections 2–7 |
| `[A]` | Rafid portfolio | Year-1 registry content source |
| `[C]` | NDMO Data Governance domain exists and mentions artifacts at domain narrative level | Why we still do not invent control IDs |
| `[NDMO verification required]` | Any future crosswalk of these recommendations to specification IDs | Explicitly not done |
