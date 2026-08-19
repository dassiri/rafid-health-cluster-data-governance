# Ownership Decision Matrix

**Document ID:** RHC-DG-P4-003  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented  
**Does not decide:** Phase 5 classification labels or Phase 6 policy text

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This matrix assigns **RACI** for the ten approved **ownership decisions** at domain level `[B]`. It uses role **types**, not people. The same matrix applies to all eight domains unless a row says otherwise (privacy review applies where personal data is in play).

**R** = Responsible (does the work)  
**A** = Accountable (**exactly one** per row)  
**C** = Consulted  
**I** = Informed  

IT / Custodian is never **A** for business meaning, quality, in-policy access, business sharing, definitions, classification application, metadata content, issue closure, or retention **business** decision.

---

## 2. Role columns

| Code | Role type |
| --- | --- |
| DO | Data Owner (Business Data Executive `[C]` name) |
| BDS | Business Data Steward `[C]` name |
| CUST | Data Custodian / IT Data Steward `[C]` name |
| DMO | Data Management Office (CDO / Data Governance Officer) `[C]` names |
| PDPO | Personal Data Protection Officer `[C]` name |
| DMC | Data Management Committee `[C]` name |

---

## 3. Decision RACI `[B]`

The two **Data sharing** rows are **separate**. They must not be merged.

| # | Decision | DO | BDS | CUST | DMO | PDPO | DMC |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Data definition | **A** | **R** | C | C | C* | I |
| 2 | Data quality rules | **A** | **R** | C | C | I | I |
| 3 | Data classification | **A** | **R** | C | C | C | I |
| 4 | Access approval (in-policy) | **A** | **R** | **R** | I | C | I |
| 5 | Access approval (exception) | C | **R** | C | **R** | C | **A** |
| 6 | Data sharing — business approval | **A** | **R** | C/I | C | C/I | I |
| 7 | Data sharing — privacy compliance review (personal data) | C | C | I | C | **A** | I |
| 8 | Metadata/catalog approval | **A** | **R** | C | C | C | I |
| 9 | Data issue resolution | **A** | **R** | **R** | C | I | I |
| 10 | Retention/lifecycle decision | **A** | **R** | **R** | C | C | I |

\* PDPO is **C** on definitions when the definition is personal or health-identifying. Otherwise **I**.

### Notes

- **Row 3** is Accountable for **applying** classification to domain datasets once a method exists. The classification **method/standard** remains a Phase 3 policy item (**A = DMC**). No dataset is classified in Phase 4 (Phase 5 is Designed / Documented; operational implementation and measured performance are not claimed).
- **Row 5** follows Phase 3: exceptions to policy-level access sit with the Data Management Committee (**A = DMC**). The Owner does not self-approve out-of-policy access.
- **Row 6** **A = Data Owner**. Custodian is **C** when technical delivery of the share must be assessed, otherwise **I**. PDPO is **C** when the share may involve personal data (and is **I** when it clearly does not). This is **business approval**, not a privacy determination.
- **Row 7** **A = PDPO**. This is the privacy compliance review for personal data. It is not a second business-approval Accountable. NDMO names the PDPO `[C]`; PDPL mapping is `[NDMO verification required]`.
- **Row 8** is domain **content** approval (definitions, catalog entries for the domain). The enterprise catalog **programme** remains CDO-Accountable in the Phase 3 enterprise RACI. DMO is **C** here to check the standard; DMO is not Owner of domain meaning.
- **Row 6** aligns with NDMO describing Business Data Executive involvement in sharing `[C]`. Regulation-level sharing steps remain `[NDMO verification required]`.

---

## 4. Single-A confirmation

Each of the ten rows has exactly one **A**:

| Row | Single A |
| --- | --- |
| 1–4, 6, 8–10 | Data Owner |
| 5 | Data Management Committee |
| 7 | PDPO |

No row has two Accountable roles.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 4 decision rows and RACI; Phase 3 exception path | Matrix |
| `[C]` | NDMO role **names**; BDE in sharing process as stated in Standards v1.5 | Why Owner is A on business sharing |
| `[NDMO verification required]` | Sharing regulation; PDPL operationalization; classification regulation | Not designed here |
