# Lineage Types

**Document ID:** RHC-DG-P9-002  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (type method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Four types; Year-1 priorities locked.

**Phase:** 9 — Data lineage  
**Does not decide:** Enterprise technical lineage; tool parsers

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records the **four lineage types** and Year-1 priorities `[A][B]`.

These types are Rafid design. They are **not** claimed as NDMO-required type names `[NDMO verification required]`.

---

## 2. Four types (locked)

| # | Type | Working meaning `[A][B]` |
| --- | --- | --- |
| 1 | **Business Lineage** | From a business question or KPI to the data that supports it (terms, elements, assets, systems, consumer). |
| 2 | **Conceptual Lineage** | Source → Transformation → Target → Consumer at asset/system-class level, without job code. |
| 3 | **Technical Lineage** | System-object and (selectively) field movement as **described**, not as scanned. |
| 4 | **End-to-End Lineage** | A chain across domains from originating capture to an external or executive consumer. |

---

## 3. Year-1 priorities (locked)

| Type | Year-1 |
| --- | --- |
| Business Lineage | **Priority** |
| Conceptual Lineage | **Priority** |
| Technical Lineage | **Conceptual only** |
| End-to-End Lineage | **One worked example only** |

Do **not** build enterprise-wide technical lineage. Technical lineage in Year-1 is a **description pattern**, not a scanner or graph.

The single end-to-end worked example is [`06-worked-example.md`](06-worked-example.md). It is illustrative `[A]`, not a production map of the cluster.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved type set and Year-1 cut | Sections 2–3 |
| `[C]` | Catalog domain **name** (lineage as metadata conceptually) | Context |
| `[NDMO verification required]` | Official NDMO lineage-type taxonomy | Not claimed |
