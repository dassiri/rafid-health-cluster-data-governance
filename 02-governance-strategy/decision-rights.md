# Decision Rights

**Document ID:** RHC-DG-P2-002  
**Phase:** 2 — Governance Design Boundaries  
**Status:** Documented at **decision-class** level only  
**Does not decide:** RACI, committee charter, reporting lines, or named incumbents

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This document defines **classes of data decisions** and the **role names NDMO requires entities to identify**, so Phase 3 (operating model) has a stable vocabulary.

It is **not** an operating model. It does **not** assign who is Accountable/Responsible for each process. That is Phase 3–4 `[B]`.

NDMO control `DG.4` (Data Management Organization) requires the entity to establish a Data Management Office and a Data Management Committee, and to identify and appoint specified roles `[C]` (NDMO Standards v1.5). Job-content alignment is to NDMO’s **Organizational Manual** `[C]` pointer. That manual was **not retrieved** for this drop, so duty-level statements are `[NDMO verification required]`.

---

## 2. Decision classes `[B]`

Industry practice groups data decisions by altitude. Rafid uses three classes `[B]`. Class names are not NDMO control IDs.

| Class | Meaning | Examples (illustrative, not a backlog) | Typical altitude |
| --- | --- | --- | --- |
| **Strategic** | Direction, policy intent, investment envelope, risk appetite for data | Approve strategy; adopt principles; accept residual risk on a sharing model | Executive / committee |
| **Tactical** | Standards, domain rules, prioritization of data products and issues | Approve a data standard; set classification process (when designed); prioritize MDM objects | Data office / domain executives |
| **Operational** | Day-to-day application of rules | Classify a dataset (when process exists); raise a data issue; grant access within policy | Stewards and system operators |

Phase 2 **does not** map each example to a person.

---

## 3. NDMO-named organizational elements `[C]`

The following names are from NDMO Standards v1.5, `DG.4`. They are recorded so later design does not invent parallel titles without mapping.

**Structures**

| Element | NDMO specification (ID) | What NDMO states (summary) | Rafid Phase 2 position |
| --- | --- | --- | --- |
| Data Management Office | `DG.4.1` | Establish an office to manage achievement of national data management agendas at entity level; responsibilities aligned to NDMO Organizational Manual | **Named as required later**; not stood up |
| Entity Data Management Committee | `DG.4.2` | Establish a committee for direction and oversight; responsibilities aligned to Organizational Manual | **Named as required later**; not chartered |

**Roles NDMO says the entity shall identify and appoint** (`DG.4.3`–`DG.4.11`) `[C]`:

| Role (NDMO name) | Spec ID | Phase 2 position |
| --- | --- | --- |
| Chief Data Officer (CDO) | `DG.4.3` | Required later; not appointed in this repo |
| Data Governance Officer | `DG.4.4` | Required later; not appointed |
| Open Data and Information Access Officer (ODIA) | `DG.4.5` | Required later; healthcare applicability of ODIA operating model `[NDMO verification required]` |
| Compliance Officer (data management agenda) | `DG.4.6` | Required later; relationship to internal audit `[NDMO verification required]` |
| Personal Data Protection Officer (PDPO) | `DG.4.7` | Required later; relationship to PDPL DPO concept `[NDMO verification required]` |
| Business Data Executive (BDE) | `DG.4.8` | Required later; domain assignment is Phase 4 |
| Business Data Steward | `DG.4.9` | Required later |
| IT Data Steward | `DG.4.10` | Required later |
| Legal Advisor (data-related regulatory matters) | `DG.4.11` | Required later |

NDMO also states that the annual compliance exercise shall be led by the Chief Data Officer, supported by other Data Management and Personal Data Protection Office roles `[C]` (Standards, Compliance and Enforcement). Rafid has not run that exercise.

---

## 4. Decision-rights rules for Phase 2 (boundary rules, not a RACI) `[B]` / `[A]`

These rules constrain later design. They are program rules, not NDMO specifications.

1. **Do not invent a second set of executive titles** that silently replace NDMO `DG.4` names. If Rafid uses a local title, Phase 3 must map it to the NDMO name `[A]` / `[C]`.
2. **Strategic class** decisions wait for a committee or equivalent executive body. Phase 3 will propose that body against `DG.4.2` `[C]`.
3. **Tactical class** decisions wait for a Data Management Office or equivalent. Phase 3 will propose that office against `DG.4.1` `[C]`.
4. **Operational class** decisions wait for steward appointments (`DG.4.9`, `DG.4.10`) `[C]`.
5. **Security control decisions** remain coordinated with NCA-aligned cybersecurity (Domain 15) `[C]`. Governance does not “own NCA.”
6. **No person in this repository is appointed.** Names of fictional incumbents are out of scope `[A]`.

---

## 5. Decision types to be allocated later (backlog for Phase 3–4) `[B]`

Listed so they are not forgotten. **Not allocated now.**

- Approve / change enterprise data policy.
- Approve exceptions to policy.
- Accept classification (when process exists).
- Accept a system as system-of-record.
- Approve external data sharing.
- Accept a data-quality threshold.
- Close a data issue.
- Approve open-data release.
- Approve FOI disclosure or denial (if applicable).
- Approve vendor processing of cluster data.

Sharing, FOI, and open-data **procedures** are defined in NDMO domains 9, 11, and 12 and in regulations the Standards point to `[C]` + `[NDMO verification required]` for regulation text.

---

## 6. What must not be inferred from this file

- That Rafid has a CDO, DMO, or committee.
- That a RACI exists.
- That `DG.4` is implemented.
- That ODIA/FOI operating models for hospitals have been designed.

---

## 7. Intentionally unresolved

- Reporting line of the CDO.
- Whether PDPO and a PDPL “controller/processor” model are the same seat.
- How many BDEs exist (by clinical vs. corporate domain).
- Voting rules of the Data Management Committee.
- Full text of NDMO Organizational Manual duties `[NDMO verification required]`.

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5, `DG.4.1`–`DG.4.11`; Compliance and Enforcement (CDO-led annual assessment); Domain 15 NCA note | Role and structure names |
| `[B]` | Strategic / tactical / operational decision classes | Section 2 |
| `[A]` | Rafid program rules | Section 4 |
