# PDPL Governance Considerations

**Document ID:** RHC-DG-P14-WP-002  
**Phase:** 14 — NDMO alignment (working pack)  
**Status:** Implemented (governance considerations only)

**Does not decide:** Legal interpretations, lawful bases, PDPL article application, or privacy-programme implementation

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

**Responsible:** DMO (governance design) · **Review:** PDPO; Legal Advisor · **Approval:** Not a legal approval. CDO accepts the file as a governance input only.

---

## 1. Purpose

Record how **PDPL** and related privacy themes are used as **regulatory inputs to Data Governance design** in this portfolio.

This is **not** legal advice.  
This is **not** a PDPL implementation.  
This is **not** a claim of PDPL compliance.

PDPL is named in the Phase 2 policy hierarchy as an example **L0** instrument (watchlist). Personal Data Protection is an NDMO domain **name** `[C]`. PDPO is an NDMO-named role `[C]`. Equivalence between PDPO and a PDPL DPO remains `[NDMO verification required]` / `[Legal / regulatory verification required]`.

No PDPL article numbers are copied in this repository. **None are invented here.**

---

## 2. How to read each row

| Column | Meaning |
| --- | --- |
| Governance Area | Rafid Data Governance capability |
| Why It Matters to Data Governance | Why the theme affects ownership, classification, access, quality, lifecycle, or evidence |
| Related Rafid Artifact | Existing file — not a new parallel control |
| Evidence State | Project evidence state (Designed / Operational / Measured) |
| Verification Status | Project verification language — never “compliant” |
| Notes | Limits and open items |

Wording used: **governance consideration** · **conceptual control consideration** · **requires legal / official verification**.

---

## 3. Considerations (11)

| Governance Area | Why It Matters to Data Governance | Related Rafid Artifact | Evidence State | Verification Status | Notes |
| --- | --- | --- | --- | --- | --- |
| Personal Data | Governance must know which assets are personal so classification, sharing, and catalog indicators are not treated as ordinary Internal data by default | Phase 8 recommended field **Contains personal data** (indicator only); Phase 5 classification process (PDPO **C** if personal); inventory rows in `08-metadata-catalog/working-pack/` | Designed for the field definition; Operational (project) where inventory rows exist | Conceptually aligned to Personal Data Protection domain **name** `[C]`; `[Legal / regulatory verification required]` for PDPL meaning | Indicator is not the personal data itself. No real personal data is used in this repository. |
| Data Classification | Handling strictness for identifiable health and workforce data is a classification decision (Data Owner **A**), not an IT default | `05-data-classification/02-classification-model.md`; `09-access-sharing-consequences.md` | Designed | Conceptually aligned to Data Classification domain **name** `[C]`; official national tier names `[NDMO verification required]`; PDPL overlay `[Legal / regulatory verification required]` | Rafid Restricted / Confidential are entity labels `[A][B]`. They are not PDPL legal classes. |
| Data Ownership | Accountability for meaning, quality, classification, and in-policy access must sit with a business Data Owner, including where data is personal | `04-ownership-stewardship/02-enterprise-ownership-matrix.md` | Designed | Conceptually aligned to Business Data Executive **name** `[C]`; duty-level and PDPL controller/processor mapping `[NDMO verification required]` / `[Legal / regulatory verification required]` | Eight Owner titles exist. Named appointments are not claimed. Do not treat IT/Custodian as Owner. |
| Access Governance | Access to personal data needs a recorded business decision plus a separate privacy review path where personal data applies | PRC-005 `05-data-access-sharing-governance-procedure.md` | Designed | Conceptually aligned to Sharing domain and PDPO **names** `[C]`; Sharing Regulation and PDPL access rules `[NDMO verification required]` / `[Legal / regulatory verification required]` | Two Accountable decisions remain separate. Conceptual control consideration only. |
| Data Lifecycle | Personal data should not remain in an unmanaged Create→Dispose path; lifecycle status belongs in governed records | `11-data-lifecycle/` principles and workflow | Designed | `[NDMO verification required]` / `[Legal / regulatory verification required]` for official lifecycle and PDPL retention/disposal overlay | Traceability principle is Rafid `[A][B]`. Not a PDPL disposal certification. |
| Retention considerations | Retention rules for personal data must not be invented “for convenience”; period fields stay empty until verified | `11-data-lifecycle/06-retention-governance.md` | Designed | Verification required — no periods in this repository | Purpose-driven retention is a **governance consideration**. PDPO **C** where personal; Legal **C** where legal risk. |
| Data Minimization considerations | Keeping more personal data than the approved purpose requires increases classification, access, and retention load | Lifecycle principle **Minimum necessary retention** (`11-data-lifecycle/02-lifecycle-principles.md`) | Designed | `[Legal / regulatory verification required]` for any PDPL minimization rule; `[NDMO verification required]` for NDMO specs | This is a conceptual control consideration using an existing lifecycle principle. It is not a copied PDPL article. |
| Purpose / use considerations | Sharing requests record purpose; retention starts from identified business purpose — purpose is a governance input to both | PRC-005 request step; lifecycle decision chain “Identify business purpose” | Designed | `[Legal / regulatory verification required]` for lawful-purpose tests; not designed as a legal-basis register | Catalog **Intended use** is recommended metadata, not a legal purpose record. |
| Data Sharing considerations | External or internal sharing of personal data is a dual-control governance event, not a single signature | PRC-005; Phase 4 sharing RACI; Restricted external wording locked in Policy | Designed | Sharing Regulation `[NDMO verification required]`; PDPL sharing overlay `[Legal / regulatory verification required]` | Locked wording: Requires Data Owner business approval + PDPO privacy compliance review where personal data is involved. “Privacy compliance review” is a Rafid process name, **not** a PDPL compliance claim. |
| Data Quality / accuracy considerations | Inaccurate personal identifiers (National ID, Patient ID) harm matching, care operations, and downstream claims — quality is a governance reliability consideration | Phase 7 dimensions (Accuracy, Completeness, Uniqueness); CDE-001 / CDE-002; practical-evidence sample | Designed (framework); illustrative sample only | Conceptually aligned to Data Quality domain **name** `[C]`; `[Legal / regulatory verification required]` for any PDPL accuracy duty; official DQ specs `[NDMO verification required]` | Sample issues are synthetic. Measured quality is not claimed. |
| Governance accountability | Privacy review, policy approval, and domain ownership must remain separable so one role cannot self-certify sharing, classification, and policy | Phase 3 role catalogue; DMC standing membership includes PDPO and Compliance Officer; POL-001 | Designed | PDPO / PDPL DPO equivalence `[NDMO verification required]` / `[Legal / regulatory verification required]` | No new roles. Requires legal / official verification before any statutory mapping. |

---

## 4. What this file does not do

- Does not claim “PDPL compliant”
- Does not create a Record of Processing, DPIA, consent register, or cross-border transfer file
- Does not interpret controller, processor, or data-subject rights
- Does not replace NCA security controls
- Does not use real personal data

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Personal Data Protection domain **name**; PDPO **name** | Domain / role pointers |
| `[A][B]` | Rafid dual-A sharing, classification, lifecycle principles, metadata indicator | Considerations |
| `[Legal / regulatory verification required]` | PDPL overlay (articles not in project sources) | Every legal-meaning cell |
| `[NDMO verification required]` | Personal Data Protection specifications not copied | Domain specs |
