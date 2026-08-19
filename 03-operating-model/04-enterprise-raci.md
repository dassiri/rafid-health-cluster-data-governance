# Enterprise RACI

**Document ID:** RHC-DG-P3-004  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Domain-level RACI (Phase 4) or procedure-level RACI (Phase 6)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This is the **high-level enterprise** Data Governance RACI for the fictional Rafid Health Cluster `[A]`. It uses **role titles**, not people.

It is an industry RACI design `[B]`. It is not an NDMO specification and is not a compliance claim.

---

## 2. Legend

| Letter | Meaning |
| --- | --- |
| **R** | **Responsible** — does the work |
| **A** | **Accountable** — one owner of the outcome; answers if it fails |
| **C** | **Consulted** — two-way input before the decision |
| **I** | **Informed** — told after the decision |

**Rules applied `[B]`**

- Exactly **one A per row**.
- Data Owners remain accountable for the business meaning and quality of their data domains.
- Business Data Stewards primarily execute and coordinate operational governance.
- IT / Data Custodians are responsible for technical implementation, not business ownership.
- IT is not Accountable for business data ownership by default.

---

## 3. Role abbreviations

| Code | Role |
| --- | --- |
| ESC | Executive Sponsor (Cluster CEO) |
| DMC | Data Management Committee |
| CDO | Chief Data Officer |
| DGO | Data Governance Officer / DMO staff |
| DO | Data Owner (Business Data Executive) `[C]` name |
| BDS | Business Data Steward `[C]` name |
| CUST | Data Custodian (IT Data Steward) `[C]` name |
| PDPO | Personal Data Protection Officer `[C]` name |
| CO | Compliance Officer (data) `[C]` name |
| LEG | Legal Advisor `[C]` name |
| ODIA | Open Data and Information Access Officer `[C]` name |
| CON | Data Consumer `[B]` |

---

## 4. Enterprise RACI matrix `[B]`

| Activity | ESC | DMC | CDO | DGO | DO | BDS | CUST | PDPO | CO | LEG | ODIA | CON |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Governance strategy | C | **A** | **R** | R | C | I | I | C | C | C | C | I |
| Policy approval (L3) | C | **A** | **R** | R | C | I | C | C | C | C | C | I |
| Data domain ownership (exercise of ownership) | I | I | C | C | **A** | **R** | C | C | I | I | I | I |
| Data definition approval | I | I | I | C | **A** | **R** | C | C* | I | I | I | I |
| Data classification (dataset application) | I | I | C | C | **A** | **R** | C | C | I | C | C† | I |
| Data quality rules | I | I | I | C | **A** | **R** | C | I | I | I | I | I |
| Data quality issue resolution | I | I | I‡ | C | **A** | **R** | R | I | I | I | I | C |
| Metadata standards (enterprise) | I | C | **A** | **R** | C | C | C | I | I | I | I | I |
| Data catalog ownership (programme + content rules) | I | I | **A** | **R** | C | R | R§ | I | I | I | I | I |
| Data lineage (technical capture + domain completeness) | I | I | **A** | C | C | C | **R** | I | I | I | I | I |
| Data access decisions (within policy) | I | I | I | I | **A** | R | **R** | C | I | I | I | C |
| Data sharing decisions (routine / in-policy) | I | I | C | C | **A** | R | C | C | I | C | C | I |
| Data sharing (external / high-risk / novel) | C | **A** | R | R | R | C | C | C | C | C | C | I |
| Data retention / lifecycle (domain application) | I | I | I | C | **A** | R | R | C | I | C | I | I |
| Regulatory escalation (material) | **A** | I | **R** | R | C | I | I | R | R | R | C | I |
| Regulatory escalation (non-material) | I | I | **A** | R | C | I | I | R | R | R | C | I |
| Governance exceptions (to L3 policy) | C | **A** | R | R | C | I | C | C | C | C | C | I |
| KPI reporting | I | I | **A** | **R** | C | R | C | I | C | I | I | I |
| Governance maturity / alignment self-assessment | I | I | **A** | R | C | I | I | C | **R** | C | C | I |

**One A per row** is in the **A** column only. Multiple **R** cells on a row are allowed.

### Notes

\* PDPO consulted when the definition is personal/health identifying.  
† ODIA consulted when the likely outcome is Public / open data.  
‡ CDO becomes **R** (Data Owner remains **A**) only after SLA-breach escalation — not a second A.  
§ Custodian **R** for the **tool**; CDO remains **A** for the catalog **programme**.

**Classification method / standard** (how Rafid classifies) is a policy/standard item: **A = DMC**, **R = CDO**. It is not a second Accountable on the “dataset application” row. Dataset application stays **A = Data Owner**.

**Sharing:** NDMO’s sharing process includes a Business Data Executive approval step `[C]`. Routine sharing is therefore **A = Data Owner**, not IT. Regulation-level sharing procedure text is `[NDMO verification required]`.

**Material vs non-material regulatory escalation:** materiality routing is in [`05-decision-escalation-model.md`](05-decision-escalation-model.md). Split into two rows so each row has exactly one A. CDO remains **R** on material cases, consistent with NDMO describing the CDO as leading the compliance exercise `[C]` — not a claim that the exercise has been run.

---

## 5. What this RACI is not

- Not a Phase 4 domain assignment
- Not a list of named Data Owners
- Not policy text
- Not evidence of NDMO implementation

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 Implementation Brief | Matrix, legend, one-A rule |
| `[C]` | NDMO Standards v1.5 — BDE involvement in sharing (as stated in the Standards); CDO-led assessment description; role **names** | Why Owner is A for routine sharing; CDO leads assessment work |
| `[NDMO verification required]` | Sharing regulation procedure detail | Not retrieved |
