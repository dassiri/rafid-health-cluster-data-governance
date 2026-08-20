# Lineage Governance (Working Pack)

**Document ID:** RHC-DG-P9-WP-001  
**Version:** 1.0  
**Status:** Implemented (working design only — not a live lineage graph)  
**Owner:** DMO `[B]` (method); domain **Data Owner** remains **A** for business lineage correctness  
**Approver:** CDO `[B]`  
**Parent design:** Phase 9 — [`../../01-framework-overview.md`](../../01-framework-overview.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

This working pack is the **applied Data Catalog & Lineage layer** of Phase 9. It shows how Rafid would register, prioritize, validate, and maintain lineage for synthetic healthcare assets already described in the Phase 8 catalog working pack.

It does **not** replace Phase 9. It does **not** create a second lineage framework. Locked design remains in:

| Topic | Locked file |
| --- | --- |
| Lifecycle and purpose | [`../../01-framework-overview.md`](../../01-framework-overview.md) |
| Lineage types | [`../../02-lineage-types.md`](../../02-lineage-types.md) |
| Object model | [`../../03-lineage-model.md`](../../03-lineage-model.md) |
| Granularity | [`../../04-granularity-model.md`](../../04-granularity-model.md) |
| Criticality (nine criteria; two-step) | [`../../05-lineage-criticality.md`](../../05-lineage-criticality.md) |
| Catalog integration | [`../../10-lineage-and-catalog.md`](../../10-lineage-and-catalog.md) |
| Ownership | [`../../11-lineage-ownership.md`](../../11-lineage-ownership.md) |
| Registration workflow | [`../../12-registration-workflow.md`](../../12-registration-workflow.md) |
| Lineage quality | [`../../13-lineage-quality.md`](../../13-lineage-quality.md) |
| MVP | [`../../16-lineage-mvp.md`](../../16-lineage-mvp.md) |

This pack adds **working records**: a 13-row lineage register, applied criticality labels, business and conceptual examples, selective field-level hops, quality checks, and catalog back-references.

---

## 2. What lineage is (working definition) `[A][B]`

**Lineage** is a governed description of how data moves: Source → Transformation → Target → Consumer.

It is **not** the underlying patient, clinical, or claims data. Publishing lineage metadata is **not** an access grant and **not** a data release.

```text
Data Catalog
      ↓
Data Asset (Phase 8 metadata)
      ↓
Lineage Reference
      ↓
Source / Transformation / Target / Consumer
```

The catalog points to lineage. Lineage points back to catalog assets. Metadata field definitions are **not** duplicated here; they remain in the Phase 8 working pack.

---

## 3. Locked lifecycle (applied, not redesigned)

```text
Identify lineage scope
→ Identify source
→ Identify movement
→ Identify transformation
→ Identify target
→ Identify consumer
→ Validate lineage
→ Approve lineage
→ Publish lineage
→ Maintain lineage
→ Review lineage
→ Retire lineage
```

The applied registration path is in [`lineage-registration-workflow.md`](lineage-registration-workflow.md). It extends the locked workflow. It does **not** create a seventh Phase 6 procedure.

---

## 4. Catalog + lineage integration `[A][B]`

Phase 8 treats Lineage Metadata as **capability-dependent**:

| Phase 8 field | Working-pack use |
| --- | --- |
| **Upstream source** | Source catalog asset or system context |
| **Downstream consumers** | Target uses (report, interchange, process) — not access grants |
| **Transformation reference** | Conceptual transformation name — not ETL code |
| **Lineage Reference** (working inventory) | Pointer such as `LIN-001` / chain `LIN-REG-PAT-001` |

Year-1 catalog exposure remains **asset-level**:

```text
Source → Target → Consumer
```

That is governed metadata for discovery. It is **not** Restricted or Confidential **data**.

Catalog assets used here reuse Phase 8 working-pack IDs (`META-PAT-*`, `META-ENC-*`, `META-CLM-*`). See [`../../../08-metadata-catalog/working-pack/metadata-inventory/metadata-inventory.md`](../../../08-metadata-catalog/working-pack/metadata-inventory/metadata-inventory.md).

---

## 5. Asset mapping (locked Phase 9 MVP names → catalog IDs)

| Phase 9 MVP asset | Catalog working-pack ID | Catalog name |
| --- | --- | --- |
| Patient Master Record | META-PAT-001 | Patient |
| Encounter / Diagnosis record | META-ENC-001 / META-ENC-002 | Encounter / Encounter Documentation Dataset |
| Claims Extract | META-CLM-001 | Claim Submission Dataset |

No new MVP domains. No new CDEs. Provider and Facility remain outside Year-1 operating scope.

---

## 6. Illustrative platform mapping to Microsoft Purview `[A][B]`

This section is an **illustrative platform mapping only**. Purview is **not** deployed. No scan, ingestion, workflow configuration, or screenshot is claimed.

| Rafid working concept | Illustrative Purview analogue |
| --- | --- |
| Lineage Registry / Lineage Record | Catalog asset lineage / process lineage as a possible later store |
| Business lineage | Glossary-to-asset relationships and documented business flows |
| Conceptual lineage (Source → Target → Consumer) | Asset-level lineage edges |
| Selective field-level lineage | Column lineage **if later populated and justified** — not Year-1 enterprise coverage |
| Critical Lineage Register | Custom governance attribute or collection — not an automatic Purview score |
| Steward validation / Owner approval | Catalog workflow / approval (however a tenant might later be configured) |
| IT / Data Custodian technical facts | Scanned technical metadata as **input**, never as Data Owner |

If Purview were later selected, Rafid occupancy rules, Owner **A** for business meaning, and the two-step criticality rule would still apply. The tool would not become Data Owner and would not make a flow Critical Lineage automatically.

---

## 7. What this file does not do

- Does not replace Phase 8 or Phase 9 locked design
- Does not implement automated lineage, a graph database, or ETL
- Does not claim Microsoft Purview (or any other tool) was deployed
- Does not claim NDMO or PDPL compliance
