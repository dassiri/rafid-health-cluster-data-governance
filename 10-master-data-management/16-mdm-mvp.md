# MDM MVP

**Document ID:** RHC-DG-P10-016  
**Version:** 1.0  
**Status:** Implemented (MVP design only — not a live hub)  
**Owner:** CDO / DMO (programme) `[B]`; Core MDM Owners **A** for content  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Patient and Provider primary; Facility lightweight supporting only.

**Phase:** 10 — Master data management  
**Does not decide:** Vendor; numeric duplicate rates; a third full MDM workstream

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Scope (locked)

**PRIMARY**

1. Patient / Person Master  
2. Provider / Clinician Master  

**SUPPORTING**

3. Facility / Organization Master  

**Facility / Organization is ONLY lightweight supporting scope.**  
It is **NOT** a third full MDM workstream.

Supporting scope **may** include:

- Facility-code consistency  
- Basic reference alignment  
- Relationship context for Patient and Provider  

**Do NOT build a separate Facility matching/survivorship/golden-record program.**

---

## 2. Master entities and minimum attributes `[A]` illustrative

| Entity | Owner | Minimum attributes (illustrative, not a physical schema) |
| --- | --- | --- |
| Patient / Person | Patient Access & Experience Director | Patient identifier; National ID where applicable; name; date of birth |
| Provider / Clinician | Medical Affairs Officer | Provider identifier; name; licence/expiry |
| Facility / Organization (supporting) | Strategy & Planning Director | Facility / department code; name |

Steward: **Business Data Steward**.

---

## 3. Matching approach (MVP)

Patient and Provider: deterministic considerations + **manual review**; probabilistic/fuzzy **conceptual only**. **No** algorithms. **No** numeric thresholds.

Facility: **code consistency** against org reference — **not** a matcher program.

---

## 4. Survivorship approach (MVP)

Per-domain, per-attribute rules set by Owner and Steward. **No** universal system ranking. Facility: prefer org-reference **codes** for alignment — still not a Facility golden-record program.

---

## 5. Quality controls

Reuse Phase 7: uniqueness of Patient and Provider identifiers; integrity of facility codes (DQ-008) as **supporting** reference quality. Issue path unchanged.

---

## 6. Governance workflow

Use the MDM entity lifecycle ([`13-master-data-lifecycle.md`](13-master-data-lifecycle.md)): Owner approves definition/domain rules; DMC escalation only within existing Phase 3 authority.

No new Standard or Procedure.

---

## 7. Qualitative success indicators `[A][B]`

- Patient and Provider identities have Owner-accepted definitions  
- Duplicate candidates can be logged and reviewed without a match engine  
- Facility codes used on Patient/Provider context are alignable to Domain 8 lists  
- Catalog can hold Master Data Entity records for the two primary masters  
- **No MDM product** is required to declare the MVP **design** complete  

Do **not** create numeric production targets. (None are set. Any future number would need `[A] Illustrative`.)

---

## 8. Why this cut

Patient and Provider are the shared identities on the Phase 9 illustrative care-to-claim chain. Facility is **context**, not a third identity factory. HR, Finance transactions, and Quality remain Non-MDM at this maturity.

---

## 9. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved MVP cut | Sections 1–8 |
| `[C]` | MDM domain **name** | Context |
| `[NDMO verification required]` | Official NDMO MDM rollout metrics | Not claimed |
