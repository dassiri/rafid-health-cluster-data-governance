# Retention Governance

**Document ID:** RHC-DG-P11-006  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for the retention **rule** (Phase 4 row 10); DMO for method and register `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual decision chain; no invented periods.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Numeric periods; healthcare statutes

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records a **conceptual retention decision framework** `[A][B]`.

**Do not invent numeric retention periods.**  
**Do not invent healthcare-specific legal retention periods.**

The **period** field is filled only after verification. Until then it remains `[NDMO verification required]` and/or `[Legal / regulatory verification required]`.

This is **not** legal advice.

---

## 2. Decision chain (locked)

```text
Identify data / record
→ Identify business purpose
→ Identify applicable requirements
→ Identify retention trigger
→ Determine retention period
→ Owner approval
→ Register retention rule
→ Monitor
→ Review
→ Archive or dispose
```

| Step | Governance activity | Role |
| --- | --- | --- |
| Identify data / record | Name the asset or record type in catalog terms (Phase 8) | Business Data Steward **R**; Data Owner **A** |
| Identify business purpose | Why the data exists and why it is kept | Data Owner **A** |
| Identify applicable requirements | Business, records, legal/regulatory, contractual (if any), privacy | Data Owner **A**; PDPO **C** where personal data; Legal **C** where legal risk — **not** invented |
| Identify retention trigger | Event that starts the clock (examples below) | Business Data Steward **R**; Data Owner **A** |
| Determine retention period | **Verified** duration after the trigger — **placeholder until verified** | Data Owner **A**; DMO **C** |
| Owner approval | Retention/lifecycle decision (Phase 4 row 10) | Data Owner **A** |
| Register retention rule | Record in Retention Schedule | DMO / Business Data Steward |
| Monitor | Watch trigger, hold, and eligibility | Business Data Steward **R**; Custodian technical |
| Review | Recheck purpose and verified requirements | Data Owner **A** |
| Archive or dispose | Follow [09](09-archiving.md) or [10](10-disposal-destruction.md) | Data Owner **A** to authorize; Custodian implements |

DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework. **No new DMC decision right.** DMC is not the routine approver of every retention rule.

---

## 3. Illustrative retention triggers `[A]`

These are **illustrative** trigger **types**. They are **not** periods.

| Trigger (illustrative) `[A]` | Typical meaning |
| --- | --- |
| **Creation date** | Clock starts when the record is created |
| **Last activity** | Clock starts after last operational use |
| **Case closure** | Clock starts when a case/incident is closed |
| **Contract termination** | Clock starts when a contract ends |
| **Patient relationship end** | Clock starts when the care relationship ends (definition to be confirmed operationally) |
| **Record completion** | Clock starts when the record is completed |

**Do not** treat a trigger as a duration. Duration remains a verification placeholder until confirmed.

---

## 4. What “determine retention period” means here

Until a requirement is verified, the Retention Period field is recorded as:

- `[NDMO verification required]` and/or  
- `[Legal / regulatory verification required]`

No invented number is used as a working default. **No indefinite retention by default** (principle in [02](02-lifecycle-principles.md)) means silence is not a keep-forever rule — it means the rule is **incomplete** until verified and approved.

Classification **does not** fill this field ([05](05-lifecycle-and-classification.md)).

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Decision chain; Owner A | Section 2 |
| `[A]` | Illustrative triggers | Section 3 |
| `[C]` | Role **names** | Naming |
| `[NDMO verification required]` | Official NDMO retention specifications | Period field |
| `[Legal / regulatory verification required]` | Healthcare retention law | Period field |
