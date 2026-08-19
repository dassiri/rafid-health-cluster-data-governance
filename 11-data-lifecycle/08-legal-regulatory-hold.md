# Legal / Regulatory Hold

**Document ID:** RHC-DG-P11-008  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for affected domain assets; DMO for hold register `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual hold process; no invented litigation rules.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Litigation strategy; what constitutes a legal hold in Saudi law

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records a **conceptual** legal / regulatory hold process `[A][B]`.

**This is not legal advice.**  
**Do not invent litigation rules.**  
Whether a given event requires a hold remains `[Legal / regulatory verification required]`.

An **active hold overrides normal disposal**.

---

## 2. Process (locked)

```text
Identify hold
→ Apply hold
→ Suspend normal disposition
→ Register affected assets/records
→ Monitor hold
→ Release hold
→ Resume approved lifecycle
```

| Step | Governance activity | Role |
| --- | --- | --- |
| Identify hold | Notice that preservation may be required (legal, regulatory, investigation — **not** invented criteria) | Legal / authorized requestor; Data Owner **C**; DMO **C** |
| Apply hold | Mark assets so they are not treated as disposal candidates | Business Data Steward **R**; Custodian technical; Data Owner **A** for domain confirmation |
| Suspend normal disposition | Stop archive-to-destroy and other disposal against held items | Custodian **R**; Business Data Steward **R** |
| Register affected assets/records | Legal / Regulatory Hold Register | DMO / Business Data Steward |
| Monitor hold | Confirm hold still applies and coverage remains complete | Business Data Steward **R**; DMO oversight |
| Release hold | Authorized release — **not** a local informal decision | Same authority pattern as apply; Legal **C** |
| Resume approved lifecycle | Return to Retention Schedule / archive / disposal **only if still eligible** | Data Owner **A**; Custodian implements |

DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework. **No new DMC decision right.** This file does **not** make DMC the litigation authority.

---

## 3. Override rule (locked) `[A][B]`

| Situation | Effect |
| --- | --- |
| Retention period **placeholder** still unverified | Do **not** dispose on a guessed clock |
| Retention period verified and expired, **no** hold | Eligible for Owner-authorized disposal process |
| **Active hold** | **Do not dispose**, even if a verified period would otherwise have expired |
| Hold released | Re-check eligibility, classification, and remaining purpose before any disposal |

Backup copies used for recovery are **not** a hold register ([03](03-lifecycle-vs-records-vs-backup.md)).

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Conceptual hold chain and override | Sections 2–3 |
| `[C]` | Role **names** | Naming |
| `[Legal / regulatory verification required]` | When a hold is legally required; litigation rules | Not invented |
| `[NDMO verification required]` | Official NDMO hold specifications | Not claimed |
