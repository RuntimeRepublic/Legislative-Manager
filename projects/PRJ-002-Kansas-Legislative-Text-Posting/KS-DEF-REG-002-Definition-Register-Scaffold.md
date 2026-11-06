# KS-DEF-REG-002 — Definition Register Scaffold

**Document ID:** KS-DEF-REG-002  
**Artifact type:** Definition Register (KLS-005 companion)  
**Project:** PRJ-002 — Kansas Legislative Text Posting  
**Governing SPEC:** SPEC-003  
**Governing Work Card:** CWC-CE-184  
**Governing Standard:** KLS-005 — Kansas Legislative Definitions Engineering Standard  
**Lifecycle state:** Proposed  
**Version:** 0.1.0  
**Effective Date:** 2026-11-06  
**Classification:** Scaffold only — terms, loci, and open questions; **no operative definitions**

CWC-CE-184 §3 item 3 and SPEC-003 §7.2(4) require a definition register scaffold for: repository, version, version identifier, posted, official action. Authoritative definition text is deferred until drafting is authorized (HG-1).

---

## 1. Register rules for this phase

1. Classification for each row is preliminary engineering class under KLS-005 §7 (Existing / New / Unknown).  
2. **Proposed authoritative text is intentionally blank.**  
3. Existing Kansas loci are cited when known; otherwise marked unknown.  
4. No term below is enacted or approved by this scaffold.

---

## 2. Term entries

### DEF-002-001 — repository

| Field | Value |
|---|---|
| Definition ID | DEF-002-001 |
| Term | repository |
| Normalized Term Key | repository |
| Aliases | official repository; legislative text repository (informal) |
| Scope type | Package / project (PRJ-002) until a statutory locus is chosen |
| Scope locus | SPEC-003 §2.2 / future BILL-002 — exact statutory locus `[TO BE VERIFIED]` |
| Classification | DEF-NEW (candidate) — no controlling Kansas statutory definition of this project’s “repository” located in Phase 1 |
| Existing controlling locus | Unknown — do not invent |
| Parent artifact | Future `KS-STAT-BILL-002` / `KS-STAT-AMD-002` (not drafted) |
| Open questions | State-owned vs contracted host; whether “repository” is distinct from “public record”; operator identity (Revisor or other) `[TO BE VERIFIED]` |
| Proposed authoritative text | *(none — scaffold only)* |

### DEF-002-002 — version

| Field | Value |
|---|---|
| Definition ID | DEF-002-002 |
| Term | version |
| Normalized Term Key | version |
| Aliases | text version; measure version (informal) |
| Scope type | Package / project |
| Scope locus | SPEC-003 objectives; future statutory/joint-rule text `[TO BE VERIFIED]` |
| Classification | DEF-NEW (candidate) / possible DEF-ADAPT if an existing Revisor or journal usage is later adopted by citation |
| Existing controlling locus | Unknown for this project’s sense — `[TO BE VERIFIED]` against Revisor / legislative journal practice |
| Open questions | Relationship to “version identifier”; whether chamber-engrossed text is a “version” before posting |
| Proposed authoritative text | *(none — scaffold only)* |

### DEF-002-003 — version identifier

| Field | Value |
|---|---|
| Definition ID | DEF-002-003 |
| Term | version identifier |
| Normalized Term Key | version identifier |
| Aliases | version ID; hash (candidate method — not selected) |
| Scope type | Package / project |
| Scope locus | SPEC-003 §15 open item 6 (hashing or version-identifier method to be named) |
| Classification | DEF-NEW (candidate) |
| Existing controlling locus | Unknown |
| Open questions | Method (cryptographic hash, sequential ID, Revisor citation, other) is **unknown** and must not be invented; AGCL 00J affinity noted in `KS-CTRL-MAP-002` |
| Proposed authoritative text | *(none — scaffold only)* |

### DEF-002-004 — posted

| Field | Value |
|---|---|
| Definition ID | DEF-002-004 |
| Term | posted |
| Normalized Term Key | posted |
| Aliases | posting; publicly posted (informal) |
| Scope type | Package / project |
| Scope locus | Future joint rule / statute / CAP — `[TO BE VERIFIED]` |
| Classification | DEF-NEW (candidate) |
| Existing controlling locus | Unknown in the PRJ-002 sense; do not borrow undefined colloquial meaning into operative text yet |
| Open questions | Instant of posting; who posts; what URL or system counts; effect of later supersession |
| Proposed authoritative text | *(none — scaffold only)* |

### DEF-002-005 — official action

| Field | Value |
|---|---|
| Definition ID | DEF-002-005 |
| Term | official action |
| Normalized Term Key | official action |
| Aliases | binding action (KOMA context — related but not identical) |
| Scope type | Package / project |
| Scope locus | Future packages; compare KOMA “binding action” language in [K.S.A. 75-4318](https://www.ksrevisor.gov/statutes/chapters/ch75/075_043_0018.html) |
| Classification | DEF-NEW (candidate) with required conflict check against KOMA vocabulary before drafting |
| Existing controlling locus | KOMA uses “binding action” ([75-4318(a)](https://www.ksrevisor.gov/statutes/chapters/ch75/075_043_0018.html)); whether PRJ-002’s “official action” should reuse, adapt, or stay distinct is **unknown** |
| Open questions | Which legislative steps count (introduction, committee report, final action, conference adoption, presentment); interaction with art. 2 § 8 internal proceedings |
| Proposed authoritative text | *(none — scaffold only)* |

---

## 3. Cross-term open matrix

| Interaction | Status |
|---|---|
| posted ↔ version / version identifier | Unknown until method chosen |
| official action ↔ KOMA binding action | Conflict analysis deferred to HG-1 drafting authorization |
| repository ↔ KORA public record | See `KS-STAT-MAP-002`; retention locus `[TO BE VERIFIED]` |

---

## 4. Explicit non-claims

1. No definition in this register is operative.  
2. Blank proposed-text fields are intentional.  
3. Filling authoritative text requires HG-1 drafting authorization and KLS-005 existing-vs-new analysis for each term.

---

## Version History

| Version | Date | Summary |
|---|---|---|
| 0.1.0 | 2026-11-06 | Proposed KLS-005 scaffold for five SPEC-003 terms under CWC-CE-184 §3 item 3. |
