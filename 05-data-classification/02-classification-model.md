# Rafid Classification Model

**Document ID:** RHC-DG-P5-002  
**Phase:** 5 — Data classification  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **Rafid’s proposed enterprise classification scheme** for the fictional cluster `[A]`. The scheme is an industry-style four-tier model `[B]`.

**This is not NDMO’s official classification scheme.**  
Official NDMO tier names remain unresolved `[NDMO verification required]`. See [`01-ndmo-baseline.md`](01-ndmo-baseline.md).

NDMO’s Data Classification **domain name** is `[C]`. That does not make these four Rafid labels national labels.

---

## 2. The four Rafid tiers `[A][B]`

Exactly four working labels. Do not add a fifth.

| Order (increasing handling strictness) | Rafid tier `[A][B]` | Working meaning (Rafid, not NDMO) |
| --- | --- | --- |
| 1 | **Public** | Intended or eligible for general availability after a deliberate release decision. Not “everything unmarked.” |
| 2 | **Internal** | For cluster workforce use in ordinary operations; not for general public release. |
| 3 | **Confidential** | Limited to defined roles; compromise would cause significant privacy, operational, financial, or reputational harm. |
| 4 | **Restricted** | Strict need-to-know; compromise could cause serious privacy, patient-safety, legal, or similarly severe harm. |

These **definitions are Rafid working definitions** `[A][B]`. They are **not** official NDMO definitions.

---

## 3. What the labels are not

| Do not say | Correct statement |
| --- | --- |
| “Rafid Restricted = NDMO Top Secret / Secret / Restricted / Confidential” | No equivalence is declared `[NDMO verification required]` for national names |
| “Internal is an NDMO tier” | Internal is a **Rafid** label `[A][B]` |
| “Four tiers means we copied NDMO’s four names” | NDMO has a four-level **concept** `[C]`; **names** are unverified and conflict |
| “Domain X is Restricted, therefore every dataset in X is Restricted” | Classification is **dataset-level** `[B]` |

---

## 4. Relationship to handling

Tier assignment is a **business classification decision** (Data Owner **A**). Technical handling is implemented by Custodians with cybersecurity coordination. Domain 15 remains under NCA `[C]`. This file does not specify encryption or tools.

Access and sharing consequences: [`09-access-sharing-consequences.md`](09-access-sharing-consequences.md).

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Approved Phase 5 Rafid model | Four tiers and working meanings |
| `[C]` | NDMO Data Classification domain **name**; NCA mandate for security domain | Context only |
| `[NDMO verification required]` | Official NDMO tier names and definitions | Explicit non-equivalence |
