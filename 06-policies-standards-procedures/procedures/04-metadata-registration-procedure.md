# Metadata Registration Procedure

**Document ID:** RHC-DG-PRC-004  
**Version:** 1.0  
**Status:** Implemented (documentation) — **not** a Phase 8 catalog  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With POL-001 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Registration path only; no catalog platform.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Parent standard:** RHC-DG-STD-004  

**Do not** implement Purview, Collibra, Atlan, or another catalog. **Phase 8 is Designed / Documented** (conceptual catalog in `08-metadata-catalog/`). Operational implementation and measured performance are not claimed.

---

## 1. Purpose

Register a dataset’s **business metadata** and keep it linked to classification `[B]`.

## 2. Process

```text
Identify dataset
  → Document business definition
  → Register metadata
  → Link classification
  → Maintain
```

| Step | Who | Action |
| --- | --- | --- |
| Identify dataset | Steward; Custodian **C** | Same unit as PRC-002 |
| Document business definition | Steward **R**; Owner **A** | Owner accepts meaning; PDPO **C** if personal/health identifying |
| Register metadata | Steward **R**; DMO completeness | Metadata Registration Form / catalog record (working register, not a product) |
| Link classification | Steward | Rafid tier from PRC-002 / Classification Registry; if unclassified, complete PRC-002 first — unlabeled is not Public |
| Maintain | Steward | Update on definition, system, or Owner change; conceptual source/system class only (lineage detail = Phase 9) |

## 3. Evidence

Metadata Registration Form; link to Classification Registry; Owner acceptance of definition.

## 4. Escalation

Definition dispute: Owner; cross-domain: DMO/CDO/DMC. DMO cannot rewrite clinical meaning to “complete” the register.
