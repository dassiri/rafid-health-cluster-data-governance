# Retention Exceptions

**Document ID:** RHC-DG-P11-021  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Requesting Data Owner; DMC remains **A** for Policy-level exceptions (existing)  
**Approver:** CDO `[B]` (process documentation)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** With the exception procedure `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Existing exception procedure reused; no new decision right; title/path only.

**Phase:** 11 — Data lifecycle  
**Does not decide:** A new exception Accountable

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records how **retention / lifecycle exceptions** are handled without creating a new decision right.

**Do NOT create a new decision right.**

Use the existing **Data Governance Exception Procedure** (title and path only):

`06-policies-standards-procedures/procedures/06-data-governance-exception-procedure.md`

No document ID is invented or restated here.

Time-boxed waivers **inside** an already approved Policy envelope remain as that procedure already describes. Out-of-Policy requests remain **DMC Accountable** as already designed. This phase does **not** add a DMC class.

DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework.

---

## 2. Process (locked)

```text
Identify exception
→ Document reason
→ Identify affected data
→ Risk assessment
→ Approval under existing governance authority
→ Register exception
→ Review
→ Close
```

| Step | Activity |
| --- | --- |
| Identify exception | Proposed keep, archive, or dispose that does **not** follow the approved Retention Rule (including a request to keep while the period is still unverified, or to dispose while unverified) |
| Document reason | Business, operational, or other justification — **not** an invented legal period |
| Identify affected data | Domain, asset/record type, classification, personal-data flag |
| Risk assessment | Quality, privacy, lineage, hold, and handling risk — PDPO **C** where personal data |
| Approval under existing governance authority | Follow the Data Governance Exception Procedure at the path above — **no new A** |
| Register exception | Retention Exception Record `[A]` Proposed Rafid governance artifact |
| Review | Time-box and compensating controls as the existing procedure requires |
| Close | Close or renew under that same existing authority |

An active **legal / regulatory hold** is **not** an “exception to keep.” It is a hold ([08](08-legal-regulatory-hold.md)).

---

## 3. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Exception chain mapped to existing procedure | Section 2 |
| `[C]` | Role **names** | Naming |
| `[NDMO verification required]` | Official NDMO exception specs | Not claimed |
| `[Legal / regulatory verification required]` | Whether an exception is lawful | Not invented |
