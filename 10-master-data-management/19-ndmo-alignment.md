# NDMO Alignment — Master Data Management

**Document ID:** RHC-DG-P10-019  
**Phase:** 10 — Master data management  
**Status:** Implemented (alignment notes only)  
**Does not claim:** Implementation, evidence, scores, specification completion, or that MDM is NDMO-mandated

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

Phase 10 alignment is **domain-name only** where defensible.

**Do not invent NDMO control IDs.**  
**Do not claim NDMO compliance.**  
**Do not claim MDM requirements are NDMO-mandated unless explicitly verified.**

Specific NDMO MDM/master-data requirements remain:

**`[NDMO verification required]`**

---

## 2. Three-way distinction (mandatory)

| Bucket | What it includes in Phase 10 |
| --- | --- |
| **Verified NDMO-supported information** `[C]` | Reference and Master Data Management is a knowledge-domain **name**; Section 8.1 **counts** (6 controls / 18 specifications) as recorded in Phase 2 — **IDs not copied, not invented**; Trusted Data principle **name** maps in part to this family; DAMA DMBOK is a key reference **name** |
| **Unverified NDMO information** `[NDMO verification required]` | **Specific MDM/master-data requirements**; official golden-record or matching specifications; domain ID string if not in the retrieved extract; Organizational Manual MDM duties |
| **Rafid’s proposed design** `[A][B]` | Core vs Reference vs Non-MDM cut; logical golden record; conceptual matching; per-attribute survivorship; MVP (Patient, Provider, Facility supporting) |

**Do not mix the three buckets.**

---

## 3. General practice vs Rafid vs NDMO

| Kind | Example |
| --- | --- |
| General MDM **best practice** `[B]` | Distinguish master / reference / transaction; logical golden record |
| **Rafid fictional design** `[A]` | Three Core MDM entities; Facility supporting-only MVP |
| **Verified NDMO-supported** `[C]` | Domain **name**; control/spec **counts** already in Phase 2 |
| **Needs verification** | Any “NDMO requires survivorship rule X” |

Do not guess specification IDs under this domain.

---

## 4. What Phase 10 is not

- Not a completed NDMO Reference and Master Data Management implementation  
- Not a vendor MDM  
- Not Phase 11  
- Not Phase 14 assessment evidence  

---

## 5. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[C]` | NDMO Standards v1.5 — domain **name**; Section 8.1 counts as recorded in Phase 2 | Verified column |
| `[NDMO verification required]` | Specific MDM requirements; specification IDs | Unverified column |
| `[A][B]` | Approved Phase 10 framework | Rafid column |
