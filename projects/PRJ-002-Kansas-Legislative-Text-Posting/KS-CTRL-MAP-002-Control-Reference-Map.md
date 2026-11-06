# KS-CTRL-MAP-002 — AGCL / NBBF / CDT Control Reference Map

**Document ID:** KS-CTRL-MAP-002  
**Artifact type:** MAP (control reference)  
**Project:** PRJ-002 — Kansas Legislative Text Posting  
**Governing SPEC:** SPEC-003 §§9–11  
**Governing Work Card:** CWC-CE-184  
**Lifecycle state:** Proposed  
**Version:** 0.1.1  
**Effective Date:** 2026-11-06  
**Classification:** Reference only — does not modify AGCL, NBBF, or CDT repositories  

PRJ-002 may reference these controls. Ownership remains with their control repositories (ARCH-004 / CLAUDE.md). No files outside Legislative-Manager were written for this card.

---

## 1. AGCL controls (00F–00J)

Titles match the control filenames in [RuntimeRepublic/AGCL-Control-Documents](https://github.com/RuntimeRepublic/AGCL-Control-Documents). Exact clause-level citations for package freeze remain open where noted. Commit SHA pins remain `[TO BE VERIFIED]`.

| Control | Title | Public file | Why SPEC-003 requires affinity | Reference posture |
|---|---|---|---|---|
| 00F | Uncertainty and Black-Swan Stress Control | [00F_Uncertainty_and_Black-Swan_Stress_Control.txt](https://github.com/RuntimeRepublic/AGCL-Control-Documents/blob/main/00F_Uncertainty_and_Black-Swan_Stress_Control.txt) | Emergency path and repository outage handling (SPEC-003 §9; R-005) | Reference only |
| 00G | Transparency and Public Ledger Control | [00G_Transparency_and_Public_Ledger_Control.txt](https://github.com/RuntimeRepublic/AGCL-Control-Documents/blob/main/00G_Transparency_and_Public_Ledger_Control.txt) | Public, permanent, verifiable record of legislative text | Reference only |
| 00H | Constitutional Compatibility Control | [00H_Constitutional_Compatibility_Control.txt](https://github.com/RuntimeRepublic/AGCL-Control-Documents/blob/main/00H_Constitutional_Compatibility_Control.txt) | Joint rule, statute, and CAP must remain constitutionally coherent | Reference only |
| 00I | Enforcement and Remedy Control | [00I_Enforcement_and_Remedy_Control.txt](https://github.com/RuntimeRepublic/AGCL-Control-Documents/blob/main/00I_Enforcement_and_Remedy_Control.txt) | Effect of acting on unposted text must be explicit | Reference only |
| 00J | System Amendment and Version Control | [00J_System_Amendment_and_Version_Control.txt](https://github.com/RuntimeRepublic/AGCL-Control-Documents/blob/main/00J_System_Amendment_and_Version_Control.txt) | Version identifiers and supersession of posted text | Reference only |

Repository: [https://github.com/RuntimeRepublic/AGCL-Control-Documents](https://github.com/RuntimeRepublic/AGCL-Control-Documents)

---

## 2. NBBF concerns

| NBBF concern (SPEC-003 §10) | PRJ-002 engineering note | Reference posture |
|---|---|---|
| Node-scoped budgeting | Identify which node funds and operates the repository (see also `KS-NODE-MAP-002`, `KS-FISC-NOTE-002`) | Reference only |
| Authority boundaries | Opt-in local nodes retain their own authority; state package does not silently annex local power | Reference only |
| Transparency of burdens | Operating cost disclosed structurally in fiscal note; **no estimates in this phase** | Reference only |

**Repository:** [https://github.com/RuntimeRepublic/NBBF-Control-Documents](https://github.com/RuntimeRepublic/NBBF-Control-Documents)  
Commit SHA pin for citation freeze: `[TO BE VERIFIED]`.

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

**CDT repository:** not publicly reachable — public URL remains `[TO BE VERIFIED]`. No CDT files were modified.

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
| 0.1.1 | 2026-11-06 | Replaced local paths with public GitHub links for AGCL 00F–00J and NBBF; CDT remains not publicly reachable `[TO BE VERIFIED]`. |
