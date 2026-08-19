# Illustrative Classification Examples

**Document ID:** RHC-DG-P5-010  
**Phase:** 5 — Data classification  
**Status:** Implemented (illustrative only)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

These examples are **fictional** `[A]` and illustrate **dataset-level** application of Rafid tiers `[A][B]`. They are **not**:

- A live Rafid inventory
- Blanket domain rules
- NDMO national-tier assignments `[NDMO verification required]`

Each row still needs Owner approval in a real process. Typical domain patterns: [`04-domain-application.md`](04-domain-application.md).

---

## 2. Approved examples `[A]`

| Illustrative dataset `[A]` | Illustrative Rafid tier `[A][B]` | Notes |
| --- | --- | --- |
| Patient demographic record | **Restricted** | Identifiable person master; typical of Patient/Person domain — still a **dataset** decision |
| De-identified clinical record | **Confidential** | Lower than a fully identifiable medical record **if** de-identification is accepted by the Owner with PDPO consult; not automatically Public |
| Provider credential record | **Confidential** | Typical of Provider/Clinician domain |
| Financial claim containing patient/clinical/financial information | **Restricted** | Combined impact → **highest** applicable; Confidential–Restricted domain range resolves **up** because identifiers + clinical + financial are present |
| Employee payroll record | **Confidential** | Typical of HR/Workforce domain |
| Medical inventory | **Internal** | Typical of Supply Chain & Asset domain unless the file is patient-linked |
| Patient safety incident | **Restricted** | Typical of Quality & Patient Safety domain when patient-linked |
| Facility hierarchy / org chart | **Internal**, potentially **Public** if deliberately published | Typical of Reference/Organizational Master Data; Public only with Owner-approved release |

---

## 3. What the examples teach `[B]`

- Healthcare data is **not** automatically Restricted (de-identified clinical record; medical inventory; org chart).
- One domain can contain more than one tier (clinical identifiable vs de-identified).
- Combination raises impact (the claim example).
- Public requires a **deliberate** decision, not absence of a label.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Phase 5 example list | Section 2 |
| `[B]` | Dataset-level and highest-impact rules | Section 3 |
| `[C]` | PDPO **name** (consult on de-identification / personal data) | Notes column |
| `[NDMO verification required]` | National names for these examples | Not applied |
