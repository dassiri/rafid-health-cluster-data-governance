# Lineage (Conceptual Metadata Only)

**Document ID:** RHC-DG-P8-011  
**Version:** 1.0  
**Status:** Implemented (conceptual only)  
**Owner:** DMO `[B]` (conceptual method); Data Owner **A** for accepting lineage **description** of domain assets  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Coarse lineage as metadata. Phase 9 is Designed / Documented.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Technical lineage architecture; automated capture; column-level lineage

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **coarse lineage as metadata** `[A][B]`.

**Detailed lineage remains Phase 9.** Phase 9 is Designed / Documented; operational implementation and measured performance are not claimed.

STD-004 already required a conceptual system/source class. This file does not upgrade that into a lineage platform.

---

## 2. Conceptual pattern (locked)

```text
Source → Transformation → Target → Consumer
```

| Element | Catalog use |
| --- | --- |
| **Source** | Upstream system class or contributing systems (see System / Primary System rule) |
| **Transformation** | Named conceptual step (extract, aggregate, code map) — **not** a mapping engine |
| **Target** | The catalog asset |
| **Consumer** | Known downstream use (report, claim extract) as metadata, not an access grant |

These may populate capability-dependent fields: Upstream source, Downstream consumers, Transformation reference.

---

## 3. Explicitly not built

- Technical lineage architecture
- Automated lineage capture
- Column-level lineage
- Integration-graph products

Illustrative sentence `[A]`: “Registration (source) → ADT feed (transformation) → Patient demographic dataset (target) → Billing extract (consumer).” This is fiction for teaching, not a measured flow.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Coarse four-step pattern | Section 2 |
| `[C]` | Catalog domain **name** | Context |
| `[NDMO verification required]` | Official NDMO lineage-in-catalog specifications | Not claimed |
