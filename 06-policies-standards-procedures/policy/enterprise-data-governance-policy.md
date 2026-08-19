# Enterprise Data Governance Policy

**Document ID:** RHC-DG-POL-001  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** Chief Data Officer `[B]`  
**Approver:** Data Management Committee `[B]`  
**Effective Date:** Upon DMC approval — not claimed as live `[A]`  
**Review Date:** Periodic with DMC cadence (no numeric SLA) `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Initial Phase 6 policy body for the fictional Rafid Health Cluster `[A]`.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

This Policy is **L3**. Detail lives in Standards (L4) and Procedures (L5). It is not an NDMO specification and is not a compliance claim. NDMO requires entity-level Data Management and Personal Data Protection Policy and Guidelines aligned to national policies and standards `[C]` (narrative). Specification-level mapping is `[NDMO verification required]`.

---

## 1. Purpose

Establish cluster-wide authority, accountability, and mandatory rules for governing Rafid Health Cluster data `[A]` so that data is treated as a managed asset, classified, usable, and shared only with a clear purpose and control `[B]`.

---

## 2. Scope

Applies to all cluster facilities and corporate functions, and to all recorded forms of cluster data, consistent with Phase 2 governance scope `[A]` / `[B]`. NDMO Purpose and Scope covers government data regardless of form `[C]`; Rafid is **assumed** in as a Public Entity `[A]` + `[NDMO verification required]`.

Business partners handling cluster/government data are in scope for alignment; partner-contract drafting is not this Policy’s job `[C]` narrative / `[A]`.

Out of scope: replacing NCA security control design (NDMO Data Security and Protection domain is under NCA `[C]`).

---

## 3. Definitions

| Term | Meaning |
| --- | --- |
| Data Owner | Business-accountable role for a domain (NDMO name: Business Data Executive `[C]`) |
| Business Data Steward | Operational governance executor (NDMO name: Business Data Steward `[C]`) |
| Data Custodian | IT implementer (NDMO name: IT Data Steward `[C]`) |
| Dataset | Bounded collection classified and registered as a unit `[B]` |
| DMC | Data Management Committee (NDMO name: Entity Data Management Committee `[C]`) |
| DMO | Data Management Office `[C]` name |
| Rafid classification tier | Public, Internal, Confidential, or Restricted `[A][B]` — **not** NDMO national tiers `[NDMO verification required]` |

---

## 4. Governance Principles

The cluster **adopts** NDMO Data Management Guiding Principles `[C]`: Data as a National Asset; Data Protection by Design; Open by Default; Ethical Data Use; Purposeful Design; Data-Driven Outcomes; Learning Culture; Trusted Data.

Open by Default does **not** mean clinical or identifiable patient data is published `[A]` / `[C]` application note. Dataset-level classification and sharing rules apply.

Candidate Rafid healthcare principles from Phase 1 remain **candidates**, not additional Policy clauses, unless later adopted.

---

## 5. Governance Authority

Data governance is **federated by data domain**, not by hospital `[B]`.

- Cluster CEO is Executive Sponsor and **chairs** the DMC `[B]`.
- CDO reports **directly** to the Cluster CEO; CIO is a **peer** `[B]`.
- DMC approves this Policy and governance **exceptions**.
- DMO coordinates the framework; it does not become operational Data Owner of a business domain.

---

## 6. Roles & Responsibilities

| Role | Policy-level duty |
| --- | --- |
| Executive Sponsor (CEO) | Resource governance; chair DMC; material regulatory **A** |
| DMC | Approve Policy; approve exceptions; oversight |
| CDO / DMO | Methodology, registries, drafts, KPI pack, consistency |
| Data Owner | Business **A** for the domain (meaning, quality, in-policy access, business sharing, classification) |
| Business Data Steward | Execute operational governance |
| Data Custodian | Technical implementation; **not** business Owner |
| PDPO | Privacy implications; **A** for sharing privacy review of personal data |
| Compliance Officer | Independent process oversight |
| Data Consumer | Use approved sources; raise issues; no unmanaged copies as a right |

Detail: Standards and Procedures.

---

## 7. Data Ownership

Every in-scope data domain **shall** have **exactly one** Data Owner, enterprise-wide across the cluster `[B]`. Assignments are in STD-001 (Phase 4 map). Shared **A** is not used. IT shall not be the business Data Owner.

---

## 8. Data Stewardship

Each domain **shall** have a Business Data Steward who executes under the Owner `[B]`. Custodians implement systems. Appointment follows PRC-001.

---

## 9. Data Classification

Every identified dataset **shall** have an approved Rafid classification: **Public, Internal, Confidential, or Restricted** `[A][B]`. Classification is **dataset-level**. The Data Owner is **Accountable** and approves classification and reclassification. IT does not decide the tier. Official NDMO tier **names** remain unresolved `[NDMO verification required]`. Detail: STD-002, PRC-002.

---

## 10. Data Quality

Data Owners are **Accountable** that domain data is fit for its stated uses `[B]`. Stewards monitor and raise issues. Custodians implement agreed technical fixes. Detailed quality dimensions, thresholds, and scorecards are **out of this Policy** (Phase 7). Detail: STD-003, PRC-003.

---

## 11. Metadata

Datasets in operational use **shall** have a business definition and be registered under catalog governance `[B]`. DMO owns catalog **methodology**; Owners remain **A** for domain meaning. Tool selection and metadata models are Phase 8. Lineage is a conceptual expectation only (Phase 9). Detail: STD-004, PRC-004.

---

## 12. Data Lifecycle

Classification **persists** through archive unless the Owner reclassifies (Phase 5). Retention and disposal **business** decisions remain Data Owner **A** (Phase 4). This Policy does **not** create a separate lifecycle framework (Phase 11). Handling must stay consistent with the dataset’s Rafid tier `[A][B]`.

---

## 13. Data Sharing

Sharing is **two distinct decisions** `[B]`:

1. **Business approval** — Data Owner **Accountable**.
2. **Privacy compliance review for personal data** — PDPO **Accountable**.

These **shall not** be merged into one approval. Restricted external sharing: **Requires Data Owner business approval + PDPO privacy compliance review where personal data is involved**. Detail: PRC-005.

---

## 14. Data Access

In-policy access: Data Owner **A**; Steward prepares; Custodian provisions `[B]`. Out-of-policy access is a **governance exception** (DMC **A**), not Owner self-approval. Detail: PRC-005, PRC-006.

---

## 15. Data Issues

Quality and data issues **shall** be logged, assigned to the owning domain, resolved or escalated, and closed with evidence `[B]`. Owner remains **A** for issue resolution. Detail: PRC-003.

---

## 16. Exceptions

Exceptions to this Policy **shall** be requested, justified, DMO-reviewed, and **approved or denied by the DMC** `[B]`. Time-boxed operational waivers inside an approved envelope remain as Phase 3 (CDO **A**, DMC informed). Envelope text is not expanded here. Detail: PRC-006.

---

## 17. Compliance & Oversight

CDO coordinates alignment work and reporting to DMC `[B]`. NDMO describes a CDO-led annual assessment `[C]`; this Policy does **not** assert that assessment has been performed. Compliance Officer provides independent process oversight. Cybersecurity incidents follow the CISO / NCA path in parallel `[C]`.

---

## 18. Policy Review

DMO prepares a refresh for DMC when strategy, law, or operating model changes, and otherwise on the DMC cadence `[B]`. No numeric review SLA.

---

## 19. Enforcement

Non-conformance is a data issue and/or exception path, not informal local practice `[B]`. Persistent Owner non-participation escalates to DMC, then CEO. This Policy does not create HR disciplinary codes.

---

## Related documents

STD-001 through STD-005; PRC-001 through PRC-006; Phase 3–5 frameworks.
