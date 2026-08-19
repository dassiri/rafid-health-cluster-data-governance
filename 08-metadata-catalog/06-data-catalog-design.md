# Data Catalog Design (Conceptual)

**Document ID:** RHC-DG-P8-006  
**Version:** 1.0  
**Status:** Implemented (conceptual design only)  
**Owner:** CDO / DMO — catalog **programme** `[B]`; Data Owner **A** for domain catalog **content** (Phase 4 row 8)  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual catalog; no platform.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** Vendor, UI wireframes, search engine, or access-control product

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

The Data Catalog is the **governed inventory of described data assets** so people can find **what exists, who owns it, how it is classified, and whether it is trusted as a description** `[B]`.

It is **not** the data store. It is **not** a sharing approval. It is **not** NDMO certification. It is **not** a tool implementation.

NDMO names Data Catalog and Metadata as a knowledge domain and describes an automated catalog as a national **concept** in Standards narrative `[C]` (Phase 0–2). Rafid does **not** have that tool in this drop `[A]`. Specification-level catalog requirements remain `[NDMO verification required]`.

---

## 2. Users (approved personas) `[A][B]`

| Persona | Catalog use |
| --- | --- |
| **Executive** | See that priority assets exist, have Owners, and have status — not a data extract |
| **Data Owner** | Approve meaning, classification link, and certification of domain assets |
| **Business Data Steward** | Create and maintain records; validate before publish |
| **Analyst** | Discover assets and definitions; request access via Phase 4/5/6 sharing-access path — not via catalog download of Restricted data |
| **Data Scientist** | Same discovery rules; no special bypass of classification |
| **IT / Custodian** | Supply technical metadata minimum; do not decide business meaning |
| **Governance Office / DMO** | Methodology, completeness check, certification register, exception routing |

---

## 3. Conceptual catalog capabilities (not a UI)

| Capability | What the design requires |
| --- | --- |
| **Search / discovery** | [`10-search-discovery.md`](10-search-discovery.md) |
| **Asset pages** | One page-equivalent per asset: mandatory metadata, glossary links, certification, coarse lineage **if** present |
| **Ownership** | Data Owner and Business Data Steward visible |
| **Classification** | Rafid tier visible as **metadata**; underlying Confidential/Restricted **data** is not shown |
| **Quality indicators** | Capability-dependent; Phase 7 status/CDE links when they exist — not a second scorecard product |
| **Glossary links** | Terms from [`05-business-glossary.md`](05-business-glossary.md) |
| **Lineage links** | Conceptual pointers only ([`11-lineage-conceptual.md`](11-lineage-conceptual.md)) |
| **Usage context** | Intended use (recommended field) |
| **Certification / status** | [`09-certification-trust-model.md`](09-certification-trust-model.md) |

No wireframes. No technical search architecture.

---

## 4. What publishing means

**Publish** = governed **metadata** is discoverable to catalog personas according to catalog rules.

Publish is **not**:

- Open-by-Default release of clinical data
- Access approval (Owner **A** in-policy; DMC **A** for Policy exceptions — Phase 4)
- Privacy determination (PDPO **A** on the sharing privacy row)

---

## 5. Programme vs content (unchanged RACI)

| Decision | A (already approved) |
| --- | --- |
| Catalog **programme / methodology** | CDO / DMO (Phase 3 enterprise pattern; STD-004) |
| Domain catalog **content / definitions** | Data Owner (Phase 4 row 8) |
| Classification **value** | Data Owner (Phase 4 row 3; Phase 5) |

No new DMC decision class. DMC remains **A** for existing classes (L3 policy, material exceptions, residual sharing risk, Owner non-participation, access **exception**).

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Personas and conceptual capabilities | Sections 2–3 |
| `[C]` | Data Catalog and Metadata domain **name**; automated catalog as national **concept** in Standards narrative | Purpose |
| `[NDMO verification required]` | Control-level catalog product mandates | Not claimed |
