# Retention Schedule

**Document ID:** RHC-DG-P11-007  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]` (schedule method); Data Owner **A** for each rule in the domain  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Schedule structure; period fields are verification placeholders.

**Phase:** 11 — Data lifecycle  
**Does not decide:** Any numeric retention period

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. Purpose

This document records a **conceptual Retention Schedule** `[A][B]`.

It is `[A]` Proposed Rafid governance artifact (see [20](20-governance-artifacts.md)). **Not** claimed as NDMO-mandated.

**Do not populate invented retention numbers.** Where the actual requirement has not been verified, use `[NDMO verification required]` or `[Legal / regulatory verification required]`.

---

## 2. Minimum fields (locked)

| Field | Intent |
| --- | --- |
| **Retention Rule ID** | Unique identifier for the rule |
| **Data Domain** | One of the eight Phase 4 domains |
| **Data Asset / Record Type** | Catalog-aligned name (Phase 8) |
| **Business Purpose** | Why the data is kept |
| **Owner** | Exact Phase 4 Data Owner title |
| **Classification** | Rafid Public / Internal / Confidential / Restricted `[A][B]` — **handling**, not duration |
| **Retention Trigger** | Event that starts the clock |
| **Retention Period** | Verified duration after trigger — **placeholder until verified** |
| **Legal / Regulatory Basis** | Cited source when verified — otherwise a verification placeholder |
| **Legal Hold Status** | Whether a hold currently applies (see [08](08-legal-regulatory-hold.md)) |
| **Archive Requirement** | Whether archive is expected before disposal (conceptual) |
| **Disposal Method** | Conceptual method class (see [10](10-disposal-destruction.md)) — not a product |
| **Approval** | Data Owner **A** (Phase 4 row 10) |
| **Effective Date** | When the approved rule takes effect |
| **Review Date** | When the rule is next reviewed |

---

## 3. Illustrative rows `[A]` — periods not invented

The following rows show **structure only**. They are **not** a live schedule and **not** legal advice.

| Retention Rule ID | Data Domain | Data Asset / Record Type | Business Purpose | Owner | Classification | Retention Trigger | Retention Period | Legal / Regulatory Basis | Legal Hold Status | Archive Requirement | Disposal Method | Approval | Effective Date | Review Date |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| RR-ILL-001 `[A]` | Patient / Person Master | Patient demographic dataset (illustrative) | Identity and access for care | Patient Access & Experience Director | Restricted `[A][B]` | Patient relationship end `[A]` illustrative | `[Legal / regulatory verification required]` / `[NDMO verification required]` | `[Legal / regulatory verification required]` | None recorded | To be confirmed after verification | Conceptual — appropriate to Restricted and media | Data Owner **A** when period is verified | Not live `[A]` | Periodic `[B]` |
| RR-ILL-002 `[A]` | Clinical / Medical Records | Encounter documentation (illustrative) | Clinical care and record of treatment | Chief Medical Officer (CMO) | Restricted `[A][B]` | Record completion `[A]` illustrative | `[Legal / regulatory verification required]` / `[NDMO verification required]` | `[Legal / regulatory verification required]` | None recorded | To be confirmed after verification | Conceptual — appropriate to Restricted and media | Data Owner **A** when period is verified | Not live `[A]` | Periodic `[B]` |
| RR-ILL-003 `[A]` | Financial / Billing & Claims | Claim record (illustrative) | Billing, claims, financial accountability | Chief Financial Officer (CFO) | Confidential `[A][B]` | Case closure `[A]` illustrative | `[Legal / regulatory verification required]` / `[NDMO verification required]` | `[Legal / regulatory verification required]` | None recorded | To be confirmed after verification | Conceptual — appropriate to Confidential and media | Data Owner **A** when period is verified | Not live `[A]` | Periodic `[B]` |

**Classification does NOT automatically determine retention duration.** The Restricted rows above do **not** imply a longer or shorter period than Confidential.

---

## 4. Operating rule

A Retention Rule is **incomplete** until:

1. Business purpose is recorded  
2. Trigger is recorded  
3. Period and basis are **verified** (or explicitly recorded as still pending verification)  
4. Data Owner **A** has approved  

Registering a placeholder rule is allowed for MVP **visibility**. Treating a placeholder as a legal keep-or-destroy instruction is **not** allowed.

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Field list and Owner A | Sections 2–4 |
| `[A]` | Illustrative rows | Section 3 |
| `[NDMO verification required]` | NDMO retention specifications | Period / basis |
| `[Legal / regulatory verification required]` | Healthcare / other law | Period / basis |
