# Lineage Registration Workflow (Working Pack)

**Document ID:** RHC-DG-P9-WP-004  
**Version:** 1.0  
**Status:** Implemented (operating design only — not a ticket-tool build)  
**Owner:** DMO `[B]` (workflow method)  
**Parent design:** [`../../12-registration-workflow.md`](../../12-registration-workflow.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

**Synthetic / Illustrative / Non-production.**

---

## 1. Purpose

This is the **working 12-step path** for registering a lineage record.

It is consistent with Phase 9, Phase 8 catalog registration, and Phase 6. It does **not** create a second registration procedure. It does **not** invent a document ID. No ticket product and no numeric SLA are specified.

Assets on a lineage path should already be identifiable in the catalog, or registered through:

**Metadata Registration Procedure**

`06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md`

---

## 2. Locked Phase 9 workflow (unchanged)

```text
Identify lineage requirement
→ Gather source/target information
→ Document transformation
→ Steward validation
→ Owner validation where required
→ DMO governance check
→ Publish
→ Review/update
```

---

## 3. Working 12-step path (extension)

```text
1. Identify Lineage Requirement
2. Register Lineage (draft ID)
3. Assign Owner / Steward
4. Document Source and Target
5. Document Transformation
6. Identify Consumer
7. Assess Criticality
8. Validate Lineage
9. Approve Where Required
10. Publish / Record
11. Maintain
12. Periodic Review (and Retire when applicable)
```

```text
Identify Lineage Requirement
        ↓
Register Lineage
        ↓
Assign Owner / Steward
        ↓
Document Source and Target
        ↓
Document Transformation
        ↓
Identify Consumer
        ↓
Assess Criticality
        ↓
Validate Lineage
        ↓
Approve Where Required
        ↓
Publish / Record
        ↓
Maintain
        ↓
Periodic Review
```

---

## 4. Steps

### Step 1 — Identify Lineage Requirement

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward **R**; Owner and DMO on criticality confirm |
| **Input** | Catalog asset; CDE; KPI; system change; or quality issue |
| **Action** | Decide whether a lineage record is needed at Levels 1–2 (or selective Level 4) |
| **Output** | Candidate on the Lineage Registry |
| **Decision** | In Year-1 MVP domains? If no, stop or keep as framework-only. If yes, continue |

### Step 2 — Register Lineage

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward |
| **Input** | Candidate source and target names |
| **Action** | Create a draft Lineage Record and assign Lineage ID (`LIN-nnn`) |
| **Output** | Draft record. Validation Status = Pending Steward Validation |
| **Decision** | ID issued? If the hop already exists, update that record instead of duplicating |

### Step 3 — Assign Owner / Steward

| Item | Working design |
| --- | --- |
| **Actor** | Steward records; DMO confirms titles match Phase 4 |
| **Input** | Source and target domains |
| **Action** | Copy Phase 4 Data Owner and Business Data Steward titles. Cross-domain hops record **target** Owner as primary on the row; source Owner remains **A** for the source asset |
| **Output** | Owner and Steward populated |
| **Decision** | Domain unambiguous? If two Owners appear to share **A** for one asset, stop — there is no shared Owner. DMO coordinates; DMO is not Owner |

### Step 4 — Document Source and Target

| Item | Working design |
| --- | --- |
| **Actor** | Steward **R**; Custodian **C** |
| **Input** | Catalog Asset IDs; system context (`SYN-REG`, `SYN-EHR`, `SYN-BILL`) |
| **Action** | Record source/target domain, asset, and element (element only when Level 4 is justified) |
| **Output** | Source and Target complete at the intended granularity |
| **Decision** | Catalog IDs exist? If the asset is missing, register it through PRC-004 / Phase 8 first |

### Step 5 — Document Transformation

| Item | Working design |
| --- | --- |
| **Actor** | Steward **R**; Custodian **C** |
| **Input** | Known movement (persist, join, code map, aggregate, outbound map) |
| **Action** | Write a **conceptual** transformation reference. Not job code. Not a claimed ETL implementation |
| **Output** | Transformation / Relationship populated, or explicitly “not yet known” |
| **Decision** | Conceptual step named? If unknown, record the gap — do not invent a mapping engine |

### Step 6 — Identify Consumer

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward |
| **Input** | Target asset; known reports, interchange, or processes |
| **Action** | Name the consumer (report, interchange, process). Consumer is **not** an access grant |
| **Output** | Consumer recorded on the Lineage Record / Notes |
| **Decision** | External consumer? Sharing still uses two Phase 4 decisions (Owner business **A**; PDPO privacy **A** where personal data applies). Lineage does not merge them |

### Step 7 — Assess Criticality

| Item | Working design |
| --- | --- |
| **Actor** | Steward identifies criteria; Owner, Steward, and DMO confirm coverage |
| **Input** | Nine candidacy criteria; working labels Critical / Important / Standard |
| **Action** | Fire candidacy, then confirm whether prioritized coverage is warranted **now** |
| **Output** | Criticality label; Critical Lineage Register flag if confirmed Critical |
| **Decision** | Confirmed Critical? If no, still record Important or Standard. Do not auto-promote |

### Step 8 — Validate Lineage

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward |
| **Input** | Draft record; catalog; lineage-quality checks |
| **Action** | Check completeness of Source → Transformation → Target → Consumer at the intended granularity; catalog IDs consistent; no Restricted **data** pasted into the record |
| **Output** | Pass, or a gap list. Validation Status may move to Steward Validated |
| **Decision** | Pass → Step 9. Fail → return to Steps 4–7 |

### Step 9 — Approve Where Required

| Item | Working design |
| --- | --- |
| **Actor** | Data Owner **A** when the flow’s **business meaning** is at stake; DMO governance check |
| **Input** | Steward-validated record |
| **Action** | Owner accepts business lineage correctness. DMO checks method, registry consistency, and that clinical/finance meaning was not rewritten |
| **Output** | Owner Approved; DMO Checked |
| **Decision** | Owner accepts? If no, return with comments. DMO check fail? Return for completeness — DMO still does not rewrite meaning |

DMC does **not** approve every lineage record. DMC remains **A** only for existing Phase 3 classes.

### Step 10 — Publish / Record

| Item | Working design |
| --- | --- |
| **Actor** | Steward / DMO |
| **Input** | Approved record in MVP domain |
| **Action** | Set Validation Status = Published. Write Phase 8 Lineage Metadata on the catalog asset (upstream, downstream, transformation reference, Lineage Reference) |
| **Output** | Lineage Record on the registry; catalog pointer updated; Critical Lineage Register row if confirmed |
| **Decision** | In MVP scope? If no, keep as registered framework inventory — do not present it as Year-1 lineage operating coverage |

### Step 11 — Maintain

| Item | Working design |
| --- | --- |
| **Actor** | Steward **R**; Custodian **C** for technical facts |
| **Input** | Approved change triggers ([`../../14-change-management.md`](../../14-change-management.md)) |
| **Action** | Update the Lineage Record and catalog pointer when a trigger fires. Create a Lineage Change Record |
| **Output** | Current record |
| **Decision** | Material business-meaning change? Return to Owner approval |

### Step 12 — Periodic Review (and Retire)

| Item | Working design |
| --- | --- |
| **Actor** | Steward **R**; Owner **A** for material change; DMO retains retired records |
| **Input** | Published record; known system or definition changes |
| **Action** | Confirm source, target, transformation, consumer, criticality, and ownership. Or set Retired |
| **Output** | Last Reviewed updated, or a retained retired record |
| **Decision** | Still operational? If no, Owner + DMO retire. No numeric review SLA |

---

## 5. Alignment

| Working steps | Locked Phase 9 | Phase 8 / Phase 6 |
| --- | --- | --- |
| 1–2 | Identify lineage requirement | Identify / register related catalog assets (PRC-004) |
| 3 | Ownership recorded | Phase 4 titles; no new roles |
| 4–6 | Gather source/target; document transformation; consumer | Phase 8 Lineage Metadata fields |
| 7 | Criticality confirm | [`../../05-lineage-criticality.md`](../../05-lineage-criticality.md) |
| 8–9 | Steward validation; Owner validation where required; DMO check | Same pattern as catalog publish |
| 10 | Publish | Catalog Lineage Reference updated |
| 11–12 | Review/update; retire | Change triggers; exception path unchanged |

---

## 6. Exceptions

Out-of-policy lineage handling reuses:

**Data Governance Exception Procedure**

`06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md`

**DMC = A** (existing right). No new exception procedure.

---

## 7. What this file does not do

- Does not create a seventh Phase 6 procedure
- Does not add a lineage-only Owner or a new DMC decision class
- Does not implement a service-management tool
- Does not treat publish as PDPL authorization
