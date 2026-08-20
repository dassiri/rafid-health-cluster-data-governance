# Conceptual Lineage Maps (Working Pack)

**Document ID:** RHC-DG-P9-WP-009  
**Version:** 1.0  
**Status:** Implemented (illustrative maps only)  
**Owner:** DMO `[B]` (maps as teaching artifacts); domain Owners **A** for meaning in a live process  
**Parent design:** [`../../06-worked-example.md`](../../06-worked-example.md)  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Synthetic / Illustrative / Non-production.**

These maps do **not** represent real MOH, NPHIES, or Rafid architecture.

---

## 1. Purpose

Conceptual lineage shows movement between **major logical data structures** at asset / system-class level:

```text
Source → Transformation → Target → Consumer
```

This file records **three** conceptual maps `[A]`. Map 1 is the locked Phase 9 end-to-end example instantiated with catalog IDs. Maps 2–3 stay inside the three MVP domains.

Systems reused from the project landscape and Phase 8 inventory:

| System class | Working ID | Role |
| --- | --- | --- |
| Registration / MPI | SYN-REG | Originating person capture / intended unique patient key |
| Cluster EMR | SYN-EHR | Clinical and encounter record |
| Billing / revenue | SYN-BILL | Claims and patient billing |
| External Claims Interchange | generic consumer | Outbound claims staging — **not** a named national product |

No additional integration platform, warehouse product, or BI tool is claimed as deployed.

---

## 2. Map 1 — Registration to external claims interchange (locked E2E)

```text
Patient Registration Dataset (META-PAT-002)
        ↓  persist / match (conceptual)
Patient Master (META-PAT-001)
        ↓  identity used on encounter
Encounter / Encounter Documentation (META-ENC-001 / META-ENC-002)
        ↓  charge / claim composition (conceptual)
Claim Submission Dataset (META-CLM-001)
        ↓  outbound mapping (conceptual)
External Claims Interchange (consumer)
```

| Hop | Register | Transformation (conceptual) | Target Owner |
| --- | --- | --- | --- |
| Registration → Patient Master | LIN-001 | Persist / MPI-style match **described**, not a matching engine | Patient Access & Experience Director |
| Patient Master → Encounter | LIN-002 | Person key used on clinical documentation | CMO |
| Encounter → Claims | LIN-003 | Charge capture and claim composition | CFO |
| Claims → Interchange | LIN-004 | Outbound mapping to a **generic** national claims interchange | CFO |

**Criticality:** Critical (confirmed Year-1 Critical Lineage Register).  
**Granularity:** Levels 1–2.  
**Classification:** Each dataset is **separately assessed** under Phase 5. Lineage does not auto-inherit Restricted from registration onto every downstream asset.

Identity, diagnosis, and claim meaning remain with their Phase 4 Owners. DMO coordinates the chain. No shared **A**.

---

## 3. Map 2 — Patient source to clinical reporting

```text
Registration / MPI (SYN-REG)
        ↓
Patient Master (META-PAT-001)
        ↓
Clinical data domain — Encounter Documentation (META-ENC-002)
        ↓
Clinical reporting layer (illustrative consumer)
```

| Node | Catalog / system | Lineage role |
| --- | --- | --- |
| Patient source | META-PAT-002 / SYN-REG | Source |
| Patient Master | META-PAT-001 | Target then source |
| Clinical data domain | META-ENC-001 / META-ENC-002 / SYN-EHR | Target then source |
| Reporting layer | Illustrative clinical reporting use | Consumer |

**Register:** LIN-001, LIN-002, LIN-010.  
**Criticality:** LIN-001 and LIN-002 Critical; LIN-010 Important.  
**Does not add** a Quality & Patient Safety MVP domain or a warehouse product.

---

## 4. Map 3 — Claims source to financial reporting

```text
Encounter Documentation Dataset (META-ENC-002 / SYN-EHR)
        ↓  charge / claim composition
Claim Submission Dataset (META-CLM-001 / SYN-BILL)
        ↓  conceptual conform for reporting
Financial / billing reporting (illustrative consumer)
```

A parallel consumer from the same claims asset:

```text
Claim Submission Dataset (META-CLM-001)
        ↓  outbound mapping
External Claims Interchange (generic consumer)
```

| Node | Catalog / system | Lineage role |
| --- | --- | --- |
| Operational / clinical input | META-ENC-002 | Source |
| Curated / extract claims dataset | META-CLM-001 | Target then source |
| Analytical / reporting use | Illustrative financial reporting | Consumer |
| External interchange | Generic claims interchange | Consumer |

**Register:** LIN-003, LIN-004, LIN-012.  
**Criticality:** LIN-003 and LIN-004 Critical; LIN-012 Important.

“Curated” here means the **governed claims extract asset** already in the catalog. It does **not** claim a deployed curation platform.

---

## 5. Generic pattern (for interview explanation)

```text
Source system
     ↓
Operational dataset
     ↓
Master / governed extract
     ↓
Analytical / reporting use
     ↓
Dashboard / report / interchange (consumer)
```

Applied to Rafid MVP assets:

| Pattern node | Rafid working example `[A]` |
| --- | --- |
| Source system | SYN-REG, SYN-EHR, SYN-BILL |
| Operational dataset | META-PAT-002, META-ENC-002 |
| Master / governed extract | META-PAT-001, META-CLM-001 |
| Analytical / reporting use | Claim Rejection Rate; clinical / financial reporting consumers |
| Consumer | Domain huddle / DMC summary; generic external interchange |

---

## 6. What the catalog may expose

At **asset level** only:

```text
Source → Target → Consumer
```

Detailed technical edges stay in [`../technical-lineage/selective-technical-lineage.md`](../technical-lineage/selective-technical-lineage.md) and are **not** required on every catalog page.

---

## 7. What this file does not do

- Does not add a second end-to-end architecture
- Does not invent systems that conflict with Phase 0–1 landscape or Phase 8 inventory
- Does not implement ETL, a graph database, or automated scanning
- Does not claim NPHIES or MOH interchange design
