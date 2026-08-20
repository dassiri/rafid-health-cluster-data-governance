# MDM Golden Record Example `[A]`

**Label:** `[A]` Fictional / illustrative Rafid assumption  
**Does not claim:** A live MDM hub, match-score engine, or a third full Facility MDM workstream

---

## Purpose

One Patient / Person Master example of:

```text
Source records → Matching → Duplicate resolution → Survivorship → Golden Record
```

The golden record is **logical and governed** (Phase 10). It does **not** require one physical database.

**Owner:** Patient Access & Experience Director  
**Steward:** Business Data Steward  
**MVP:** Patient / Person is **primary**. Facility appears only as supporting context (code), not as a separate matching program.

No numeric match threshold is used. Candidate match is qualitative; Owner/Steward confirmation is required (Phase 10).

---

## Source records (synthetic)

Three systems hold slightly different versions of the **same fictional person**.

| Field | Source A — SYN-REG | Source B — SYN-EHR | Source C — SYN-BILL |
| --- | --- | --- | --- |
| Local ID | REG-9001 | EHR-44119 | BILL-77 |
| National ID (CDE-001) | SYN-NID-10001 | SYN-NID-10001 | *(blank)* |
| Patient ID / MRN (CDE-002) | MRN-A1001 | MRN-A1001 | MRN-A1001 |
| Given name | Noura | Noura | N. |
| Family name | Al-Harbi | Al Harbi | Alharbi |
| Date of birth | 1990-03-02 | 1990-03-02 | 1990-03-02 |
| Mobile | 050-000-0001 | 050-000-0001 | *(blank)* |
| Facility code | FAC-SYN-01 | FAC-SYN-01 | FAC-SYN-01 |

---

## Matching (conceptual)

| Signal | Assessment `[A]` |
| --- | --- |
| National ID | A and B identical (`SYN-NID-10001`) |
| MRN | All three identical (`MRN-A1001`) |
| Date of birth | All three identical |
| Name | Same person; spacing/punctuation differs |
| Result | **Candidate duplicate / same person** — not auto-merged |

Silent merge is **not** allowed. Duplicate Review Register occupancy would be recorded in a live process (CAT-A15 in the catalog sample).

---

## Survivorship (per-attribute, Owner rule)

Illustrative Patient / Person rules `[A][B]` — not a scoring model:

| Attribute | Trusted source (illustrative) | Why |
| --- | --- | --- |
| National ID | SYN-REG | Registration is the capture point for identity |
| MRN | SYN-REG | Registration issues the cluster identifier |
| Legal name (normalized) | SYN-REG | Registration captures identity documents |
| Date of birth | SYN-REG, confirmed by SYN-EHR | Both agree |
| Mobile | SYN-REG | Billing copy is incomplete |
| Facility code | SYN-REG (supporting) | Lightweight facility context only |

SYN-BILL does **not** win identity attributes. Claims remain **transactional** (Non-MDM at this maturity).

---

## Golden record (logical)

| Attribute | Trusted value `[A]` |
| --- | --- |
| Golden Record ID | GR-PAT-A0001 (logical) |
| National ID | SYN-NID-10001 |
| MRN | MRN-A1001 |
| Name | Noura Al-Harbi (normalized from registration) |
| Date of birth | 1990-03-02 |
| Mobile | 050-000-0001 |
| Facility context | FAC-SYN-01 (supporting reference; not a Facility golden-record program) |
| Status | Active (illustrative) |
| Owner | Patient Access & Experience Director |

Downstream encounter and claim records **consume** GR-PAT-A0001 conceptually. They are not a second person master.

**Not in this example:** Provider matching; Facility matching/survivorship program; HR employee master.
