# Ownership Lifecycle

**Document ID:** RHC-DG-P4-006  
**Phase:** 4 — Ownership and stewardship  
**Status:** Implemented

**Labels used:** `[A]` Fictional assumption · `[B]` Industry best practice · `[C]` NDMO-supported · `[NDMO verification required]`

---

## 1. Purpose

This document records how domain ownership is **kept valid** when the fictional cluster `[A]` changes. Design is `[B]`. It is not an NDMO control set.

Throughout: **exactly one Data Owner** after every change. No shared **A**. DMO updates registries; DMO does not become Owner by running the process.

---

## 2. Organizational restructuring

When cluster functions merge, split, or rename:

1. Data Owner of record confirms whether the **domain meaning** still matches the new function.
2. If the function that held ownership disappears, the CDO tables a **single** successor Owner title to the Data Management Committee.
3. DMC **approves** the Owner change (ownership approval control).
4. DMO writes the **Ownership Change Record** and updates the Ownership and Steward Registries.
5. Consulted stakeholders from the old structure remain **C** only if still relevant — they do not become a second Owner.

---

## 3. Domain split

When one domain must become two (for example identity vs a new related subject area):

1. Current Owner and DMO propose the split scope so **no dataset is left without an Owner**.
2. Each resulting domain receives **one** Owner before the split is effective.
3. DMC approves the new domain(s) and Owner(s).
4. Stewards are nominated per domain (may be the same person only as a capacity choice, not as merged accountability of two Owners).
5. Unassigned remainder, if any, is **Unassigned-Domain Escalation** until an Owner is approved — it is not silently parked in IT or DMO as Owner.

Creating a new domain is also Section 7.

---

## 4. System changes

When a system of record is replaced, migrated, or added:

- **Custodian** responsibility may move with the platform.
- **Data Owner does not automatically change.** Business meaning stays with the domain Owner.
- Steward and Custodian update technical contacts in the Steward Registry.
- If a system change **mixes two domains** in one platform, ownership stays by **data domain**, not by application owner. IT remains Custodian.

This is not a Phase 5 classification exercise and not a Phase 10 MDM design.

---

## 5. Business responsibility transfer

When operational accountability for a process moves (for example revenue cycle reporting line changes):

1. Outgoing and incoming executives agree which **domain** moves — or confirm it does not.
2. If ownership must move, treat as Owner change: DMC approval, registries, Change Record.
3. Until approval, the **current registered Owner remains A**. There is no “joint Owner” period.

---

## 6. Owner departure

When the person in an Owner **title** leaves:

- Accountability stays with the **title**, then with an **acting** occupant of that title if the cluster names one `[A]` HR practice.
- If the **title** is abolished, treat as restructuring (Section 2). Do not leave the domain on the departed individual.
- Steward continues operational packs; decisions wait for the Owner title (or DMC if the decision is an access exception / residual risk).
- DMO flags the domain in the registry as **Owner seat vacant** until the title is filled or reassigned — vacancy is not DMO ownership.

---

## 7. New domain creation

1. Requestor (CDO, Owner, or Committee) describes why an existing domain cannot hold the data without breaking one-Owner clarity.
2. DMO checks overlap with the eight Year-1 domains.
3. DMC approves the new domain **and** a single Owner **together**.
4. Steward is nominated; registries updated; Change Record filed.
5. Until approval, data remains with the **current** domain Owner of the closest approved domain, or Unassigned-Domain Escalation if no closest Owner is defensible.

Year-1 approved set is the eight domains. Additional domains are not created in this file.

---

## 8. Sources

| ID | Source | Use |
| --- | --- | --- |
| `[B]` | Approved Phase 4 lifecycle handling | All sections |
| `[A]` | Rafid as a changing public cluster | Trigger examples |
| `[C]` | BDE / DMO / DMC **names** | Who approves vs who registers |
| `[NDMO verification required]` | Any specification-level change-control requirement | Not labeled as NDMO controls |
