# Master Data Domain Assessment

**Document ID:** RHC-DG-P10-003  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (assessment method); Data Owners **A** for their domains  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-005 `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Core / Reference / Non-MDM at this maturity; no new Owners.

**Phase:** 10 — Master data management  
**Does not decide:** Future promotion of HR or Finance into Core MDM

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document **evaluates** the eight Phase 4 domains as MDM context. It does **not** automatically declare all eight to be MDM domains. It does **not** introduce new Data Owner titles.

---

## 2. Classification at this maturity (locked) `[A][B]`

### CORE MDM (exactly three)

| Domain / master | Data Owner (Phase 4) | Why Core |
| --- | --- | --- |
| **Patient / Person Master** | Patient Access & Experience Director | Shared identity across care, billing, quality |
| **Provider / Clinician Master** | Medical Affairs Officer | Shared practitioner identity across EMR, credentialing, roster joins |
| **Facility / Organization Master** | Strategy & Planning Director | Shared location/org identity; **MVP supporting only** ([`16-mdm-mvp.md`](16-mdm-mvp.md)) |

### REFERENCE DATA / GOVERNED REFERENCE

| Domain / set | Data Owner (Phase 4) | Treatment |
| --- | --- | --- |
| **Supply Chain / Item-type** reference data | Supply Chain Director | Governed **reference**, not Core MDM |
| Other controlled code sets (diagnosis, claim status, gender, country, encounter type) | Owner of the **consuming or list-owning** domain per Phase 4 (e.g. diagnosis lists under Clinical Owner for clinical meaning) | Governed reference ([`12-reference-data-management.md`](12-reference-data-management.md)) |

### NON-MDM AT THIS MATURITY

| Domain | Data Owner (Phase 4) | Why not Core MDM now |
| --- | --- | --- |
| **HR / Workforce** | HR Director | Workforce records are important; Year-1 Core MDM is Patient and Provider. HR remains **non-MDM at this maturity** (roster–provider join is a **consistency** issue, not a fourth master program) |
| **Financial / Billing & Claims** | CFO | Claims/payments are **transactions** |
| **Quality & Patient Safety** | CQPSO | Incidents/indicators are **transactional / derived**, not a shared identity master |

---

## 3. Reference / Organizational Master vs Facility / Organization Master

Phase 4 Domain 8 (**Reference / Organizational Master Data**) is owned by **Strategy & Planning Director**. Facility / Organization Master **uses** that domain’s reference structures.

This relationship does **not** create an additional full MDM workstream. Domain 8 stewardship (analyst hosted in DMO) remains Phase 4: DMO **hosts** the Steward; DMO is **not** Owner. In Phase 10 examples the Steward role is labeled **Business Data Steward** only.

---

## 4. Clinical / Medical Records

Not a Core MDM domain. Encounters and diagnoses are **transaction / clinical content** (CMO). They **consume** Patient and Provider masters.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Core / Reference / Non-MDM cut | Section 2 |
| `[C]` | Role **names**; MDM domain **name** | Context |
| `[NDMO verification required]` | Official NDMO master-domain list | Not claimed |
