# Classification Criteria

**Document ID:** RHC-DG-P5-003  
**Phase:** 5 — Data classification  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Unit of classification

Classification is applied at the **dataset** level, not automatically at the domain level `[B]`.

A **dataset** here means a bounded collection of records or files that is used, stored, or shared as a unit (for example an extract, a registry, a system table cluster, a report mart) `[B]`. Formal inventory IDs come from the proposed registry, not from Phase 8 catalog tooling (Phase 8 is Designed / Documented as conceptual catalog design; no catalog product is implemented).

Domains in Phase 4 are **ownership groupings**. They are not a single classification stamp.

---

## 2. Decision rule: highest applicable impact `[B]`

Use a **qualitative** rule: assign the Rafid tier that matches the **highest applicable impact** if the dataset is disclosed, modified, or accessed without authorization.

**Do not** introduce numeric scores, weights, or point totals.  
**Do not** treat this rule as a verified NDMO specification. NDMO describes impact assessment at domain/narrative level `[C]`; official impact-to-national-tier mapping is `[NDMO verification required]`.

---

## 3. Impact dimensions to consider `[B]`

Consider all that apply to the **dataset** (not only privacy):

| Dimension | Question (qualitative) |
| --- | --- |
| Privacy impact | Would individuals be identifiable, including patients or staff? |
| Patient safety impact | Could wrong, missing, or leaked data affect diagnosis, treatment, medication, or identity matching? |
| Financial impact | Could compromise cause material financial loss, fraud, or claims distortion? |
| Legal / regulatory impact | Could mishandling breach applicable law or regulator expectations? Mapping to PDPL/NDMO detail `[NDMO verification required]` |
| Security impact | Could compromise enable further unauthorized access or harm to operations? Coordinate with cybersecurity; NCA owns Domain 15 `[C]` |
| Reputational impact | Could compromise seriously damage trust in the cluster? |
| Operational impact | Could compromise stop or degrade cluster operations? |

Also consider the **harm event** types:

- Unauthorized **disclosure**
- Unauthorized **modification**
- Unauthorized **access**

If dimensions disagree, the **highest** resulting Rafid tier wins. No averaging.

---

## 4. Combining and transforming data `[B]`

- **Linkage / combination:** classify the result at least as strictly as the **highest** input dataset, unless a documented, Owner-approved reason exists (for example a deliberately published Public extract).
- **Aggregation:** aggregation does not automatically lower classification. Re-identification and small-cell risk remain qualitative factors for the Owner.
- **De-identification:** may support a **lower** Rafid tier only after the Data Owner approves, with PDPO consulted where personal data is involved. It is not automatic.

---

## 5. What this file does not do

- It does not write a Phase 6 classification **policy**.
- It does not score datasets.
- It does not set review SLAs in days or hours.

---

## 6. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 5 criteria; dataset-level practice | Sections 1–4 |
| `[C]` | NDMO classification domain narrative (impact assessment **concept**); NCA mandate | Why impact is considered; security coordination |
| `[NDMO verification required]` | Official national impact labels and name mapping | Not copied as Rafid scores |
| `[A]` | Rafid as healthcare cluster | Safety and privacy dimensions matter in examples |
