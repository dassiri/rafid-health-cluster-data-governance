# Classification Change Management

**Document ID:** RHC-DG-P5-007  
**Phase:** 5 — Data classification  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records when a Rafid dataset **must be reconsidered** and who may change the tier `[A][B]`.

**Only the Data Owner approves the classification change.**  
Stewards propose. DMO records. Custodians implement. PDPO reviews privacy implications for personal data. Compliance Officer may audit the process. **IT does not approve the new tier.**

---

## 2. Change triggers `[B]`

Reconsider classification when any of the following occurs:

| Trigger | Example (fictional, not exhaustive) `[A]` |
| --- | --- |
| Change in sensitivity | Identifiers added to a previously aggregate file |
| New regulation | New applicable personal-data or health-sector rule — legal mapping `[NDMO verification required]` |
| New use case | Registry reused for research or public reporting |
| New data combination / linkage | Billing extract joined to clinical notes |
| Security incident | Unauthorized access suggests impact was understated |
| Organizational change | Domain Owner title changes (Phase 4 lifecycle); new Owner still must confirm or re-approve the tier |
| Dataset transformation | Migration, derivation, or archive packaging that changes content or identifiability |
| Change in sharing context | Internal-only file proposed for external partner use |

A trigger **opens a review**. It does not automatically raise or lower the tier.

---

## 3. Change path

```text
Trigger or Steward flag
    → Steward impact narrative (qualitative)
    → PDPO C if personal data
    → Data Owner approval of new Rafid tier (or confirmation of existing)
    → Steward updates Classification Registry
    → DMO oversight
    → Custodian adjusts technical handling
```

If the Owner is vacant, Phase 4 Owner-departure rules apply: the **title** remains A; DMO does not become classifier.

Access **exceptions** remain DMC **A** (Phase 4). That is not a classification-tier change.

---

## 4. Direction of change

- **Upward** (more strict): default when linkage or identifiability increases, using highest applicable impact.
- **Downward** (less strict): only with explicit Owner approval and documented rationale (for example evidenced de-identification, or deliberate Public release). Downward is never implied by “we aggregated it.”

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 5 triggers and Owner-only approval | All sections |
| `[A]` | Rafid examples | Table |
| `[C]` | PDPO **name** | Privacy consult |
| `[NDMO verification required]` | Regulatory trigger detail | Not specified as articles |
