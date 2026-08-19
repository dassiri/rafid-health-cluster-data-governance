# NDMO domain map (names only)

Official domain names `[C]` — NDMO Standards v1.5, Section 6.  
This is a **name map**, not a statement that Rafid has implemented any domain.

```mermaid
flowchart LR
  subgraph protect [Classification and protection]
    DC[13 Data Classification]
    PDP[14 Personal Data Protection]
    SEC[15 Data Security - NCA]
  end
  subgraph govern [Governance and enablement]
    DG[1 Data Governance]
    MCM[2 Catalog and Metadata]
    DQ[3 Data Quality]
    OPS[4 Data Operations]
    DCM[5 Document and Content]
    ARCH[6 Architecture and Modeling]
  end
  subgraph use [Use sharing and value]
    MDM[7 Reference and MDM]
    BI[8 BI and Analytics]
    SHR[9 Sharing and Interoperability]
    VAL[10 Data Value Realization]
    OD[11 Open Data]
    FOI[12 Freedom of Information]
  end
  DG --> MCM
  DG --> DQ
  DG --> DC
```

Grouping into the three boxes is a reading aid `[B]`. It is **not** an official NDMO grouping. Official grouping language in the Standards includes themes such as Data Assetization, Data Usage, Data Classification and Availability, and Data Protection `[C]` (Section 6 figure description). If a brief requires official grouping, use the PDF figure, not this diagram.
