# Operating Workflow

**Document ID:** RHC-DG-P3-007  
**Phase:** 3 — Operating model  
**Status:** Approved / Implemented  
**Does not decide:** Ticket tools, SLA numbers, or Phase 4 routing table by domain

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records the approved end-to-end governance workflow for the fictional Rafid Health Cluster `[A]`. It is an operating design `[B]`, not a system specification and not an NDMO procedure pack.

---

## 2. End-to-end workflow `[B]`

```text
Data issue / request
    → Intake (DGO routing rules; Business Data Steward of the owning domain)
    → Business Data Steward (investigate, draft)
    → Data Owner (in-policy decision)
         ↳ if cross-domain or Owner conflict → DGO mediate → CDO
         ↳ if policy exception or residual risk → Data Management Committee
         ↳ if material regulatory / entity risk → Executive Sponsor
    → Decision (logged against class: operational / tactical / strategic)
    → Implementation (Custodian if system change; Steward if process/content)
    → Monitoring (Steward + DGO KPI / issue ageing)
```

Until Phase 4 assigns Owners, “owning domain” is a **routing design**, not an assignment of named Owners.

---

## 3. Variant — in-policy access request

Consumer → Business Data Steward (completeness) → **Data Owner A** → Custodian provisions → Consumer **I**.

PDPO is **C** when the data are personal or health-related `[A]` landscape + PDPO role `[C]` name. PDPL operational mapping `[NDMO verification required]`.

---

## 4. Variant — external or high-risk share

Same as access, then PDPO + Legal Advisor **C**. If novel or high-risk → **Data Management Committee A**.

NDMO describes a sharing process that includes Business Data Executive approval `[C]`. Regulation-level steps are `[NDMO verification required]`.

---

## 5. Classes (from Phase 2) `[B]`

| Class | Typical landing |
| --- | --- |
| Operational | Steward execution; Owner decision |
| Tactical | DGO / CDO (methods, mediation, standard proposals) |
| Strategic | Data Management Committee; CEO for residual / material regulatory |

---

## 6. Intentionally unresolved

- Which domain receives an issue when ownership is ambiguous — Phase 4
- Tooling for intake (service desk vs register) — not a Phase 3 decision
- Issue register format — later artifact; NDMO later expects governance artifacts. Control-level citation `[NDMO verification required]`

---

## 7. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 3 Implementation Brief | Workflow and variants |
| `[C]` | NDMO Standards v1.5 — BDE in sharing process (as stated); PDPO **name** | Share and privacy consult |
| `[NDMO verification required]` | Sharing regulation; artifact control IDs | Not treated as verified here |
