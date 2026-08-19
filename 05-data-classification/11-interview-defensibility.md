# Interview Defensibility — Data Classification

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P5-011  
**Phase:** 5 — Data classification  
**Audience:** Candidate using this repository in a Data Governance interview

**This file is not organizational policy.**  
**This file is not an NDMO submission.**  
**This file does not claim compliance.**

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## Classification vs sensitivity

**Sensitivity** is a loose description of how much harm might follow from mishandling (Phase 0 landscape notes were informal). **Classification** is an **approved Rafid tier** on a **dataset**, with an Owner, a rationale, and consequences for access and sharing `[B]`. Informal “high/medium” labels are not classification.

Rafid tiers are Public, Internal, Confidential, Restricted `[A][B]`. They are **not** NDMO’s official names `[NDMO verification required]`.

---

## Who decides classification?

The **Data Owner** is Accountable and **approves** initial classification and reclassification. The **Steward** proposes and records. **IT/Custodian implements and does not decide.** DMO owns methodology and the registry. PDPO reviews privacy implications for personal data. Compliance Officer audits the process.

---

## Multiple classifications within one domain?

**Yes.** Classification is **dataset-level**, not domain-level. Domain rows are **typical guidance** only. Example: Clinical / Medical Records is typically Restricted, but a de-identified clinical record may be Confidential if the Owner approves `[A]`.

---

## Why isn’t healthcare data automatically Restricted?

Not every healthcare-related file has the same impact. Medical inventory can be Internal. An org chart can be Internal or Public if published. A de-identified extract can be Confidential rather than Restricted. Automatic Restricted would ignore Open-by-Default constraints that still require a **justified** non-public decision `[C]` principle name, and would hide real Restricted datasets in noise `[B]`.

---

## Combining datasets?

Use **highest applicable impact**. A financial claim that **contains** patient and clinical information is Restricted in the approved example `[A]`, even though finance as a domain is described as Confidential–Restricted **typical** guidance.

---

## Reclassification?

Triggered by sensitivity change, new regulation, new use case, linkage, security incident, organizational change, transformation, or sharing-context change. **Only the Data Owner approves the classification change.** Downward moves need an explicit rationale (not “we aggregated it”).

---

## Relationship between classification and Data Governance?

Classification is a **Data Governance decision** (authority, Owner, process, registry, consequences). It is **not** only a security labelling exercise. Cybersecurity implements handling and remains coordinated with NCA for NDMO’s security domain `[C]`. Governance does not replace NCA. Sharing still uses Phase 4’s two rows; Restricted external sharing uses the exact sentence in [`09-access-sharing-consequences.md`](09-access-sharing-consequences.md).

---

## NDMO names in interviews

Do **not** resolve Top Secret / Secret / Restricted / Public versus Top Secret / Secret / Confidential / Public. Both remain `[NDMO verification required]`. Do **not** say Rafid’s four labels are NDMO’s four labels. NDMO has a Data Classification domain and a four-level **concept** `[C]`.

---

## Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 5 Q&A and Rafid scheme | All answers |
| `[C]` | Domain names; Open by Default principle **name**; NCA mandate | Limits of the answers |
| `[NDMO verification required]` | Official NDMO tier names | Unresolved |
