# Data Classification Standard

**Document ID:** RHC-DG-STD-002  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer / DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Codifies Phase 5 without redesign.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent policy:** RHC-DG-POL-001  
**Procedure:** RHC-DG-PRC-002  

Data Classification is an NDMO knowledge-domain **name** `[C]`. Official NDMO **tier names and definitions** remain unresolved `[NDMO verification required]`. Candidate national name-sets (Top Secret / Secret / Restricted / Public **versus** Top Secret / Secret / Confidential / Public) are **not selected**. This Standard does **not** equate Rafid tiers with NDMO national tiers. No control IDs. No compliance claim.

---

## 1. Purpose

Require dataset-level classification using **Rafid’s proposed four-tier scheme** `[A][B]`.

---

## 2. Rafid tiers `[A][B]` — not NDMO national tiers

In increasing handling strictness:

1. **Public**  
2. **Internal**  
3. **Confidential**  
4. **Restricted**  

Working meanings are in Phase 5 (`02-classification-model.md`). They are Rafid definitions, not official NDMO definitions `[NDMO verification required]`.

---

## 3. Mandatory rules

1. Classify at **dataset** level, not automatically at domain level.
2. Use qualitative **highest applicable impact** (privacy, patient safety, financial, legal/regulatory, security, reputational, operational; unauthorized disclosure, modification, access). **No numeric scoring.**
3. Data Owner is **Accountable** and **approves** initial classification and **reclassification**. Only the Data Owner approves a classification **change**.
4. Steward proposes, records, flags misclassification.
5. Custodian implements technical handling; **does not decide** the tier.
6. DMO owns methodology and the Classification Registry.
7. PDPO reviews privacy implications for personal data.
8. Compliance Officer audits the process independently.
9. Domain “typical” tiers in Phase 5 are **guidance**, not blanket rules.
10. Combination/linkage uses the highest input impact unless the Owner approves a documented exception (for example de-identification).
11. Unlabeled existing data is not Public.
12. Archive does not drop classification.

---

## 4. Typical domain guidance (not blanket) `[A]`

| Domain | Typical Rafid tier | Owner |
| --- | --- | --- |
| Patient / Person Master Data | Restricted | Patient Access & Experience Director |
| Clinical / Medical Records Data | Restricted | CMO |
| Provider / Clinician Data | Confidential | Medical Affairs Officer |
| Financial / Billing & Claims Data | Confidential–Restricted | CFO |
| HR / Workforce Data | Confidential | HR Director |
| Supply Chain & Asset Data | Internal | Supply Chain Director |
| Quality & Patient Safety Data | Restricted | CQPSO |
| Reference / Organizational Master Data | Internal (potentially Public if deliberately published) | Strategy & Planning Director |

---

## 5. Restricted external sharing

**Requires Data Owner business approval + PDPO privacy compliance review where personal data is involved**

Security handling stays high-level; NCA remains mandate for NDMO Data Security and Protection `[C]`. No algorithms or tools.

---

## 6. Evidence

Classification Registry entries (Phase 5 schema); Owner approval date; rationale without scores. Procedure: PRC-002.
