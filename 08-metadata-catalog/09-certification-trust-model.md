# Certification and Trust Model

**Document ID:** RHC-DG-P8-009  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for Certified; DMO for register method `[B]`  
**Approver:** CDO `[B]` (model as framework artifact)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-004 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Five internal statuses; explicitly not regulatory/NDMO certification.

**Phase:** 8 — Metadata and catalog  
**Does not decide:** External seals; NDMO assessment scores; tool workflows

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Nature of certification (locked)

Catalog certification is:

**`[A][B]` Proposed Rafid internal trust mechanism.**

It is **not**:

- Regulatory certification
- NDMO certification
- External compliance approval
- Evidence that a specification is implemented

Do not brief “Certified” as a national or regulator seal.

---

## 2. Five statuses (locked)

| # | Status | Meaning |
| --- | --- | --- |
| 1 | **Registered** | Mandatory metadata submitted; asset is in the catalog |
| 2 | **Reviewed** | Steward has validated the record |
| 3 | **Certified** | Data Owner accepts the description as trustworthy for discovery/use **as metadata** |
| 4 | **Deprecated** | Should not be used for new work; still visible as a warning |
| 5 | **Retired** | No longer an operational catalog asset; record retained |

Status is mandatory metadata ([`04-minimum-metadata-standard.md`](04-minimum-metadata-standard.md)).

---

## 3. Responsibility (locked) `[A][B]`

| Status | Accountable / responsible actor |
| --- | --- |
| **Registered** | Business Data Steward |
| **Reviewed** | Business Data Steward |
| **Certified** | **Data Owner** |
| **Deprecated** | Data Owner **or** DMO |
| **Retired** | Data Owner with **DMO record-keeping** |

IT / Custodian does not certify business meaning.

Certified does **not** replace access approval or PDPO privacy review.

---

## 4. Relationship to DMC

Moving among these five statuses is **not** a new DMC decision class.

DMC is involved only through **already approved** authority (for example a Policy exception that would allow publishing without Owner-accepted definition). That uses the existing exception path (**DMC = A**), not a “catalog certification committee.”

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Five statuses and actors | Sections 1–3 |
| `[C]` | Data Catalog and Metadata domain **name** | Context |
| `[NDMO verification required]` | Whether NDMO specifies catalog certification states | Not claimed |
