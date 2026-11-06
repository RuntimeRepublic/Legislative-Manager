# KS-CTRL-MAP-002 — AGCL / NBBF / CDT Control Reference Map

**Document ID:** KS-CTRL-MAP-002  
**Artifact type:** MAP (control reference)  
**Project:** PRJ-002 — Kansas Legislative Text Posting  
**Governing SPEC:** SPEC-003 §§9–11  
**Governing Work Card:** CWC-CE-184  
**Lifecycle state:** Proposed  
**Version:** 0.1.0  
**Effective Date:** 2026-11-06  
**Classification:** Reference only — does not modify AGCL, NBBF, or CDT repositories  

PRJ-002 may reference these controls. Ownership remains with their control repositories (ARCH-004 / CLAUDE.md). No files outside Legislative-Manager were written for this card.

---

## 1. AGCL controls (00F–00J)

Titles below are taken from filenames in the AGCL-Control-Documents tree available to the Human Engineer’s workspace. Exact clause-level citations for package freeze remain open where noted.

| Control | Title (from control filename) | Why SPEC-003 requires affinity | Reference posture |
|---|---|---|---|
| 00F | Uncertainty and Black-Swan Stress Control | Emergency path and repository outage handling (SPEC-003 §9; R-005) | Reference only |
| 00G | Transparency and Public Ledger Control | Public, permanent, verifiable record of legislative text | Reference only |
| 00H | Constitutional Compatibility Control | Joint rule, statute, and CAP must remain constitutionally coherent | Reference only |
| 00I | Enforcement and Remedy Control | Effect of acting on unposted text must be explicit | Reference only |
| 00J | System Amendment and Version Control | Version identifiers and supersession of posted text | Reference only |

**Workspace path evidence (not a publication claim):**  
`X:\GitHub\AGCL-Control-Documents\AGCL-Control-Documents\00F_Uncertainty_and_Black-Swan_Stress_Control.txt` (and sibling `00G`…`00J` files).

**Open:** Canonical public GitHub URLs / commit SHAs for each control file at package freeze — `[TO BE VERIFIED]` if a pin is required later.

---

## 2. NBBF concerns

| NBBF concern (SPEC-003 §10) | PRJ-002 engineering note | Reference posture |
|---|---|---|
| Node-scoped budgeting | Identify which node funds and operates the repository (see also `KS-NODE-MAP-002`, `KS-FISC-NOTE-002`) | Reference only |
| Authority boundaries | Opt-in local nodes retain their own authority; state package does not silently annex local power | Reference only |
| Transparency of burdens | Operating cost disclosed structurally in fiscal note; **no estimates in this phase** | Reference only |

**Repository evidence:** Local tree `X:\GitHub\NBBF-Control-Documents\NBBF-Control-Documents\README.md` states node-scoped budgeting, authority boundaries, fiscal exit conditions, sunset/renewal mechanics. Public remote URL / commit pin for citation freeze `[TO BE VERIFIED]`.

---

## 3. CDT mappings (metadata readiness)

SPEC-003 §11 requires CDT-ready metadata, not CDT runtime.

| Node / edge type | Example for PRJ-002 | Status |
|---|---|---|
| Constitutional locus | Art. 2 § 8; Art. 2 § 14; Art. 14 § 1; new section TBD | Located / placement TBD |
| Statutory locus | K.S.A. 75-4317a; 75-4318; 45-215 et seq. | Located |
| Legislative-rule locus | Joint Rules 1, 3(f) | Located |
| Artifact | RES, BILL, AMD, MAP, CAP, DEF, FISC, PUB | Project IDs only |
| Version-of edge | Each posted text version → its measure | Method `[TO BE VERIFIED]` (see DEF-002-003) |

**CDT repository:** Local workspace `X:\GitHub\CDT-Control-Documents` — authoritative public pin `[TO BE VERIFIED]`. No CDT files were modified.

---

## 4. Explicit non-claims

1. This map does not amend AGCL, NBBF, or CDT text.  
2. Affinity is not compliance certification.  
3. No UNBKE runtime dependency is asserted (SPEC-003 §15.7).

---

## Version History

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-11-06 | Proposed control reference map under CWC-CE-184 §3 item 4. |
