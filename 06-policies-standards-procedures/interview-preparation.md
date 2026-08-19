# Interview Preparation — Phase 6

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P6-INT  
**Phase:** 6 — Policies, standards, and procedures  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Why one Data Governance Policy instead of multiple policies?

One L3 Policy keeps **must/must not** in a single DMC-owned document `[B]`. Multiple enterprise data policies fragment authority (IT policy vs HIM policy vs quality policy) and recreate silos the federated model was meant to stop. Topic depth belongs in **five Standards**, not a second Policy. NDMO expects entity policy aligned to national standards `[C]` (narrative); that is not a licence to invent many overlapping cluster policies. Specification-level mapping `[NDMO verification required]`.

---

## What is the difference between Policy, Standard and Procedure?

| Layer | Question |
| --- | --- |
| **Policy** | Must we? Who is the authority? |
| **Standard** | What does good look like for this topic? |
| **Procedure** | How do we do this instance, with evidence? |

Templates/records prove the procedure ran. They are not a fourth “law.”

---

## Why is MDM a standalone Standard?

Master data is **cross-process identity and lists**, not the same as “have a catalog.” Catalog (STD-004) is discovery/definition registration. MDM (STD-005) is **who is authoritative for Person, Provider, org reference** and duplicate **governance** — without Phase 10 matching engines. Folding MDM into metadata would hide ownership of identity under a tooling conversation.

---

## Why isn’t Data Quality fully defined yet?

STD-003 / PRC-003 set **accountability and issue path**. Dimensions, thresholds, and rule libraries are **Phase 7**. Writing fake KPIs would invent governance the cluster has not designed. Trusted Data is an NDMO principle **name** `[C]`; that does not complete the Quality domain.

---

## How does an exception work?

Request → justification → DMO review → **DMC approves or denies** → register → monitor → close/renew. **DMC is Accountable.** Owner cannot self-approve out-of-policy access. In-policy shares use PRC-005 instead.

---

## Who approves the Data Governance Policy?

**Data Management Committee**, chaired by the Cluster CEO `[B]`. CDO **owns** (drafts/maintains). CDO does not chair their own oversight.

---

## How do Policies connect to operational evidence?

Policy → Standard → Procedure → **record** (registry, issue, share request, exception register). If there is no record, the procedure did not happen for audit purposes `[B]`. This is still not an NDMO evidence pack (Phase 14 not built).

---

## How do you prevent governance documentation from becoming unmanageable?

**1 + 5 + 6** and stop. No hospital-level policy stacks. No extra standards for tools. Later phases (7–10) **extend** STD-003/004/005; they should not create parallel policy trees. Templates stay an **index**, not ten more “standards.”

---

## Must-nots

| Do not say | Say instead |
| --- | --- |
| “We have four data policies.” | “One Policy, five Standards, six Procedures.” |
| “Rafid Restricted is the NDMO Restricted tier.” | Rafid tiers are `[A][B]`; NDMO names `[NDMO verification required]`. |
| “Sharing is one signature.” | Owner business **A** and PDPO privacy **A** are **separate**. |
| “We are NDMO compliant because we wrote POL-001.” | Documents are design; no specification evidenced. |
