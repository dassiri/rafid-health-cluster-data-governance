# Data Access / Sharing Governance Procedure

**Document ID:** RHC-DG-PRC-005  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Two separate accountability decisions preserved.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent policy:** RHC-DG-POL-001  

NDMO describes a sharing process that includes Business Data Executive approval `[C]`. Regulation-level steps `[NDMO verification required]`. **No control IDs. No compliance claim.**

---

## 1. Purpose

Govern **in-policy access** and **data sharing** without merging business and privacy accountability `[B]`.

## 2. Two distinct decisions (mandatory)

| # | Decision | Accountable |
| --- | --- | --- |
| 1 | **Business approval** | **Data Owner = A** |
| 2 | **Privacy compliance review for personal data** | **PDPO = A** |

**Do not combine these into one approval.**  
A share of personal data is **not** complete until **both** decisions are recorded.  
If the dataset is **not** personal data, decision 2 is **not applicable** (record N/A); decision 1 still runs. PDPO is **I** on business approval when personal data is clearly absent (Phase 4).

## 3. Process

```text
Request
  → Data Owner business approval
  → PDPO privacy review where personal data applies
  → Technical implementation
  → Logging / evidence
```

| Step | Who | Action |
| --- | --- | --- |
| **Request** | Consumer / requestor | Data Sharing Request (or access request); dataset; purpose; internal vs external |
| **Data Owner business approval** | Data Owner **A**; Steward **R** | In-policy: approve/deny business use. **Out-of-policy access** → PRC-006 (DMC **A**), not Owner self-exception |
| **PDPO privacy review where personal data applies** | PDPO **A** | Separate decision; may approve, deny, or require conditions. Does **not** replace Owner **A** on business approval |
| **Technical implementation** | Custodian **R** | Provision or refuse on security grounds (CISO+CDO); not a third business **A** |
| **Logging / evidence** | Steward / DMO | Request record; both decisions; Rafid classification of the dataset |

## 4. Restricted external sharing

Use this wording **exactly**:

**Requires Data Owner business approval + PDPO privacy compliance review where personal data is involved**

## 5. Classification

Sharing does not reclassify. If the dataset is unclassified, complete PRC-002 first.

## 6. Evidence

Data Sharing Request; Owner business decision; PDPO decision or N/A; provision log.
