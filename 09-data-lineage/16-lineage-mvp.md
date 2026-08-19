# Lineage MVP

**Document ID:** RHC-DG-P9-016  
**Version:** 1.0  
**Status:** Implemented (MVP design only — not a live lineage graph)  
**Owner:** CDO / DMO (programme) `[B]`; domain Owners **A** for MVP content  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Three-domain MVP; Critical Lineage Register focus; no enterprise-wide lineage.

**Phase:** 9 — Data lineage  
**Does not decide:** Tool purchase; numeric coverage targets; remaining five domains in Year-1 operating cut

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the **approved lineage MVP** `[A][B]`.

Do **not** attempt enterprise-wide lineage. Success is **qualitative**. Do not invent numeric targets.

---

## 2. Initial domains (locked)

1. Patient / Person Master  
2. Clinical / Medical Records  
3. Financial / Billing & Claims  

These are the same three Phase 8 catalog MVP domains. Other domains remain in the framework but **outside** Year-1 lineage operating scope.

**Owners (Phase 4):** Patient Access & Experience Director; CMO; CFO. Steward: **Business Data Steward**.

---

## 3. Initial use cases (locked)

1. Patient Registration → Clinical → Billing/Claims lineage (the single E2E example, including generic external interchange as consumer)  
2. Patient Claim Rejection Rate business lineage  

---

## 4. Initial assets (locked)

- Patient Master Record  
- Encounter / Diagnosis record  
- Claims Extract  

Required metadata: **Phase 8 Lineage Metadata fields** (Upstream source, Downstream consumers, Transformation reference), plus catalog mandatory fields already required to publish an asset.

---

## 5. Governance workflow (locked)

Use the Phase 9 registration workflow ([`12-registration-workflow.md`](12-registration-workflow.md)). No new Phase 6 procedure.

**Focus the Year-1 MVP on the Critical Lineage Register** — confirmed prioritized coverage for the two use cases, not every cluster interface.

---

## 6. Qualitative success `[A][B]`

- The two use cases can be described at Levels 1–2  
- Lineage Metadata fields are populated or explicitly gapped  
- Owners of the three domains can validate business meaning  
- Classification reassessment questions can be asked without auto-tiering  
- No lineage product is required to declare the MVP **design** complete  

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved MVP cut | Sections 2–6 |
| `[C]` | Catalog domain **name** | Context |
| `[NDMO verification required]` | Official NDMO lineage rollout metrics | Not claimed |
