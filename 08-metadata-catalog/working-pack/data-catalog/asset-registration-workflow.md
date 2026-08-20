# Asset Registration Workflow (Working Pack)

**Document ID:** RHC-DG-P8-WP-010  
**Version:** 1.0  
**Status:** Implemented (operating design only — not a ticket-tool build)  
**Owner:** DMO `[B]` (workflow method)  
**Parent design:** [`../../07-asset-registration-workflow.md`](../../07-asset-registration-workflow.md) and PRC-004  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice

---

## 1. Purpose

This is the **working 13-step path** for registering a data asset into the conceptual catalog.

It is consistent with Phase 6 (PRC-004) and Phase 8. It does **not** create a second registration procedure. No ticket product and no numeric SLA are specified.

```text
1. Identify Data Asset
2. Submit Registration Request
3. Assign Data Owner
4. Assign Business Data Steward
5. Complete Minimum Metadata
6. Apply Classification
7. Identify CDE Status
8. Validate Metadata
9. Resolve Missing Information
10. Approve Asset
11. Publish to Catalog
12. Periodic Review
13. Update or Retire
```

Steps 3–4 usually **record** the Phase 4 domain assignment rather than invent a new Owner.

---

## 2. Steps

### Step 1 — Identify Data Asset

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward; IT / Data Custodian **C** |
| **Input** | Operational use, system change, or DMO intake note |
| **Action** | Name the candidate; propose domain and asset type |
| **Output** | Candidate on the intake list |
| **Decision** | Is this a catalog asset (Dataset, Master Data Entity, or in-scope element)? If no, stop. If yes, continue |

### Step 2 — Submit Registration Request

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward |
| **Input** | Candidate name; domain hypothesis; source system class if known |
| **Action** | Create a draft record and assign Asset ID |
| **Output** | Draft catalog record. Lifecycle Status = Draft. Approval Status = Pending Steward Validation |
| **Decision** | ID issued? If the asset already exists, update that record instead of duplicating |

### Step 3 — Assign Data Owner

| Item | Working design |
| --- | --- |
| **Actor** | Steward records; DMO confirms the title matches Phase 4 |
| **Input** | Business Domain |
| **Action** | Copy the Phase 4 Data Owner title onto the record |
| **Output** | Business Owner populated |
| **Decision** | Domain unambiguous? If two domains appear to fit, escalate to DMO / CDO using existing Phase 3 paths — do not create shared ownership |

### Step 4 — Assign Business Data Steward

| Item | Working design |
| --- | --- |
| **Actor** | Data Owner (already nominated the steward); Steward / DMO records the title |
| **Input** | Domain; Steward Registry |
| **Action** | Record the Phase 4 appointed steward title |
| **Output** | Business Data Steward populated |
| **Decision** | Seat recorded? If vacant, Owner nominates before publish. DMO does not act as Owner |

### Step 5 — Complete Minimum Metadata

| Item | Working design |
| --- | --- |
| **Actor** | Steward **R**; Custodian supplies technical fields |
| **Input** | Draft record; occupancy rules |
| **Action** | Fill Required fields and any Conditional fields that apply. Do not invent quality or lineage values |
| **Output** | Minimum metadata complete enough for classification and CDE flagging |
| **Decision** | Required fields present? If no, remain Draft |

### Step 6 — Apply Classification

| Item | Working design |
| --- | --- |
| **Actor** | Data Owner **A**; Steward prepares the pack |
| **Input** | Phase 5 method; existing Classification Registry if the dataset is already classified |
| **Action** | Apply Public / Internal / Confidential / Restricted. If unlabeled, complete PRC-002 first |
| **Output** | Classification on the record |
| **Decision** | Tier assigned? **Unlabeled is not Public.** Elements inherit parent dataset context in this pack |

### Step 7 — Identify CDE Status

| Item | Working design |
| --- | --- |
| **Actor** | Steward records; Data Owner confirms for the domain |
| **Input** | Phase 7 catalogue (exactly 13 CDEs); domain watch-item list |
| **Action** | For Data Element rows: Yes — {CDE-ID}, No — watch-item, or No. Do **not** add CDEs |
| **Output** | CDE Status populated on element rows |
| **Decision** | Is this one of the 13? If a new candidate appears, it remains a watch-item until the two-step CDE method is run. That work is Phase 7, not this workflow |

