# Domain Application (Typical Guidance)

**Document ID:** RHC-DG-P5-004  
**Phase:** 5 — Data classification  
**Status:** Implemented  
**Does not decide:** Classification of any specific live dataset

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Principle

The table below is **typical domain-level guidance** `[A][B]`. It is **not** a blanket rule.

Classification remains **dataset-level**. A dataset in a “typically Restricted” domain may be Internal or Public if impact supports it (for example a deliberately published org chart). A dataset in a “typically Internal” domain may be Restricted if it is linked to identifiable patient or safety data.

Owners and Stewards are the Phase 4 titles `[A]`. IT is never the classification decision-maker.

Rafid tiers used here are `[A][B]`, not NDMO national tiers `[NDMO verification required]`.

---

## 2. Typical patterns by domain

| Domain | Typical Rafid tier `[A][B]` | Data Owner (Phase 4) | Why this is only “typical” |
| --- | --- | --- | --- |
| Patient / Person Master Data | **Restricted** | Patient Access & Experience Director | Identity data is usually high privacy and safety impact; a non-identifying statistical count extract could be lower if Owner-approved |
| Clinical / Medical Records Data | **Restricted** | Chief Medical Officer (CMO) | Care documentation is usually high privacy and safety impact; a de-identified teaching set may be lower if Owner-approved with PDPO consult |
| Provider / Clinician Data | **Confidential** | Medical Affairs Officer | Credentials and practitioner masters are limited-role; public-facing consultant directories, if deliberately published, may be Public |
| Financial / Billing & Claims Data | **Confidential–Restricted** | Chief Financial Officer (CFO) | Range, not a single stamp: claims **with** patient/clinical identifiers typically **Restricted**; some finance operational files may be **Confidential** |
| HR / Workforce Data | **Confidential** | HR Director | Payroll and employee personal data are typically Confidential; a public vacancy notice may be Public |
| Supply Chain & Asset Data | **Internal** | Supply Chain Director | Ordinary inventory is typically Internal; files linking assets to named patients or high-risk security layouts may be higher |
| Quality & Patient Safety Data | **Restricted** | Chief Quality & Patient Safety Officer (CQPSO) | Incident and safety files are often patient-linked; de-identified indicator packs may be lower if Owner-approved |
| Reference / Organizational Master Data | **Internal** | Strategy & Planning Director | Facility hierarchy is typically Internal; **potentially Public if deliberately published** |

---

## 3. Exceptions (must be dataset-specific)

Examples of exceptions **not** decided here — they require Owner approval using [`03-classification-criteria.md`](03-classification-criteria.md):

- De-identified or aggregated extracts
- Deliberate Public publication (org chart, public waiting-time report)
- Combined extracts (claim + clinical + identity → treat with **highest** impact; often Restricted)
- Shadow copies on shares (still classified as datasets; copies do not inherit a weaker tier automatically)

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Approved Phase 5 typical tiers; Phase 4 Owner titles | Table |
| `[B]` | Dataset-level principle; typical vs blanket | Section 1 |
| `[C]` | PDPO/personal-data **names** (consult when personal) | Exception handling |
| `[NDMO verification required]` | National tier equivalence | Not claimed |
