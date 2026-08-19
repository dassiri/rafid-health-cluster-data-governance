# Metadata Governance Artifacts

**Document ID:** RHC-DG-P8-015  
**Version:** 1.0  
**Status:** Implemented (proposed artifacts only)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual index; exceptions reuse Phase 6 procedure.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Physical schemas; NDMO-mandated registers `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document is a **conceptual design/index** of proposed Rafid metadata artifacts `[A][B]`.

They are **not** claimed as NDMO-mandated. **No compliance is claimed. No NDMO control IDs are invented.**

---

## 2. Proposed artifacts (locked list)

| Artifact `[A][B]` | Purpose | Notes |
| --- | --- | --- |
| **Metadata Registry** | Working store of metadata records (fields in the minimum standard) | May be the same store as the catalog; name describes the **content** |
| **Data Asset Registry** | List of registered assets (IDs, types, domain, status) | Year-1 types only |
| **Business Glossary** | Terms and definitions | [`05-business-glossary.md`](05-business-glossary.md) |
| **Metadata Quality Report** | Qualitative view of mandatory-field gaps and stale reviews | No numeric KPI pack |
| **Catalog Certification Register** | Status history (Registered → … → Retired) | Internal trust only |
| **Metadata Change Record** | Material changes to definition, Owner, classification link, or status | Evidence of Maintain |
| **Metadata Exception Record** | Out-of-policy metadata/catalog handling | **Reuses Phase 6 exception mechanism — no new procedure** |

---

## 3. Metadata Exception Record — reuse Phase 6

Do **not** create a new exception procedure.

Out-of-policy requests use:

**Data Governance Exception Procedure**

`06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md`

**DMC remains Accountable** for those Policy exceptions (existing decision right). The Metadata Exception Record is a **pointer / extract** for catalog-related exceptions in the Policy Exception Register — not a second law.

In-policy residual (for example “lineage not yet described”) stays on the asset record as a known gap, not an exception.

---

## 4. Relationship to Phase 6 templates

Phase 6 already indexes a Metadata Registration Form as a supporting artifact. This phase **names** the catalog set. It does not replace STD-004.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Seven proposed artifacts | Section 2 |
| `[C]` | Data Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Whether NDMO mandates these named artifacts | Not claimed |