### Step 8 — Validate Metadata

| Item | Working design |
| --- | --- |
| **Actor** | Business Data Steward |
| **Input** | Completed draft; occupancy rules; glossary |
| **Action** | Check completeness, Owner/domain consistency, glossary links, and that underlying data was not pasted into the record |
| **Output** | Pass, or a gap list. Trust status may move to **Reviewed** |
| **Decision** | Pass → Step 10. Fail → Step 9 |

### Step 9 — Resolve Missing Information

| Item | Working design |
| --- | --- |
| **Actor** | Steward coordinates; Custodian for technical gaps; Owner if meaning is missing |
| **Input** | Gap list |
| **Action** | Fill missing Required / applicable Conditional fields. DMO cannot rewrite clinical or finance meaning to “complete” the register |
| **Output** | Updated draft. Approval Status = Returned until re-validated |
| **Decision** | Gaps closed? Re-enter Step 8. If an out-of-policy exception is requested, use the Data Governance Exception Procedure (**DMC = A**) |

### Step 10 — Approve Asset

| Item | Working design |
| --- | --- |
| **Actor** | Data Owner **A** (content); DMO (governance check) |
| **Input** | Validated record |
| **Action** | Owner accepts definition and catalog content. DMO checks method completeness (Owner, domain, classification present) |
| **Output** | Approval Status = Approved. Certified is a separate Owner trust action when used |
| **Decision** | Owner accepts? If no, return with comments (Step 9). DMO check fail? Return for completeness — DMO still does not rewrite meaning |

Outside-MVP domains may be approved as **framework records** without Year-1 publish.

### Step 11 — Publish to Catalog

| Item | Working design |
| --- | --- |
| **Actor** | Steward / DMO |
| **Input** | Approved record in **MVP domain** |
| **Action** | Set Lifecycle Status = Active. Make **metadata** discoverable to MVP users |
| **Output** | Published catalog page (working record). Trust status at least **Registered** |
| **Decision** | In MVP scope? If no, keep as registered framework inventory — do not present it as Year-1 catalog operating coverage |

### Step 12 — Periodic Review

| Item | Working design |
| --- | --- |
| **Actor** | Steward **R**; Owner **A** for material change |
| **Input** | Published record; known system or definition changes |
| **Action** | Confirm meaning, classification, ownership, CDE flag, and lineage pointer |
| **Output** | Last Reviewed updated, or a change raised |
| **Decision** | Still correct? If yes, remain Active. If material change, re-enter approval. No numeric review SLA |

### Step 13 — Update or Retire

| Item | Working design |
| --- | --- |
| **Actor** | Steward maintains; Owner accepts material updates or retirement; DMO retains retired records |
| **Input** | Review outcome or system retirement |
| **Action** | Update metadata, or set Deprecated / Retired |
| **Output** | Current record, or retained retired record |
| **Decision** | Still in operational use? If no, Owner + DMO retire. Deprecated warns consumers not to start new work on it |

---

## 3. Path through forums

| Situation | Forum |
| --- | --- |
| In-domain definition / classification / catalog entry | Domain huddle |
| Cross-domain clash or catalog practice | Steward Forum |
| Intake routing only | DMO operations huddle |
| Policy exception; Owner non-participation | Data Management Committee (existing classes only) |

---

## 4. Alignment

| Working steps | Phase 8 | PRC-004 |
| --- | --- | --- |
| 1–2 | Identify, Register | Identify dataset, Register metadata |
| 3–4 | Assign ownership | Domain assignment already exists |
| 5–7 | Describe, Classify | Document definition, Link classification |
| 8–10 | Validate | Owner acceptance; DMO completeness |
| 11 | Publish | Result of register |
| 12–13 | Maintain, Review, Retire | Maintain |

---

## 5. What this file does not do

- Does not implement a service-management tool
- Does not add a catalog-only appeals committee
- Does not treat publish as PDPL authorization
