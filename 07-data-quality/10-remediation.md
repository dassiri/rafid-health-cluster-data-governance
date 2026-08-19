# Remediation

**Document ID:** RHC-DG-P7-010  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Data Owner **A** (accept residual or require fix); Steward **R**; Custodian technical implementation  
**Approver:** CDO `[B]` (method)  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic with STD-003 `[B]` (no numeric SLA)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Eight approved approaches; source correction preferred where practical.

**Phase:** 7 — Data quality  
**Does not decide:** Specific code fixes; MDM survivorship; catalog tooling

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document records approved **remediation approaches** for data quality issues `[A][B]`.

Correcting the **source** is preferred where practical `[B]`. Downstream-only patches that leave the source wrong are a last resort and must be visible on the issue record.

---

## 2. Approved approaches (locked) `[A][B]`

| # | Approach | Typical when |
| --- | --- | --- |
| 1 | **Correct the record** | A specific instance is wrong and can be safely corrected in place. |
| 2 | **Correct the source** | The originating system or process will keep producing the defect unless changed. **Preferred where practical.** |
| 3 | **Fix transformation logic** | The source is right; mapping/derivation is wrong. |
| 4 | **Improve validation** | Prevention at entry or interface is feasible. |
| 5 | **Update reference data** | The code list or master value is the cause (CDE-013 and similar). |
| 6 | **Process change** | The workflow allows the defect. |
| 7 | **Training** | Execution knowledge is the gap (see RCA category User training). |
| 8 | **Policy/governance change** | Definition, rule, exception, or ownership is the gap. Policy change is **DMC A** if it changes POL-001 intent. |

More than one approach may apply. Record the **primary** approach.

---

## 3. Source-first principle `[B]`

| Prefer | Avoid as the only fix |
| --- | --- |
| Fix registration so National ID is captured correctly (CDE-001) | Nightly script that patches the warehouse while MPI stays wrong |
| Fix credentialing status so expiry is visible (CDE-006) | Manual spreadsheet that IT re-keys after the fact |
| Fix item master so invalid codes cannot be chosen (CDE-010) | Finance “mapping table” that hides invalid codes |

Where source correction is **not** practical in the current lifecycle stage, the Owner **A** documents residual risk. That is not a silent workaround. Out-of-policy residual may require the Data Governance Exception Procedure (**DMC = A**).

Phase 10 matching/survivorship is **not** a Phase 7 remediation design. Duplicate **governance** still uses the issue path under the Patient/Person or Provider Owner.

---

## 4. Who does the work (Phase 4 — not redesigned)

| Role | Remediation |
| --- | --- |
| Data Owner | **A** for business outcome and residual acceptance |
| Business Data Steward | **R** for coordinating the business fix and verification |
| IT Data Steward / Custodian | Technical remediation in systems |
| DMO | Coordinates cross-domain; does not own the business fix |
| PDPO | **C** if the fix itself has privacy implications (for example identity merge) |

---

## 5. Verification before close

Remediation is not complete until the Steward **verifies** (Phase 6 Verify) that the defect no longer reproduces **or** the Owner-accepted residual is documented. Close remains Owner **A**.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Eight approaches; source-first | Sections 2–3 |
| `[C]` | Data Quality domain **name** | Context |
| `[NDMO verification required]` | Official NDMO remediation mandates | Not claimed |
