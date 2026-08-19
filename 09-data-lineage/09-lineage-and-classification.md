# Lineage and Classification

**Document ID:** RHC-DG-P9-009  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for classification (Phase 5); DMO (this integration note) `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 5 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — No automatic highest-tier inheritance; Phase 5 remains sole method.

**Phase:** 9 — Data lineage  
**Does not decide:** Any new classification tier, scoring, or inheritance rule

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose (critical)

This document records how lineage **interacts with classification**.

**Phase 5 remains the sole source of classification authority and method.**  
**Lineage does not automatically classify or reclassify data.**  
**Lineage does not introduce any new classification rule.**

Rafid tiers remain Public / Internal / Confidential / Restricted `[A][B]`. They are **not** NDMO national tiers `[NDMO verification required]`.

---

## 2. What this phase does **not** say

Do **not** state that downstream data automatically inherits the highest classification tier as a Phase 9 rule.

Highest-applicable-impact remains a **Phase 5 qualitative rule applied by the Data Owner to a dataset**. Lineage may **inform** that assessment. It does not execute it.

---

## 3. Governance question (locked)

> Does the downstream asset still contain the same sensitive elements as the source? If so, the Data Owner should assess the downstream classification using the Phase 5 classification framework.

That is a **reassessment prompt**, not an automatic result.

---

## 4. Transformation can change sensitivity `[B]`

The Data Owner remains **accountable** for the **downstream** classification decision.

| Change | Why reassessment may be needed |
| --- | --- |
| Transformation | Derived values may be less (or more) identifying |
| Tokenization | Identifiers may no longer be directly sensitive **if** the Owner accepts the tokenized dataset with PDPO consult where personal data applies |
| Removal of fields | Identifiers or clinical content may be gone |
| Aggregation | Individual-level impact may drop — **not** automatically Public |
| De-identification | Phase 5 already used a de-identified clinical example as possibly Confidential rather than Restricted — still **Owner A**, not lineage A |

Lineage **only surfaces the need for reassessment**. Custodian implements technical controls; Custodian does **not** decide the Rafid tier.

---

## 5. Sharing remains two decisions

If lineage shows an external consumer, sharing still uses:

1. Data Owner **A** — business approval  
2. PDPO **A** — privacy compliance review where personal data applies  

Lineage does not merge these rows.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Reassessment prompt; no inheritance rule | Sections 2–4 |
| `[C]` | Data Classification domain **name**; PDPO **name** | Context |
| `[NDMO verification required]` | National tier names; official “derived dataset” classification law | Not claimed |
