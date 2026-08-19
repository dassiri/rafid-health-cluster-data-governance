# Disposal / Destruction

**Document ID:** RHC-DG-P11-010  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for authorization; Custodian implements approved mechanism `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual disposal governance; no invented timeframes or mandatory methods.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Tools, shredder standards, crypto products, or vendor contracts

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records **secure disposal governance** at a conceptual level `[A][B]`.

**Do not prescribe technical implementation details.**  
**Do not invent disposal timeframes.**  
**Do not claim a particular disposal method is legally mandatory unless verified.**

NCA remains the security-control domain **name** `[C]`. This file does not implement NCA controls.

---

## 2. Process (locked)

```text
Identify disposal candidate
→ Verify retention expiry
→ Check legal hold
→ Owner authorization
→ Execute approved disposal
→ Record evidence
→ Close
```

| Step | Governance activity | Role |
| --- | --- | --- |
| Identify disposal candidate | Asset/record appears eligible under the Retention Schedule | Business Data Steward **R** |
| Verify retention expiry | Period must be **verified** and the trigger satisfied — **not** a guessed clock | Data Owner **A**; DMO **C** |
| Check legal hold | Active hold **blocks** disposal ([08](08-legal-regulatory-hold.md)) | Business Data Steward **R** |
| Owner authorization | Retention/lifecycle decision (Phase 4 row 10) | Data Owner **A** |
| Execute approved disposal | Custodian (or approved provider) uses the **approved conceptual method class** | IT / Custodian **R** |
| Record evidence | Disposal Record ([11](11-disposal-evidence.md)) | Business Data Steward / Custodian |
| Close | Closure status on Disposal Register | DMO oversight |

If the retention period is still `[NDMO verification required]` or `[Legal / regulatory verification required]`, the asset is **not** a confirmed disposal candidate.

DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework. **No new DMC decision right.**

---

## 3. Conceptual method classes `[A][B]`

These are **classes of approach**, not products and not claimed as legally mandatory:

| Method class | Meaning (conceptual) |
| --- | --- |
| **Secure deletion** | Information is removed from the governed store so it is not recoverable through ordinary use |
| **Cryptographic erasure where applicable** | Keys rendering ciphertext unusable — **where applicable**; not a mandate |
| **Physical destruction for applicable media** | Physical media destroyed when that media is in scope |
| **Controlled destruction by approved service provider** | Third party executes under Rafid authorization and evidence return |

**Classification influences handling** of disposal (Restricted requires the most careful handling band) but **does not** by itself select a legal method or a clock ([05](05-lifecycle-and-classification.md)).

PDPO is **C** where personal data is involved.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Process and method classes | Sections 2–3 |
| `[C]` | NCA mandate **name** for security domain; role **names** | Context |
| `[NDMO verification required]` | Official NDMO disposal specifications | Not claimed |
| `[Legal / regulatory verification required]` | Mandatory destruction methods or clocks | Not invented |
