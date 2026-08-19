# MDM Integration (Conceptual)

**Document ID:** RHC-DG-P10-015  
**Version:** 1.0  
**Status:** Implemented (conceptual only)  
**Owner:** DMO `[B]`  
**Approver:** CDO `[B]`  
**Effective Date:** Upon DMC approval of POL-001 — not claimed as live `[A]`  
**Review Date:** Periodic `[B]`  
**Classification:** Internal `[A][B]` (Rafid working label — not an NDMO national tier)  
**Change History:** v1.0 — Conceptual relationships; no technical architecture.

**Phase:** 10 — Master data management  
**Does not decide:** ESB, APIs, MDM hub, ETL

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records **conceptual** relationships. It does **not** create technical integration architecture.

---

## 2. Relationships (locked)

```text
MDM
↔ Data Quality
↔ Metadata / Catalog
↔ Lineage
↔ Classification
↔ Ownership
↔ Data Sharing
```

| Related phase | Use |
| --- | --- |
| **Phase 7** Data Quality | Uniqueness/consistency of masters; issue path; no second framework |
| **Phase 8** Metadata / Catalog | Master Data Entity type; glossary terms; lineage metadata fields |
| **Phase 9** Lineage | Impact of identity change on downstream encounter/claim |
| **Phase 5** Classification | Owner assesses master **datasets**; illustrative tiers are not standing rules |
| **Phase 4** Ownership | Three Core MDM Owner titles; two sharing **A**s unchanged |

---

## 3. Example chain (locked)

```text
MDM change
→ Lineage impact
→ Data Quality impact
→ Catalog metadata update
```

Illustrative `[A]`: merge of duplicate Patient identities → Phase 9 conceptual lineage to encounter and claims extract → uniqueness issue close on CDE-002 → catalog Master Data Entity and glossary **Patient** record updated.

No bus, no API design, no ETL.

Sharing still: Owner business **A**; PDPO privacy **A** where personal data applies.

---

## 4. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[A]` | Illustrative merge chain | Section 3 |
| `[B]` | Cross-capability impact | Sections 2–3 |
| `[C]` | Related domain **names** | Context |
| `[NDMO verification required]` | Official NDMO MDM-integration specifications | Not claimed |
