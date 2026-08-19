# Interview Defensibility — Ownership and Stewardship

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P4-009  
**Phase:** 4 — Ownership and stewardship  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Why isn’t IT the Data Owner?

IT is the **Custodian** (NDMO name: IT Data Steward `[C]`). Custodians implement systems, interfaces, and provisioning. They do not own **business meaning** or **quality** of clinical, identity, or finance data `[B]`. If IT were Owner, every definition dispute would become an EMR ticket, and clinicians would disengage. Phase 3 already forbade IT as Accountable for business ownership; Phase 4 assigns **zero** domains to CIO/Custodian.

---

## Why is ownership enterprise-wide, not hospital-by-hospital?

Rafid is modeled with a **cluster-wide EMR** and patients who move across four hospitals and PHCs `[A]`. Phase 3 federated **by domain**, not by facility `[B]`. Hospital-level Owners would recreate duplicate identity and conflicting definitions. One Patient/Person Owner covers the cluster; facility staff may **support** the steward, they do not become a second Accountable Owner.

---

## Why isn’t the CMO Owner of all patient data?

“Patient data” is not one domain. **Who the person is** (identity master) is owned by the **Patient Access & Experience Director**. **What was documented in the medical record** is owned by the **CMO**. Mixing them would make Medical Affairs responsible for registration data they do not run, and would hide identity-quality failures inside “clinical governance.” The CMO is **Consulted** on identity rules that affect safety, not a second Owner.

---

## How is shared ownership handled?

**It is not used.** Phase 4 forbids two Accountable Owners. Where two executives had a claim (for example CMO vs Medical Affairs on provider data), **one A** was chosen (Medical Affairs Officer for Provider/Clinician Data) and the other remains **C**. For sharing, **two rows** split business approval (Owner **A**) from privacy review (PDPO **A**) so there is never dual-A on one activity.

---

## Data Owner vs Data Steward?

| | Data Owner | Business Data Steward |
| --- | --- | --- |
| NDMO name `[C]` | Business Data Executive | Business Data Steward |
| RACI | **A** on meaning, quality, in-policy access, business sharing, classification application, catalog content, issues, retention | **R** on those rows (executes) |
| Does not | Write L3 policy; run EMR platforms as Owner | Approve out-of-policy access; act as PDPO |

Owner **answers** if the domain’s data is wrong. Steward **does the work** to keep it right, under the Owner.

---

## Who is accountable if data quality is poor?

The **Data Owner** of that domain is **Accountable**. The Steward is **Responsible** for rules monitoring and issue investigation. The Custodian is **Responsible** for technical fixes. DMO **coordinates**. IT is **not** Accountable for business quality. Example: duplicate patients → Patient Access & Experience Director **A**, not CIO and not CMO (CMO is consulted if clinical harm is in play).

---

## Short facts to have ready

- Eight domains, eight Owners, no IT Owner `[A]` / `[B]`
- No numeric steward SLA `[B]`
- Year-1 DMC standing members include three domain Owners (Patient, Clinical, Financial) plus CEO, CDO, CIO, PDPO, Compliance Officer `[A]`
- Control-level NDMO IDs were not used; role **names** are `[C]`

---

## Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Owner titles and DMC composition | Examples |
| `[B]` | Ownership principles; federated-by-domain | Arguments |
| `[C]` | NDMO role names | Owner vs steward vs custodian labels |
| `[NDMO verification required]` | Specification-level “must assign X” | Not claimed |
