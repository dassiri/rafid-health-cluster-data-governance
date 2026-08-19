# Dependency Model

**Document ID:** RHC-DG-P13-005  
**Version:** 1.0  
**Status:** Implemented (documentation)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Hard/soft/parallel; not strictly linear.

**Phase:** 13 — Implementation roadmap  
**Does not decide:** A waterfall calendar

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

Dependencies among the twelve workstreams `[A][B]`.

**The roadmap is not strictly linear.**

---

## 2. Hard dependencies (locked)

| Rule | Why |
| --- | --- |
| **WS1 before all workstreams** | Forums and DMO routing must exist before domain work is “governance” rather than local heroics |
| **WS2 before WS4** | Classification **A** is the Data Owner (Phase 4 row 3) |
| **WS4 before WS10** | Sharing handling depends on an Owner-approved Rafid tier |
| **WS2 + WS4 before WS6** | Catalog mandatory fields include Owner, Steward, and Classification |

---

## 3. Soft dependencies (locked)

**WS5 / WS7 / WS8 benefit from WS6** but can **begin narrowly** before full catalog maturity (for example: CDE issue lists, Critical Lineage candidates, duplicate review) without waiting for every Year-1 catalog type to be populated.

---

## 4. Parallelizable (locked)

| Parallel | Note |
| --- | --- |
| **WS3 alongside WS4 / WS5** | Adoption of already-written Policy/Standards while classification and quality MVP start |
| **WS11 from Day 1 across workstreams** | Evidence occupancy and “not evidenced” reporting — not fake scores |
| **WS12 continuously throughout implementation** | Verification register hygiene; **not** a compliance project |

---

## 5. Illustrative chain `[A]`

```text
WS1
 → WS2
    → WS4 → WS10
    → WS2+WS4 → WS6
 → WS3 (parallel with WS4/WS5)
 → WS5 / WS7 / WS8 (narrow start; stronger with WS6)
 → WS9 (Owner A; no invented periods)
 → WS11 (throughout)
 → WS12 (throughout)
```

Year 2 expansion is **gated** ([11](11-implementation-gates.md)), not automatic.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A][B]` | Hard/soft/parallel split | Sections 2–4 |
| `[NDMO verification required]` | Official NDMO dependency order | Not claimed |
