# Business Lineage Example — Patient Claim Rejection Rate

**Document ID:** RHC-DG-P9-007  
**Version:** 1.0  
**Status:** Implemented (illustrative only)  
**Owner:** CFO **A** for the financial meaning of the KPI in a live process; this file is a teaching example  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Locked KPI example; not a real organizational metric.

**Phase:** 9 — Data lineage  
**Does not decide:** Live KPI definition, numeric targets, or BI tool

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose and disclaimer

This file records **exactly one** business-lineage example `[A]`:

**Patient Claim Rejection Rate**

The name and trace are **illustrative**. They are **not** a real Rafid, MOH, or payer metric, and they are **not** a Phase 12 KPI pack.

---

## 2. Trace (locked)

```text
Business KPI
→ Business Definition
→ Data Elements
→ Data Assets
→ Source Systems
→ Transformation
→ Consumer
```

| Step | Illustrative content `[A]` |
| --- | --- |
| **Business KPI** | Patient Claim Rejection Rate — proportion of submitted claims returned or rejected in a reporting period (definition not a measured rate) |
| **Business Definition** | Owner-accepted meaning of “claim,” “rejection,” and the in-scope population (Financial domain **A** = CFO) |
| **Data Elements** | Claim identifier (CDE-007); billed service / charge code (CDE-008); diagnosis code as billing input (CDE-003 consumed); Patient identifier on the claim (CDE-002 consumed) |
| **Data Assets** | Claims Extract; Encounter / Diagnosis record; Patient Master Record (catalog assets) |
| **Source Systems** | Billing / claims (primary context); EMR clinical (contributing); EMR / registration (identity context) — Phase 8 System / Primary System rule: not exactly one source |
| **Transformation** | Conceptual: encounter coding → charge capture → claim composition → rejection flag from interchange response (**not** ETL code) |
| **Consumer** | Revenue-cycle Domain Huddle / DMC **summary** theme — not a published open-data statistic |

No numeric target is given (would be `[A] Illustrative` if one were ever shown; none is shown here).

---

## 3. Links to prior phases (consumed, not redesigned)

| Phase | Connection |
| --- | --- |
| **Phase 8 Business Glossary** | Terms **Claim**, **Diagnosis**, **Encounter**, **Patient** `[A]` in `08-metadata-catalog/05-business-glossary.md` |
| **Phase 8 Data Catalog** | Assets registered with mandatory metadata; lineage fields: upstream / downstream / transformation reference |
| **Phase 7 Data Quality** | Invalid diagnosis (DQ-002), duplicate claim ID (DQ-005), incomplete charge (DQ-006) can **feed** rejections — impact analysis in [`08-lineage-and-quality.md`](08-lineage-and-quality.md) |
| **Phase 4 Ownership** | KPI/claim extract **A** = CFO; clinical diagnosis meaning **A** = CMO; person identity **A** = Patient Access & Experience Director. Steward label: **Business Data Steward**. No second Owner. |

Sharing the rejection report still uses two decisions if personal data is in the output: Owner business **A**; PDPO privacy **A**. Lineage does not merge them.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative KPI and trace | Sections 1–2 |
| `[B]` | Business lineage as KPI-to-source | Method |
| `[C]` | Role **names** | Context |
| `[NDMO verification required]` | Any national claims-rejection reporting rule | Not claimed |
