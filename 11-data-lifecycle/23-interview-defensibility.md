# Interview Defensibility — Data Lifecycle Management

**INTERNAL / INTERVIEW PREPARATION**

**Document ID:** RHC-DG-P11-023  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Audience:** Candidate using this repository  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]` · `[Legal / regulatory verification required]`

---

## 1. What is Data Lifecycle Management?

Enterprise governance of data from **Create / Acquire** through Register, Classify, Store, Use, Share, Retain, Archive, to **Dispose / Destroy** `[A][B]`. It is **not** a storage architecture, backup product, Records Management programme, or database retention config. I documented a conceptual framework for fictional Rafid `[A]`. I did **not** invent retention numbers or claim NDMO/legal compliance.

---

## 2. Difference between retention and archiving?

**Retention** is the **rule** for how long data must be kept after a trigger (business, legal/regulatory, records, contract, hold, privacy) — period **verified**, not guessed `[B]`. **Archiving** is a **lifecycle state**: reduced active use while still retained `[B]`. Archived data is **not** disposed. Classification persists unless the Owner reclassifies (Phase 5).

---

## 3. Difference between archive and backup?

**Archive** is governed lifecycle state (Owner, classification, retention rule, hold, disposal eligibility). **Backup** supports **recovery and continuity** and is **not** retention or archival `[B]`. Backup expiry is not the Retention Schedule.

---

## 4. How do you determine retention?

Identify the data/record → business purpose → applicable requirements → **retention trigger** → determine **period** (only after verification) → Owner approval → register → monitor → review → archive or dispose `[A][B]`. Classification **does not** automatically set duration. Until verified: `[NDMO verification required]` / `[Legal / regulatory verification required]`. Illustrative triggers `[A]`: creation date, last activity, case closure, contract termination, patient relationship end, record completion — **not** periods.

---

## 5. Who approves retention?

**Data Owner A** for the domain (Phase 4 row 10: Retention/lifecycle decision). Business Data Steward **R**. Custodian **R** for technical implementation. DMO **C**. PDPO **C** where personal data. DMC: Governance escalation and decisions within the approved Phase 3 governance authority and decision-right framework. **No new DMC decision right.** DMC is **not** the routine approver of every rule.

---

## 6. What happens when legal hold is applied?

Identify → apply → **suspend normal disposition** → register affected assets → monitor → release → resume approved lifecycle `[A][B]`. An **active hold overrides normal disposal**. This is **not** legal advice. Litigation rules were **not** invented.

---

## 7. How do you dispose of Restricted data?

Same governance chain: candidate → verified expiry → hold check → Owner **A** → execute **approved** method class → evidence → close `[A][B]`. Classification **influences handling** (stricter method class as appropriate) but does **not** invent a clock or a legally mandatory product. Conceptual methods: secure deletion; cryptographic erasure where applicable; physical destruction for applicable media; controlled destruction by approved provider. **No** method claimed legally mandatory unless verified. PDPO **C** where personal data.

---

## 8. What evidence proves disposal?

A **Disposal Record** `[A]` Proposed Rafid governance artifact (not NDMO-mandated): IDs, asset, Owner, classification, retention rule, eligibility date, legal hold check, authorization, disposal date, method, executing party, evidence/reference, verification, closure status.

---

## 9. How does classification affect lifecycle?

Rafid Public / Internal / Confidential / Restricted `[A][B]` influence **access, sharing, storage safeguards, transmission, monitoring, and disposal handling**. **Classification does NOT automatically determine retention duration.** Retention still considers business need, legal/regulatory, records, contractual where applicable, litigation/hold, and privacy.

---

## 10. How does lineage support lifecycle changes?

Lifecycle change → lineage impact → affected downstream assets → Owner review where necessary `[A][B]`. Examples: source retirement, system migration, asset archival, asset disposal. Phase 9 remains **conceptual**. No technical lineage.

---

## 11. How does MDM interact with lifecycle?

Phase 10 entity lifecycle (Create → Match → Merge → Publish → Maintain → Deactivate, within the longer Propose→Retire chain) is **not** Phase 11 Create→Dispose. **Deactivate ≠ dispose.** Related data follows **enterprise** Retention Rules. **No MDM-specific retention rules.**

---

## 12. How would you start lifecycle management in healthcare?

Year-1 MVP: **Patient / Person Master**, **Clinical / Medical Records**, **Financial / Billing & Claims** `[A]`. Stand up lifecycle status, retention-rule **registry** with **placeholder** periods, decision framework, hold concept, archive and disposal registers, disposal evidence, Owner/Steward responsibilities. **Do not** invent health-record years. **Do not** claim compliance. Verify NDMO and legal requirements before any live keep-or-destroy clock.

---

## 13. Phrases not to use

| Do not say | Say instead |
| --- | --- |
| “We retain clinical records for [any number].” | Period is `[Legal / regulatory verification required]`. |
| “NDMO requires this Retention Schedule.” | Proposed Rafid artifact `[A]`; specs `[NDMO verification required]`. |
| “Archive is our backup.” | Archive ≠ Backup. |
| “Restricted means keep forever.” | No indefinite retention by default; Owner-approved **verified** rule or hold. |
| “We are legally compliant.” | Framework documented; no legal compliance claimed. |
