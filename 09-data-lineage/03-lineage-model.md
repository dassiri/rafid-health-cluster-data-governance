# Lineage Model

**Document ID:** RHC-DG-P9-003  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (model method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With Phase 8 asset model `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Reuses Phase 8 hierarchy; no parallel object model.

**Phase:** 9 — Data lineage  
**Does not decide:** A second catalog model; physical ERD

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **what lineage is drawn on**. It **reuses Phase 8’s hierarchy exactly**. It does **not** create a parallel data-object model.

---

## 2. Object hierarchy (Phase 8 — unchanged)

```text
Data Domain
→ Data Asset
→ Data Structure / Object
→ Data Element
```

Lineage edges connect these objects (usually **assets** in Year-1). They do not invent a fifth object type.

---

## 3. Existing relationships (consumed, not redesigned)

| Relationship | Source |
| --- | --- |
| Data Asset ↔ Data Owner / Business Data Steward | Phase 4 + Phase 8 catalog |
| Data Element ↔ Business Term | Phase 8 glossary |
| Data Element ↔ Classification | Phase 5 applies at **dataset** level; elements inform Owner assessment — lineage does not classify |
| Data Element ↔ Quality Rule | Phase 7 (CDE / rule) |

---

## 4. Lineage concepts (locked)

```text
Source → Transformation → Target → Consumer
```

| Concept | Meaning |
| --- | --- |
| **Source** | Upstream asset or system context |
| **Transformation** | Conceptual change between source and target |
| **Target** | Downstream catalog asset |
| **Consumer** | Use of the target (report, interchange, process) — not access approval |

These map to Phase 8 capability-dependent fields: Upstream source, Downstream consumers, Transformation reference.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Phase 8 hierarchy reuse; four-step flow | Sections 2–4 |
| `[C]` | Catalog domain **name** | Context |
| `[NDMO verification required]` | Official NDMO lineage metamodel | Not claimed |
