# Lineage and Data Quality

**Document ID:** RHC-DG-P9-008  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (integration method); Data Owner **A** for quality outcomes (Phase 7)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 7 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Impact chain only; no second DQ framework.

**Phase:** 9 — Data lineage  
**Does not decide:** New dimensions, thresholds, CDEs, or scorecards

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records how lineage **supports impact analysis** for data quality `[B]`.

It **reuses Phase 7 terminology**. It does **not** create a second Data Quality Framework.

Trusted Data is an NDMO principle **name** `[C]`. That does not make this file an NDMO quality specification `[NDMO verification required]`.

---

## 2. Approved conceptual chain (locked)

```text
Quality failure in a source field
→ downstream dataset
→ downstream process/report
→ KPI
```

| Link | Meaning |
| --- | --- |
| **Source field** | Often a CDE (for example invalid diagnosis code — DQ-002 / CDE-003) |
| **Downstream dataset** | Claims Extract still carries or depends on that field |
| **Downstream process/report** | Claim composition or rejection listing |
| **KPI** | Illustrative Patient Claim Rejection Rate `[A]` |

Issues still follow the Phase 6 **Data Quality Issue Management Procedure** (title/path as in Phase 7). Lineage does not replace Log → Triage → Assign → Resolve → Verify → Close.

---

## 3. Impact analysis `[B]`

When a quality defect is logged:

1. Identify the **source field** and owning domain (Phase 4).  
2. Use **conceptual lineage** to list **downstream assets and consumers** (Phase 8 fields).  
3. Notify downstream Stewards; each Owner remains **A** for their domain quality.  
4. Prefer **source correction** (Phase 7 remediation) so the chain stops generating the defect.

Lineage does not assign a new severity model. Phase 7 Critical / High / Medium / Low `[A][B]` remains.

---

## 4. Illustrative walk `[A]`

Invalid diagnosis code at encounter → claims extract with mismatched coding → interchange rejection → Claim Rejection Rate movement (illustrative, not measured).

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative chain | Section 4 |
| `[B]` | Impact analysis via lineage | Sections 2–3 |
| `[C]` | Trusted Data principle **name**; Data Quality domain **name** | Context |
| `[NDMO verification required]` | Official NDMO lineage-quality specifications | Not claimed |
