# Metadata Lifecycle (Working Pack)

**Document ID:** RHC-DG-P8-WP-004  
**Version:** 1.0  
**Status:** Implemented (working design only)  
**Owner:** DMO `[B]` (method); Data Owner **A** for meaning and Certified status  
**Parent design:** [`../../01-framework-overview.md`](../../01-framework-overview.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This file is the **operating sequence** used in the working pack. It is consistent with the Phase 8 lifecycle and with PRC-004. It does **not** replace either.

Phase 8 locked sequence:

```text
Identify → Register → Describe → Classify → Assign ownership
→ Validate → Publish → Maintain → Review → Retire
```

Working sequence (same outcomes, more explicit approval gates):

```text
Identify
↓
Register
↓
Classify
↓
Assign Owner & Steward
↓
Complete Metadata
↓
Validate
↓
Approve
↓
Publish
↓
Review
↓
Update / Retire
```

Classify and ownership are placed **before** completing remaining metadata so unlabeled assets are not treated as Public, and so every record has an accountable Owner before it is described in full.

---

## 2. Stages

### 2.1 Identify

| Item | Working design |
| --- | --- |
| **Purpose** | Recognize a data asset (or CDE / watch-item element) in operational use |
| **Responsible** | Business Data Steward **R**; Custodian **C** |
| **Required metadata** | Working name; domain hypothesis; source system class if known |
| **Output** | Candidate asset on the intake list |

### 2.2 Register

| Item | Working design |
| --- | --- |
| **Purpose** | Create the governed catalog record with a stable Asset ID |
| **Responsible** | Business Data Steward **R**; DMO records the ID method |
| **Required metadata** | Asset ID; Asset Name; Asset Type (filled in this pack); Domain |
| **Output** | Draft record; Lifecycle Status = Draft; Approval Status = Pending Steward Validation |

Follows PRC-004 “Register metadata”.

### 2.3 Classify

| Item | Working design |
| --- | --- |
| **Purpose** | Apply a Rafid classification tier at dataset level (Phase 5). Elements inherit the parent dataset context unless a separate dataset exists |
| **Responsible** | Data Owner **A**; Steward **R** (pack); PRC-002 if not already classified |
| **Required metadata** | Classification (Public / Internal / Confidential / Restricted) |
| **Output** | Classification on the record. **Unlabeled is not Public.** |

### 2.4 Assign Owner & Steward

| Item | Working design |
| --- | --- |
| **Purpose** | Record the Phase 4 Owner and Steward for the domain |
| **Responsible** | Already assigned at domain level; Steward records the titles |
| **Required metadata** | Data Owner; Business Data Steward |
| **Output** | Accountable and executing roles visible on the asset |

Owner is not invented per table. One Owner per domain.

### 2.5 Complete Metadata

| Item | Working design |
| --- | --- |
| **Purpose** | Fill mandatory fields and any conditional fields that apply |
| **Responsible** | Steward **R**; Custodian supplies technical fields; Owner will later accept meaning |
| **Required metadata** | Business Definition; Source System; Lifecycle Status; Approval Status; CDE Status for element rows; other conditional fields when they apply |
| **Output** | Minimum metadata complete enough for validation |

This is Phase 8 **Describe**.

### 2.6 Validate

| Item | Working design |
| --- | --- |
| **Purpose** | Check completeness, internal consistency, and that Restricted/Confidential **data** was not pasted into the record |
| **Responsible** | Business Data Steward |
| **Required metadata** | All Required fields; Conditional fields that the occupancy rules say must be present |
| **Output** | Validation result: pass, or gap list. Trust status may move to **Reviewed** |

### 2.7 Approve

| Item | Working design |
| --- | --- |
| **Purpose** | Owner accepts meaning and catalog content; DMO performs the governance check |
| **Responsible** | Data Owner **A** (content); DMO (method completeness) |
| **Required metadata** | Owner-accepted Business Definition; classification present; Owner and Steward present |
| **Output** | Approval Status = Approved. Certified is a **separate** Owner action when the description is accepted as trustworthy for discovery |

DMO cannot rewrite meaning to force a pass.

### 2.8 Publish

| Item | Working design |
| --- | --- |
| **Purpose** | Make **metadata** discoverable to catalog personas. Not a data release |
| **Responsible** | Steward / DMO after approval |
| **Required metadata** | Phase 8 mandatory set (see [`../metadata-model/minimum-metadata-model.md`](../metadata-model/minimum-metadata-model.md)) |
| **Output** | Lifecycle Status = Active; trust status at least **Registered**; discoverable metadata page |

MVP publish is limited to the three approved domains.

### 2.9 Review

| Item | Working design |
| --- | --- |
| **Purpose** | Confirm meaning, classification, ownership, and CDE flag remain correct |
| **Responsible** | Steward **R**; Owner **A** for material change |
| **Required metadata** | Last Reviewed date (recommended); change note if anything moved |
| **Output** | Review confirmation, or an update/retire action |

No numeric review SLA is set.

### 2.10 Update / Retire

| Item | Working design |
| --- | --- |
| **Purpose** | Keep metadata current, or remove the asset from operational catalog use |
| **Responsible** | Steward maintains; Owner accepts material updates; Owner + DMO record-keeping for **Retired** |
| **Required metadata** | Updated fields; or Lifecycle Status = Deprecated / Retired |
| **Output** | Current record, or a retained retired record |

**Deprecated** = do not use for new work; still visible as a warning. **Retired** = no longer operational.

---

## 3. Mapping to Phase 6 and Phase 8

| Working stage | Phase 8 | PRC-004 |
| --- | --- | --- |
| Identify | Identify | Identify dataset |
| Register | Register | Register metadata |
| Classify | Classify | Link classification |
| Assign Owner & Steward | Assign ownership | (domain assignment already exists) |
| Complete Metadata | Describe | Document business definition |
| Validate / Approve | Validate | Owner acceptance; DMO completeness |
| Publish | Publish | Result of register |
| Review / Update / Retire | Maintain, Review, Retire | Maintain |

---

## 4. What this file does not do

- Does not invent numeric SLAs
- Does not automate catalog ingestion
- Does not treat publish as PDPL or access approval
