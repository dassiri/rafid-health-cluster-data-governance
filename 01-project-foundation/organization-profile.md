# Organization Profile

**Document ID:** RHC-DG-P0-002  
**Phase:** 0 — Project Foundation  
**Status:** Documented  
**Label for this file:** Almost all organizational facts are `[A]`. Regulatory posture statements that cite NDMO are `[C]` for the national text and `[NDMO verification required]` for Rafid’s real-world applicability.

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose of this document

This profile defines the **fictional** entity used throughout the framework so later artifacts share one organization story. It is not a commercial, legal, or MOH filing.

---

## 2. Identity

| Attribute | Value | Label |
| --- | --- | --- |
| English name | Rafid Health Cluster | `[A]` |
| Arabic name | مجمع رافد الصحي | `[A]` |
| Short name | Rafid / RHC | `[A]` |
| Organization type | Ministry of Health (MOH) health cluster — multi-facility public healthcare delivery network | `[A]` |
| Country | Kingdom of Saudi Arabia | `[A]` |
| Headquarters | Cluster corporate offices, Rafid City | `[A]` |
| Portfolio status | Fictional organization created for a data governance case study | `[A]` |

---

## 3. Assumed mandate

Rafid Health Cluster is assumed to plan, deliver, and coordinate publicly funded healthcare for a defined catchment, including emergency, inpatient, outpatient, primary care, and selected tertiary services `[A]`.

It is **modeled as** a Public Entity that receives, produces, and holds government data and personal data `[A]`.

NDMO defines Public Entities to include independent governmental or public entities and affiliates in the Kingdom, and treats certain operators of public utilities or public services as public entities `[C]` (NDMO Standards v1.5, Definitions). NDMO defines Government Data as raw or processed data received, produced, or held by public entities, regardless of source, form, or nature `[C]`.

**Applicability of those definitions to a real MOH health cluster is not independently confirmed in this drop** `[NDMO verification required]`. For this portfolio, Rafid is **assumed in** `[A]`.

---

## 4. Scale and footprint `[A]`

Figures below are portfolio assumptions, not operational statistics.

| Attribute | Assumed value |
| --- | --- |
| Catchment population | Approximately 1.1 million |
| Workforce | Approximately 12,000 (clinical, allied health, admin, outsourced support) |
| Acute hospitals | 4 (1 tertiary referral, 2 general, 1 women and children) |
| Primary healthcare centers (PHC) | 18 |
| Specialty centers | 1 oncology center; 1 rehabilitation center |
| Cluster corporate functions | CEO office, medical affairs, nursing, quality, finance, HR, supply chain, IT/digital, legal, internal audit, patient experience |

Facility names used in later examples (all `[A]`):

- Rafid Central Hospital (tertiary)
- North Rafid General Hospital
- South Rafid General Hospital
- Rafid Women and Children Hospital
- Rafid Oncology Center
- Rafid Rehabilitation Center
- PHC network (PHC-01 through PHC-18)

---

## 5. Operating context `[A]`

| Theme | Working assumption |
| --- | --- |
| Care model | Cluster-level referral pathways; PHC as first contact; tertiary at Rafid Central |
| Digital core | Cluster-wide electronic medical record (EMR) with remaining departmental systems |
| Integration | Partial HL7/interface engine; several standalone lab, radiology, and pharmacy modules at older sites |
| Reporting | Routine statistical reporting to MOH; quality indicators to cluster quality office |
| Sharing | Ad hoc data sharing with other clusters, MOH programs, insurers, and academic partners — not yet standardized |
| Language | Arabic and English operational records |

None of the above is an NDMO requirement.

---

## 6. Current-state data governance (as-is) `[A]`

This is the **problem premise** for the program. It is fictional.

| Area | As-is condition |
| --- | --- |
| Authority | No appointed Chief Data Officer; data issues escalate through IT or medical records |
| Policy | Health information confidentiality clauses exist in HR and medical records SOPs; no enterprise data policy stack |
| Ownership | System owners exist; business data owners are informal |
| Classification | Records labeled mainly as “medical record / confidential” by habit, not by NDMO impact assessment |
| Quality | Duplicate patient records; inconsistent national ID capture; lab coding variance across sites |
| Catalog | No enterprise data catalog; data dictionaries live in vendor manuals and personal spreadsheets |
| Lineage | Known by long-tenured interface analysts only |
| Master data | No cluster golden Patient / Provider / Location records |
| Lifecycle | Retention follows mixed medical-records practice; disposal poorly evidenced |
| Partners | Vendor and outsourcing contracts do not consistently address government-data handling |

This as-is picture is **not** an NDMO maturity score.

---

## 7. Stakeholders (inventory only)

This list identifies **who will later need a role** in the operating model. It is not a RACI and does not appoint NDMO officers `[B]`.

| Group | Examples `[A]` | Later-phase relevance |
| --- | --- | --- |
| Cluster executive | CEO, Cluster Medical Director, CFO, CIO/CDIO | Strategy approval; committee sponsorship |
| Clinical leadership | Chiefs of service, nursing directors, pharmacy, lab, radiology | Business data domains |
| Corporate | Quality, finance, HR, supply chain, legal, audit | Non-clinical domains; compliance liaison |
| Digital / IT | Applications, infrastructure, integration, cybersecurity | IT stewardship; NCA-aligned security coordination |
| Health information | Medical records / HIM, coding | Record integrity; classification operations |
| External | MOH, other clusters, insurers, universities, EMR vendor, outsourced billing | Sharing, processors, business partners |

NDMO Data Governance control `DG.4` requires a Data Management Office, Data Management Committee, and named roles (including CDO, Data Governance Officer, and others) `[C]`. **Those appointments are not made in Phase 0.** Role design is Phase 3+. Duty-level alignment to NDMO’s *Organizational Manual* is `[NDMO verification required]` because that manual was not retrieved for this drop.

---

## 8. Related regulatory landscape (orientation only)

This is a **watchlist**, not a compliance claim.

| Instrument | Why it appears here | Label |
| --- | --- | --- |
| NDMO Data Management and Personal Data Protection Standards v1.5 (Jan 2021) | National data management framework for public entities and business partners handling government data | `[C]` |
| NDMO-related regulations named in the Standards (classification, sharing, FOI, and others) | Standards point to them; full texts not used in this drop | `[NDMO verification required]` |
| Saudi Personal Data Protection Law (PDPL) and implementing regulations | Personal health data is likely in scope for a real cluster | `[NDMO verification required]` for mapping to NDMO Personal Data Protection domain |
| National Cybersecurity Authority (NCA) controls | NDMO Domain 15 (Data Security and Protection) is under NCA mandate `[C]` | Security control design is out of this program; coordination is later |
| MOH, CBAHI, SFDA, or Council of Health Insurance rules | Possible sector overlays for a real cluster | `[NDMO verification required]` — not designed here |

---

## 9. Intentionally unresolved

- Legal form (agency vs. cluster administrative unit vs. other) `[A]` left generic.
- Exact reporting line of a future CDO (CEO vs. CIO vs. other) — Phase 3.
- Which facilities are in-scope for year-1 operations — Phase 13.
- Vendor names for EMR and ancillary systems — deliberately generic `[A]`.

---

## 10. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Portfolio fiction | Identity, scale, as-is, stakeholders |
| `[C]` | NDMO Standards v1.5, Definitions; Purpose and Scope; Domain 1; `DG.4`; Domain 15 note on NCA | Public Entity / Government Data; role names; security mandate |
| `[B]` | Stakeholder inventory as a foundation practice | Section 7 structure |
