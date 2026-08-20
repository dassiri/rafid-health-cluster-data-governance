# Data Quality Example `[A]`

**Label:** `[A]` Fictional / illustrative Rafid assumption  
**Does not claim:** Live Rafid performance, a quality tool, or NDMO-required thresholds

---

## Purpose

Show **Sample Data → Quality Rules → Issues → Result** on a tiny synthetic registration extract.

This is **not** measured Rafid performance. Thresholds remain `[A]` illustrative (Phase 7).

**Owner (Phase 4):** Patient Access & Experience Director  
**Steward:** Business Data Steward  
**CDEs in scope:** CDE-001 National ID; CDE-002 Patient identifier (MRN)  
**Rules reused:** DQ-003 Completeness (National ID); DQ-001 Uniqueness (National ID)

---

## Sample data (synthetic)

Eight registration rows. Identifiers are obviously fictional.

| Row | SYN Patient ID | National ID (CDE-001) | MRN (CDE-002) | Registration date | Facility code (CDE-013 context) |
| --- | --- | --- | --- | --- | --- |
| 1 | PAT-A0001 | SYN-NID-10001 | MRN-A1001 | 2026-01-12 | FAC-SYN-01 |
| 2 | PAT-A0002 | SYN-NID-10002 | MRN-A1002 | 2026-01-12 | FAC-SYN-01 |
| 3 | PAT-A0003 | *(blank)* | MRN-A1003 | 2026-01-13 | FAC-SYN-01 |
| 4 | PAT-A0004 | SYN-NID-10001 | MRN-A1004 | 2026-01-14 | FAC-SYN-02 |
| 5 | PAT-A0005 | SYN-NID-XXXXX | MRN-A1005 | 2026-01-14 | FAC-SYN-01 |
| 6 | PAT-A0006 | SYN-NID-10006 | MRN-A1002 | 2026-01-15 | FAC-SYN-01 |
| 7 | PAT-A0007 | SYN-NID-10007 | MRN-A1007 | 2024-06-01 | FAC-SYN-01 |
| 8 | PAT-A0008 | SYN-NID-10008 | MRN-A1008 | 2026-01-16 | FAC-SYN-99 |

---

## Rules applied (illustrative)

| Rule | Dimension | Logic `[A]` |
| --- | --- | --- |
| DQ-003 | Completeness | In-scope row must have a National ID, or an Owner-approved exception reason (none recorded here). |
| DQ-001 | Uniqueness | The same National ID must not appear on two different Patient IDs without a documented linked-record exception. |
| Format check | Validity | National ID must match the synthetic pattern `SYN-NID-` + five digits. |
| Key check | Consistency | MRN must be unique in this extract unless an exception is recorded. |
| Currency check | Timeliness | For this **illustrative** extract, registration date older than 12 months is flagged for review (not a legal clock; not an NDMO threshold). |

Integrity (relationship to facility reference) is noted for FAC-SYN-99 if that code is not on the illustrative facility list.

---

## Issues

| Issue ID | Row | CDE | Dimension | Finding `[A]` | Severity (Phase 7 style) |
| --- | --- | --- | --- | --- | --- |
| ISS-A001 | 3 | CDE-001 | Completeness | National ID blank; no exception reason | High |
| ISS-A002 | 1, 4 | CDE-001 | Uniqueness | SYN-NID-10001 used on PAT-A0001 and PAT-A0004 | Critical |
| ISS-A003 | 5 | CDE-001 | Validity | SYN-NID-XXXXX does not match the synthetic digit pattern | High |
| ISS-A004 | 2, 6 | CDE-002 | Uniqueness / Consistency | MRN-A1002 used on two Patient IDs | High |
| ISS-A005 | 7 | CDE-002 context | Timeliness | Registration date is outside the illustrative 12-month review window | Medium |
| ISS-A006 | 8 | CDE-013 context | Integrity | FAC-SYN-99 not on the illustrative facility list (CDE-013) | Medium |

---

## Result (illustrative — not a Rafid score)

| Dimension | In-scope rows | Pass | Fail | Comment |
| --- | --- | --- | --- | --- |
| Completeness (CDE-001) | 8 | 7 | 1 | ISS-A001 |
| Uniqueness (CDE-001) | 8 | — | 2 rows in one duplicate group | ISS-A002 |
| Validity (CDE-001) | 8 | 6 | 2 | blank + invalid pattern |
| Consistency (MRN) | 8 | 6 | 2 | ISS-A004 |
| Timeliness (illustrative window) | 8 | 7 | 1 | ISS-A005 |

**No enterprise-wide quality index is calculated** (Phase 7 lock).

**Remediation path (existing):** Data Quality Issue Management Procedure — `06-policies-standards-procedures/procedures/03-data-quality-issue-management-procedure.md`. Duplicate National IDs are **not** silently merged (Phase 10 matching is a separate design).

**Owner A** remains Patient Access & Experience Director.
