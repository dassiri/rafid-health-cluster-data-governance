# Governance Principles

**Document ID:** RHC-DG-P1-003  
**Phase:** 1 — Governance Direction  
**Status:** Documented  
**Does not decide:** Entity-only principles as a final approved set; operating procedures

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

NDMO requires the entity to **adopt the National Data Management and Personal Data Protection Guiding Principles** so the entity’s program aligns to the national agenda. The entity **may** add entity-level principles that augment, not replace, that core set. Principles may sit in the strategy or in a standalone document `[C]` (NDMO Standards v1.5, `DG.1.2`).

This file:

1. **Adopts** the official NDMO guiding principles `[C]`.
2. Records **candidate** Rafid healthcare principles `[A]` / `[B]` that are **not** treated as NDMO text and are **not** a closed approved set.

Principle definitions below follow the official Standards (v1.5, Section 5). Wording is summarized for documentation use; the official PDF remains the source of truth. Mapped domains are those NDMO lists for each principle `[C]`.

---

## 2. Adopted NDMO guiding principles `[C]`

Source: NDMO Standards v1.5, Section 5 — Data Management Guiding Principles.

| Principle | Official intent (summary) | NDMO-mapped domain families (from Section 5) |
| --- | --- | --- |
| **Data as a National Asset** | Government data should be discoverable, protected, and maintained with clear accountability, with potential to be monetized. | Data Governance (and related asset treatment in the national framework) |
| **Data Protection by Design** | Build systems and processes that are proactive in protecting individuals’ privacy and their rights to consent and/or refuse under applicable KSA laws. | Personal Data Protection; Data Classification; Data Security and Protection |
| **Open by Default** | Avail most government data to the public by default unless non-disclosure is justified as of greater public interest. | Open Data; Data Governance |
| **Ethical Data Use** | Build ethical practices around governance and use of data, with fairness, traceability, and contribution to the common good, aligned with Saudi culture. | Data Governance |
| **Purposeful Design** | Human-centric approach to collection, sharing, and usage to meet future needs of the Kingdom. | Data Operations; Data Sharing and Interoperability; Data Architecture; Reference and Master Data Management |
| **Data-Driven Outcomes** | A public sector where operational and strategic decisions and policy formulation are based on data insights. | Business Intelligence and Analytics; Data Value Realization |
| **Learning Culture** | Saudi talent continuously learns, adapts, and leads as data management and technology advance. | Data Value Realization; Business Intelligence and Analytics; Data Governance |
| **Trusted Data** | Build trust through high-quality data and transparency about quality. | Data Quality; Reference and Master Data Management; Data Catalog and Metadata; Document and Content Management |

**Implementation note:** Adopting these principles in a Phase 1 document is a **direction statement**. It is not evidence that Rafid has operationalized them in systems, training, or audits.

---

## 3. How Rafid will apply Open by Default `[A]` + `[C]` + `[NDMO verification required]`

NDMO’s **Open by Default** principle is adopted `[C]`.

Rafid is a healthcare delivery cluster whose landscape is dominated by personal and clinical data `[A]`. NDMO classification assigns Public only where impact is none/insignificant, and allows some low-impact data to be Public only after a defined assessment, including whether disclosure breaches existing regulation `[C]` (`DC.3.2`, `DC.3.3`).

**Working application (not a classification procedure):** Open by Default does **not** mean clinical records are published. Openness applies where classification and other applicable law allow. Dataset-level decisions are Phase 5 and sharing/open-data phases. Health-sector and PDPL constraints on disclosure are `[NDMO verification required]`.

---

## 4. Candidate Rafid-level principles `[A]` / `[B]`

NDMO permits additional entity-level principles (`DG.1.2`) `[C]`. The following are **candidates only**. They are not NDMO principles and are not issued as cluster policy.

| Candidate | Intent | Status |
| --- | --- | --- |
| **Care safety first** | Where data use could affect diagnosis, treatment, medication, or identity matching, safety risk outweighs convenience. | Candidate — not approved as a separate official principle |
| **Minimum necessary** | Access and extracts should be limited to what the role or purpose requires. | Candidate — may overlap PDPL/NDMO protection expectations `[NDMO verification required]` |
| **One conversation about the same patient** | Identity and encounter data should converge toward a single operational understanding of the patient over time. | Candidate — MDM design is Phase 10 |
| **No silent copies** | Creating unmanaged copies (shares, extracts, vendor sandboxes) is a governance event, not a personal productivity choice. | Candidate — lifecycle/sharing later |

These candidates must not be briefed as NDMO requirements. If later design rejects them, Phase 1 still stands because the **adopted** set is Section 2.

---

## 5. Intentionally unresolved

- Formal Data Management Committee adoption of Section 2 (`DG.1.4` / committee not yet designed).
- Whether Section 4 candidates are kept, rewritten, or dropped.
- Procedure-level meaning of each principle (policies, training, architecture).
- Exact official English/Arabic principle table layout vs. this summary — always prefer the official PDF if wording is disputed `[C]`.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5, Section 5; `DG.1.2`; `DC.3.2`; `DC.3.3` | Principle names, intent, domain mapping, open/classification interaction |
| `[A]` / `[B]` | Rafid healthcare context; common clinical-data practice | Candidate principles and Open by Default application note |
