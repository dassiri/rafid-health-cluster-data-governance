# Maturity Assessment Guidance (Working Pack)

**Document ID:** RHC-DG-P12-WP-007  
**Phase:** 12 — KPIs and maturity (working pack)  
**Status:** Implemented (method only — no Rafid score)

**Does not decide:** An actual Rafid maturity result

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[NDMO verification required]`

**Responsible:** DMO (method) · **Review:** CDO · **Approval:** CDO (method). DMC informed under existing authority.

**Parent design:** [`../../21-maturity-assessment-method.md`](../../21-maturity-assessment-method.md) · [`../../23-maturity-assessment-output.md`](../../23-maturity-assessment-output.md) · [`../../22-kpi-maturity-link.md`](../../22-kpi-maturity-link.md)

---

## 1. Purpose

Record **how** maturity would be assessed for future measurement and review `[A][B]`.

**This is NOT an actual Rafid maturity result.**  
If a scoring approach is shown, it is **`[A] Illustrative assessment method`** / **Illustrative assessment only.**

---

## 2. Qualitative lenses (locked — reused)

Assess each of the ten areas using:

| Lens | Question |
| --- | --- |
| **Governance definition** | Is the framework documented and scoped? |
| **Process implementation** | Is the process used, or only written? |
| **Role adoption** | Are Owner / Business Data Steward / Custodian / PDPO acting in role (titles, not named people in this drop)? |
| **Evidence availability** | Do registers exist and contain occupancy? |
| **Measurement** | Are KPIs defined and evidenced (this phase)? |
| **Continuous improvement** | Are actions closed and measures adjusted? |

A level is a **judgement across lenses**, not a formula that copies KPI percentages into a level number.

---

## 3. Assessment steps `[A]` Illustrative assessment method

| Step | Rule |
| --- | --- |
| 1 | For each area, record narrative evidence against the six lenses |
| 2 | Assign a **provisional** level 1–5 using [`five-level-maturity-model.md`](five-level-maturity-model.md) |
| 3 | Use KPIs as **inputs** (coverage, aging, exceptions) — **do not** auto-map “≥80% ⇒ Level 4” |
| 4 | Record residual risk and improvement actions |
| 5 | CDO recommends; DMC is informed / escalates within existing Phase 3 authority |

**Do not** average the ten areas into a single “Rafid = 3.2” headline as a claimed result. An optional overall narrative is allowed; a fake decimal maturity index is vanity.

Cadence: align a **maturity narrative** to the existing **quarterly DMC** pack when CDO so proposes. Do not create an annual-only extra board. NDMO’s own annual specification assessment remains Phase 14 and is **not** this method.

Output shape remains the empty template in [`../../23-maturity-assessment-output.md`](../../23-maturity-assessment-output.md). This pack does not fill it with Rafid scores.

---

## 4. How Reporting & Analytics feeds the assessment

| Maturity area | Informative KPIs (not auto-level) |
| --- | --- |
| Governance | DG-KPI-013, 011 |
| Ownership | DG-KPI-001, DG-KPI-WP-003 |
| Classification | DG-KPI-003 |
| Data Quality | DG-KPI-005, 006, 012, DG-KPI-WP-001, DG-KPI-WP-002 |
| Metadata | DG-KPI-004, 014 |
| Lineage | DG-KPI-007, 015, DG-KPI-WP-004 |
| MDM | DG-KPI-008, 016 |
| Lifecycle | DG-KPI-009, 017, DG-KPI-WP-005 |
| Access/Sharing | DG-KPI-010, 018 |
| Measurement/Improvement | DG-KPI-020, 013 |

A strong leading KPI with no process implementation still fails the **Process implementation** lens.

---

## 5. Future measurement and review (not operational)

```text
Define / refresh KPI
→ Confirm evidence source occupancy
→ Run KPI-input quality check
→ Report Not evidenced or (later) an evidenced value
→ Review in Phase 3 forums
→ Optional: CDO tables a maturity narrative on the quarterly DMC pack
→ Improvement actions close through existing forums
→ Archive the evidence pack
```

Until a baseline exists, Target Status remains **To be established after baseline measurement.**  
Until repeatable results exist, maturity cells remain **Not assessed in this drop.**

---

## 6. Worked non-result — Illustrative assessment only `[A]`

**Illustrative assessment only. NOT an actual Rafid maturity result.**

A reviewer *might* describe:

- **Ownership design** as resembling Level 3 *characteristics* because eight titles are documented.  
- **Managed** as **not evidenced** because the Ownership Registry is not live.  
- **Measurement / KPIs** as resembling Level 3 *characteristics* because the catalogue and this working pack exist, while Level 4 requires evidenced KPI results — which this repository does not claim.

That paragraph is **teaching**. It is **not** a Rafid score.

---

## 7. What assessment is not

- A new Performance Management Committee  
- An NDMO assessment workshop claimed as complete `DG.7`  
- Automatic maturity assignment from the dashboard  
- A claim that documentation equals Optimized  

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Six lenses; inform vs determine | Entire document |
| `[NDMO verification required]` | Official NDMO maturity method | Not claimed |
