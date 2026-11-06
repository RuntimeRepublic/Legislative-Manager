# KS-AUTH-MAP-002 — Authority and Layer Map

**Document ID:** KS-AUTH-MAP-002  
**Artifact type:** MAP (authority / layer)  
**Project:** PRJ-002 — Kansas Legislative Text Posting (One-Hour Posting Rule)  
**Governing SPEC:** SPEC-003 v0.4.x — Kansas One-Hour Posting Rule  
**Governing Work Card:** CWC-CE-184 (HG-0 Pre-Draft engineering)  
**Lifecycle state:** Proposed  
**Version:** 0.1.0  
**Effective Date:** 2026-11-06  
**Classification:** Non-operative engineering map — not RES, BILL, AMD, or CAP text  

This map identifies constitutional and joint-rule authority layers relevant to PRJ-002. It does not draft operative text and does not decide HG-1 open items.

---

## 1. Purpose

Record the authority stack that constrains any later joint-rule resolution (`RES-002`), statute package, and constitutional amendment package (`KS-CONST-CAP-002`), and record open items deferred by CWC-CE-184 §9 for HG-1.

---

## 2. Authority layers (identification)

| Layer | Subject | Engineering note for PRJ-002 | Source |
|---|---|---|---|
| Constitutional — house rules | Each house elects its officers and determines the rules of its proceedings; the two houses may adopt joint rules and provide for the manner of change thereof | Limits statute-only enforcement against purely internal legislative steps; joint rules rest on this section | [Kan. Const. art. 2, § 8](https://ksrevisor.gov/kanconst/093_002_0008.html) |
| Constitutional — presentment | Within ten days after passage, every bill shall be signed by the presiding officers and presented to the governor; veto and pocket-approval timing follow | Any statute requiring posting before presentment may interact with this ten-day presentment clock; interaction remains open | [Kan. Const. art. 2, § 14](https://ksrevisor.gov/kanconst/093_002_0014.html) |
| Constitutional — amendment pathway | Concurrent resolution; two-thirds of members elected (or appointed) and qualified in each house; publication; submission to electors; majority of electors voting on the amendment | Pathway for `KS-CONST-CAP-002`; do not simulate electoral outcomes | [Kan. Const. art. 14, § 1](https://ksrevisor.gov/kanconst/093_014_0001.html) |
| Joint rules — adoption / amendment / suspension / revocation | Joint rules adopted under art. 2 § 8; expire with House terms; adopt/amend/suspend/revoke by concurrent resolution; notice and vote thresholds in Joint Rule 1 | A posting joint rule remains suspendable under Joint Rule 1 unless later constrained by statute/CAP | [2025–2026 Joint Rules (HCR 5003 enrolled)](https://www.kslegislature.gov/b2025_26/bills/download/?apn=b2025_26%2Fyear1%2Fready_for_publication%2Fhcr_5003%2Fhcr5003_enrolled.pdf); [HCR 5003 page](https://kslegislature.gov/b2025_26/resolutions/hcr5003/) |

### 2.1 Joint Rule 1 — suspension mechanics (summary of located text)

From the 2025–2026 joint rules text located via HCR 5003 / Senate rules joint-rules reprint:

- Joint rules are adopted under Kan. Const. art. 2, § 8.
- After one day's previous notice, amendment, suspension, or revocation requires the affirmative vote of not less than a majority of the members then elected (or appointed) and qualified in each house.
- Without that notice, amendment, suspension, or revocation requires the affirmative vote of 2/3 of the members then elected (or appointed) and qualified in each house.
- Commencement-of-session special conditions exist for majority adoption without prior notice when sponsor and mailing/availability conditions are met.

Source: [Senate Rules page — Joint Rule 1 text](https://www.kslegislature.gov/b2025_26/senate/rules/); [HCR 5003 enrolled PDF](https://www.kslegislature.gov/b2025_26/bills/download/?apn=b2025_26%2Fyear1%2Fready_for_publication%2Fhcr_5003%2Fhcr5003_enrolled.pdf).

---

## 3. Layer placement for later `RES-002` — OPEN (HG-1)

SPEC-003 §7 and §15.3 record that SPEC-001 defines no layer ID for joint-rule resolutions. CWC-CE-184 §9 deferred the decision:

| Open item | Status | Decision gate |
|---|---|---|
| Layer ID for `RES-002` (presently shown as `[LAYER TBD]-RES-002` in SPEC-003 §7) | **Unknown / deferred** — no layer invented in this map | HG-1 (Human Engineer) |
| Whether a KLS standard for joint-rule resolutions is needed (SPEC-003 §8 / §15.4) | **Unknown / deferred** — gap recorded; no KLS text invented | HG-1 (Human Engineer) |

Engineering consequence until decided: `RES-002` remains identifiable as a project production ID, but its SPEC-001 layer token stays `[LAYER TBD]`.

---

## 4. Related impact loci (non-operative cross-pointers)

| Locus | Role relative to authority stack | Status |
|---|---|---|
| Joint Rule 3(f) — conference report copies / dispense | Existing timing rule that a posting requirement may later replace or extend | Located; see `KS-STAT-MAP-002` / citation verification |
| Joint Rule 4(k) — bill-consideration deadline | Context only; suspendable by majority of members then elected (or appointed) and qualified in the house considering the bill | Located; not a posting rule |
| House Rules / Senate Rules (chamber-local) | Conforming analysis may be needed | `[TO BE VERIFIED]` for chamber-specific posting interactions |

---

## 5. Explicit non-claims

1. This map does not authorize drafting of RES / BILL / AMD / CAP text.  
2. This map does not resolve whether a joint rule alone can create a non-suspendable posting duty (SPEC-003 treats CAP as required for non-suspendable binding).  
3. Exact placement of any new constitutional section remains `[TO BE VERIFIED]` (SPEC-003 §5.2).  

---

## Version History

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-11-06 | Proposed authority/layer map under CWC-CE-184 §3 item 1; open items for RES-002 layer ID and joint-rule KLS standard recorded for HG-1. |
