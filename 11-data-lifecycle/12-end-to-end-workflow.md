# End-to-End Lifecycle Workflow

**Document ID:** RHC-DG-P11-012  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (workflow method); Data Owner **A** at decision points  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Stage map reusing prior phases; no parallel frameworks.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Tools or SLAs

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records the **end-to-end lifecycle workflow** `[A][B]`.

**Reuse existing phases rather than creating parallel frameworks.**

DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework. **No new DMC decision right.**

---

## 2. Locked workflow

```text
Create / Acquire
→ Register
→ Classify
→ Assign Owner
→ Store / Use
→ Share where authorized
→ Monitor
→ Retain
→ Archive when appropriate
→ Dispose when eligible
```

---

## 3. Stage map

| Stage | Responsible role | Key governance activity | Key artifact / record | Relevant previous phase |
| --- | --- | --- | --- | --- |
| **Create / Acquire** | Data Owner **A** (domain); Business Data Steward **R**; Custodian technical | Data comes into existence or is received; identify domain | Source / intake context (operational) | Phase 4 domains |
| **Register** | Business Data Steward **R**; Data Owner **A** for catalog content | Metadata registration | Catalog entry; Metadata Registration Procedure (title/path): `06-policies-standards-procedures/procedures/04-metadata-registration-procedure.md` | Phase 8 |
| **Classify** | Data Owner **A**; Business Data Steward **R** | Apply Rafid Public / Internal / Confidential / Restricted `[A][B]` | Classification record (Phase 5 / Classification Standard and Procedure — not redesigned) | Phase 5, Phase 6 |
| **Assign Owner** | Already assigned **by domain** (Phase 4) — confirm on the asset | Confirm the eight locked Owner titles; Steward = **Business Data Steward** | Ownership on catalog / Lifecycle Registry | Phase 4 |
| **Store / Use** | Custodian implements approved handling; Data Owner **A** for meaning and in-policy access | Use within authorization; classification-aware handling | Access / quality / catalog status | Phase 4, 5, 7 |
| **Share where authorized** | Data Owner **A** business approval; PDPO **A** privacy review where personal data | Two **A**s remain separate. Restricted external: Requires Data Owner business approval + PDPO privacy compliance review where personal data is involved | Sharing record — Data Access / Sharing Governance Procedure: `06-policies-standards-procedures/procedures/05-data-access-sharing-governance-procedure.md` | Phase 4, 5, 6 |
| **Monitor** | Business Data Steward **R**; DMO oversight; Custodian technical | Quality, lineage impact, hold, lifecycle status | Quality issues (Phase 7 procedure by existing path); Lifecycle Registry | Phase 7, 9, this phase |
| **Retain** | Data Owner **A** for the rule; Business Data Steward **R**; DMO register | Apply Retention Schedule; period remains a verification placeholder until verified | Retention Rule / Retention Schedule | This phase; Phase 4 row 10 |
| **Archive when appropriate** | Data Owner **A**; Business Data Steward **R**; Custodian implements | Move to archived state — **not** backup | Archive Register | This phase; Phase 8 metadata |
| **Dispose when eligible** | Data Owner **A** authorize; Custodian execute; DMO close | Expiry verified; hold clear; evidence recorded | Disposal Record / Disposal Register | This phase |

**Assign Owner** does **not** create a ninth Owner. New assets inherit the **domain** Owner already locked in Phase 4.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Ten-stage E2E map | Sections 2–3 |
| `[C]` | Role **names** | Naming |
| `[NDMO verification required]` | Official NDMO lifecycle workflow | Not claimed |
| `[Legal / regulatory verification required]` | When dispose is legally permitted | Not invented |
