# Policy hierarchy

Layer codes (`L0`–`L5`) are Rafid documentation labels `[B]`, not NDMO control IDs.

Higher layers prevail.

```mermaid
flowchart TB
  L0[L0 Kingdom law]
  L1[L1 NDMO and NCA]
  L2[L2 Sector rules if applicable]
  L3[L3 Rafid policy]
  L4[L4 Rafid standards]
  L5[L5 Rafid procedures]
  L0 --> L1 --> L2 --> L3 --> L4 --> L5
```

Entity policy (L3) is required by NDMO `DG.2` when that control is executed `[C]`. L3–L5 are **not written** in Phase 0–2.
