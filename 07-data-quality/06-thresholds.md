# Quality Thresholds

**Document ID:** RHC-DG-P7-006  
**Version:** 1.0  
**Status:** Implemented (illustrative thresholds only)  
**Owner:** Domain Data Owner **A** for thresholds on that domain’s CDE rules; DMO owns the threshold method `[B]`  
**Approver:** CDO `[B]` (method); Data Owner **A** (domain application)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Target / Warning / Breach; numeric examples labeled illustrative.

**Phase:** 7 — Data quality  
**Does not decide:** Live Rafid targets; regulator-imposed numbers; NDMO official thresholds `[NDMO verification required]`

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records **how** Rafid sets quality thresholds and shows **illustrative** numbers for teaching the model `[A][B]`.

Every numeric example in this file is:

**`[A] Illustrative Rafid target`**

Numeric examples are **not**:

- NDMO requirements
- Regulatory requirements
- Real Rafid performance

Specific NDMO thresholds remain `[NDMO verification required]`. **No compliance is claimed.**

---

## 2. Three-level model (locked) `[A][B]`

| Level | Meaning |
| --- | --- |
| **Target** | The intended operating level for the rule in the current lifecycle stage. |
| **Warning threshold** | Steward attention and Domain Huddle visibility; not automatically a DMC item. |
| **Breach threshold** | Issue is logged (if not already) and treated as a quality breach for that rule. |

Warning is **not** a numeric SLA clock. Breach is **not** an automatic Policy exception. Out-of-policy handling still uses the Data Governance Exception Procedure with **DMC = A**.

---

## 3. Thresholds may vary `[A][B]`

The same dimension does **not** require the same numbers everywhere. Owners may set different Target / Warning / Breach values according to:

- **CDE criticality** (patient-safety identity vs reference code drift)
- **Domain**
- **Business impact** of a defect
- **Lifecycle stage** (new interface vs stable process)
- **Confirmed regulatory context** — only where a requirement is verified; otherwise `[NDMO verification required]` and do not invent a number as “the law”

DMO challenges inconsistency of **method**, not as a second Data Owner.

---

## 4. Illustrative numeric examples `[A] Illustrative Rafid target`

These figures exist so the scorecard and rules have a **worked example**. They must be briefed as fiction.

### Completeness-style rules (example: DQ-003, DQ-006)

| Level | Illustrative value |
| --- | --- |
| Target | 98% |
| Warning | 95% |
| Breach | 90% |

**`[A] Illustrative Rafid target`** — not NDMO, not regulatory, not measured Rafid performance.

### Validity-style rules (example: DQ-002, DQ-007)

| Level | Illustrative value |
| --- | --- |
| Target | 99% |
| Warning | 97% |
| Breach | 95% |

**`[A] Illustrative Rafid target`**

### Uniqueness-style rules (example: DQ-001, DQ-005)

Uniqueness is often expressed as duplicate-group count rather than a percentage.

| Level | Illustrative value |
| --- | --- |
| Target | 0 duplicate groups (except documented exceptions) |
| Warning | 1 duplicate group in the governed population |
| Breach | 2 or more duplicate groups |

**`[A] Illustrative Rafid target`**

Optional percentage expression (same fiction): Target 100%, Warning 99.5%, Breach 99.0% — still **`[A] Illustrative Rafid target`**.

### Timeliness-style rules (example: DQ-004)

| Level | Illustrative value |
| --- | --- |
| Target | 0 undetected expired-active credentials |
| Warning | 1 |
| Breach | 2 or more |

**`[A] Illustrative Rafid target`**

### Integrity-style rules (example: DQ-008)

| Level | Illustrative value |
| --- | --- |
| Target | 0 orphan facility/department codes in agreed extracts |
| Warning | Isolated orphan codes in a single extract |
| Breach | Repeated orphan codes across extracts |

**`[A] Illustrative Rafid target`** (qualitative breach language is allowed where a percentage would fake precision).

---

## 5. Applying a threshold to an issue

| Observation vs threshold | Governance action |
| --- | --- |
| Meets Target | Continue Steward monitoring |
| Crosses Warning, not Breach | Steward investigates; Domain Huddle notes trend |
| Crosses Breach | Follow Data Quality Issue Management Procedure (`06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`) |

No numeric response SLA is added.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative numbers and three-level model application | Sections 4–5 |
| `[B]` | Target / Warning / Breach; variation by criticality | Method |
| `[C]` | Data Quality domain **name**; Trusted Data principle **name** | Context |
| `[NDMO verification required]` | Official NDMO or sector numeric quality thresholds | Not claimed |
