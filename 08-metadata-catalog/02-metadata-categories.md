# Metadata Categories

**Document ID:** RHC-DG-P8-002  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (category method)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Seven categories; mandatory vs capability-dependent split locked.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** NDMO official category names; physical schema

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the **seven Rafid metadata categories** `[A][B]`.

These names are **Rafid design choices**. They are **not** claimed as NDMO-required category names. Specific NDMO metadata categories remain `[NDMO verification required]`. **No compliance is claimed. No NDMO control IDs are used.**

---

## 2. The seven categories (locked)

| # | Category | Working content `[A][B]` |
| --- | --- | --- |
| 1 | **Business Metadata** | Name, description, business definition, glossary links, intended use |
| 2 | **Governance Metadata** | Domain, Data Owner, Business Data Steward, status, approval, change history |
| 3 | **Security / Classification Metadata** | Rafid classification tier (Public / Internal / Confidential / Restricted `[A][B]`); personal-data indicator for discovery — **not** the underlying data; **not** NCA control design |
| 4 | **Technical Metadata** | System / primary system context; asset type; structure/object names at a governance minimum |
| 5 | **Quality Metadata** | Quality status, relevant CDEs, known issues (when quality capability exists) |
| 6 | **Operational Metadata** | Refresh/usage context at a governance level (not a monitoring platform) |
| 7 | **Lineage Metadata** | Coarse upstream / downstream / transformation **references** (not Phase 9 architecture) |

Rafid classification labels are **not** NDMO national tiers `[NDMO verification required]`.

---

## 3. Mandatory vs capability-dependent (locked) `[A][B]`

| Group | Categories | Application |
| --- | --- | --- |
| **Mandatory** | Business; Governance; Security / Classification; Technical (**minimum**) | Required for a published catalog asset in operational use |
| **Capability-dependent** | Quality; Operational; Lineage | Recorded when the capability exists; absence is a known gap, not a fake complete record |

**Do not** treat all seven as equally populated on day one. That would make the minimum model unimplementable `[B]`.

**Do not** drop a mandatory category from a published operational asset. If Technical Metadata is only a system class, that **is** the Year-1 minimum.

---

## 4. Relationship to the minimum field list

Field-level Mandatory / Recommended / Capability-dependent rules are in [`04-minimum-metadata-standard.md`](04-minimum-metadata-standard.md). Categories group those fields; they do not add a second schema.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved seven categories and split | Sections 2–3 |
| `[C]` | Data Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Official NDMO metadata category names and mandates | Not resolved |
