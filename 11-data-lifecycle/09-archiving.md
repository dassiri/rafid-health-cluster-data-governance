# Archiving

**Document ID:** RHC-DG-P11-009  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** for archive eligibility in the domain; DMO for Archive Register `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Active / Archived / Disposed; Archive ≠ Backup; no storage technology.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Archive platform, tape, object storage, or WORM products

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records **conceptual** archive governance `[A][B]`.

**Do not design storage technology.**  
**Archive ≠ Backup.**

Specific NDMO archiving requirements remain `[NDMO verification required]`. Healthcare archive obligations remain `[Legal / regulatory verification required]`.

---

## 2. Three states (locked)

```text
Active Data
→ Archived Data
→ Disposed Data
```

| State | Meaning |
| --- | --- |
| **Active Data** | Needed for current operations or frequent use |
| **Archived Data** | Reduced active business use; still **retained** under a rule; still classified; still subject to hold |
| **Disposed Data** | Authorized disposal completed and evidenced ([10](10-disposal-destruction.md), [11](11-disposal-evidence.md)) |

Archived data has **not** been disposed. Classification **persists** unless the Owner reclassifies (Phase 5).

---

## 3. Archive eligibility (conceptual) `[A][B]`

A candidate may be considered for archive when **one or more** apply:

- Reduced active business use  
- Retention requirement still in force (period **verified** or still pending — do not invent)  
- Historical / reference value  
- Legal / record requirements (when verified)

Eligibility is **not** “put it on a backup.” Backup supports recovery and continuity ([03](03-lifecycle-vs-records-vs-backup.md)).

---

## 4. Archive ≠ Backup (locked)

| | Archive | Backup |
| --- | --- | --- |
| Purpose | Governed **lifecycle** state while still retaining | **Recovery** and continuity |
| Governance | Owner, classification, retention rule, hold, disposal eligibility | Continuity design (out of this phase) |
| Discovery | Catalog / Archive Register | Not a substitute catalog |
| Disposal | Follows verified rule + hold check + Owner authorization | Backup expiry is not Retention Schedule |

---

## 5. Conceptual archive metadata `[A][B]`

| Field | Intent |
| --- | --- |
| Archive date | When the asset entered archive state |
| Source asset | Catalog asset / record type archived |
| Owner | Phase 4 Data Owner title |
| Classification | Rafid tier — persists |
| Retention rule | Link to Retention Rule ID |
| Legal hold status | Hold overrides disposal |
| Disposal eligibility | Not eligible while hold active or period unverified |
| Retrieval requirements | Who may retrieve and for what purpose — conceptual, not a retrieval SLA |

No media, path, or vendor is specified.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Three states; eligibility; metadata; Archive ≠ Backup | Sections 2–5 |
| `[NDMO verification required]` | Official NDMO archive specifications | Not claimed |
| `[Legal / regulatory verification required]` | Healthcare archive law | Not invented |
