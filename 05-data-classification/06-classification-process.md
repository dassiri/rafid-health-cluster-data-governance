# Classification Process

**Document ID:** RHC-DG-P5-006  
**Phase:** 5 — Data classification  
**Status:** Implemented  
**Does not decide:** Ticketing tools, numeric SLAs, or Phase 6 SOP text

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. End-to-end flow `[B]`

```text
Data created / acquired
    → Identify dataset
    → Determine classification (Steward proposes; qualitative highest impact)
    → Owner approval
    → Steward records classification (registry)
    → DMO oversight (consistency)
    → Technical implementation (Custodian; not a decision)
    → Periodic review
    → Reclassification when triggered (Owner approval only)
```

No numeric review SLA. “Periodic” is qualitative and tied to DMC/DMO oversight cadence from Phase 3, not a day-count.

---

## 2. Handling by data state `[B]`

| State | Handling |
| --- | --- |
| **New data** | Identify as a dataset before broad use. Steward proposes; Owner approves **before** (or as a condition of) operational release. |
| **Existing data** | Treat as in-scope even if historically unlabeled. Steward flags; Owner approves an initial Rafid tier. Unlabeled is not “Public.” |
| **Imported data** | Receiving-domain Owner is **A** for the Rafid tier **as used in the cluster**. Source labels (vendor, other cluster) inform but do not bind. PDPO **C** if personal. |
| **Derived data** | Classify the **derived dataset** on its own impact. Default: not weaker than the highest input unless Owner approves a documented reason (for example de-identification). |
| **Aggregated data** | Aggregation does not auto-downgrade. Owner approves the aggregate dataset’s tier. |
| **Shared data** | Sharing does not change classification by itself. Apply [`09-access-sharing-consequences.md`](09-access-sharing-consequences.md). External Restricted shares use the approved wording in that file. |
| **Archived data** | Classification **persists** in archive unless the Owner reclassifies. Disposal still follows lifecycle (Phase 11) under the current tier. Classification does **not** automatically determine retention duration. |

---

## 3. Identify dataset

Steward (with Custodian **C** for system boundaries) names the dataset, domain, and related systems. If two domains overlap, Phase 4 ownership decides **which Owner is A**; do not dual-classify as two Owners’ **A**.

---

## 4. Determine and approve

1. Steward documents qualitative impacts (no scores).  
2. PDPO reviews if personal data is involved.  
3. Data Owner **approves** the Rafid tier.  
4. Custodian implements handling.  
5. DMO checks the registry entry is complete.

IT must not “set Restricted because the folder is in the EMR.” That is not a classification decision.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 5 process | All sections |
| `[A]` | Rafid domains/Owners | Who approves |
| `[C]` | PDPO **name**; NCA mandate for security implementation coordination | Consult vs implement |
| `[NDMO verification required]` | Official national process steps / regulation | Not copied as Rafid SOP |
