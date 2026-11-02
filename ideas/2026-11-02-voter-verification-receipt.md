# Bill idea — Kansas Voter Verification Receipt Act

| Field | Value |
|---|---|
| Idea ID | IDEA-2026-11-02-VVR |
| Version | 0.1.0 |
| Date | 2026-11-02 |
| Originator / Human Engineer | Human Engineer |
| Proposed jurisdiction / layer | Kansas / state statutory |
| Intended future artifact | BILL; package ID not assigned |
| Status | Proposed idea — non-operative; not an activated production project |
| Authorization | Human Engineer's instruction in this conversation: “make it a bill idea on the Main repo” |
| Scope | Capture the concept for review; no operative statutory text, project activation, certification or implementation authorization |
| CWC-CE / CEP / project SPEC | Not issued for this idea; required workflow remains pending before production engineering |
| Legal authority / affected statutes | Unresolved; authority and dependency research required |
| Effective date / funding | Undetermined |
| Human acceptance | Pending review; repository placement does not imply acceptance |

## Purpose

Allow a voter to leave the polling place with an anonymous receipt and later verify that the corresponding encrypted ballot was included in the published tally. The full verification objective is that a ballot is cast as intended, recorded as cast, and tallied as recorded, while preserving ballot secrecy.

The Human Engineer's central idea is a ballot UID incorporated into the ballot's cryptographic hash, plus a second UID privately delivered as the voter receipt. The voter possesses the receipt and knows the three connected values. No voter biography appears on the receipt.

## The three values

| Value | Proposed role | Privacy boundary |
|---|---|---|
| Ballot UID | Unpredictable identifier printed on the ballot and bound into its encrypted record / cryptographic commitment | Never derived from voter identity, check-in number, time or a predictable sequence |
| Ballot hash | Cryptographic fingerprint binding the ballot UID and the encrypted ballot record within the chosen protocol | Never a simple hash of candidate selections; the exact construction must follow an independently evaluated protocol |
| Receipt UID | Separate, high-entropy secret delivered privately to the voter | Never printed on the retained ballot or published in plaintext; avoid retention in printer queues, logs and lookup analytics |

The receipt may contain all three as readable text and a QR code, subject to protocol review. The ballot UID is an input bound by the hash, not necessarily an extractable substring of the hash. A UID alone is not a password.

**Target:** Only the voter receives the receipt. **Unresolved security claim:** A device that generates or prints a secret may know it. Exclusive voter knowledge cannot be promised until generation, delivery, retention and compromise risks have been evaluated. Someone who copies the receipt can use the same bearer secret.

## Proposed voter journey

1. Privately mark and review a human-readable paper ballot.
2. Have the system interpret and encrypt the ballot and commit its record, using a protocol that supports checking correct capture.
3. Privately receive the verification receipt. Final cast/challenge ordering must follow the evaluated protocol; do not invent a sequence that defeats challenge verification.
4. Retain the paper ballot under election custody for audits and recounts.
5. After election evidence is published, use the receipt on a read-only verification service or independent verifier.
6. Check inclusion in the specified tally version and the validity of the supporting proofs.
7. Report missing, inconsistent or unverifiable evidence through a documented dispute process.

An internet lookup does not require internet-connected voting equipment. ElectionGuard describes offline operation for ballot encryption and later publication of verification evidence. [S2]

## Proposed bill section outline — policy topics, not statutory language

| Section | Proposed subject |
|---|---|
| 1 | Purpose, scope and definitions: distinguish UID, secret, encrypted ballot, hash, commitment and proof |
| 2 | Voter opportunity to receive an anonymous verification receipt, without making receipt possession a condition of counting |
| 3 | Three-value design requirements, uniqueness, secure randomness and election-specific separation |
| 4 | Ballot secrecy: no names, addresses, birth dates, registration numbers, signatures or selections on receipts |
| 5 | Separate eligibility/check-in records from anonymous ballot records; prevent identity linkage through timestamps, ballot ordering, logs or exported images |
| 6 | Cast-as-intended, recorded-as-cast and tallied-as-recorded verification requirements |
| 7 | Publication of encrypted records and proofs; independent downloadable verification and vendor-neutral access |
| 8 | Custody, reconciliation, paper audits and recount compatibility |
| 9 | Receipt problems and dispute resolution: evidence preservation, investigation, deadlines and review |
| 10 | Accessible alternatives, no smartphone requirement, and protection for voters who lose or decline receipts |
| 11 | Independently evaluated pilot, usability testing, certification review and deployment gates |
| 12 | Fiscal analysis, administration, oversight and periodic improvement review |

All section topics are proposed policy choices. Administrative ownership, enforcement powers, remedies and deadlines remain for Human Engineer decisions and legal review.

## Verification requirements and limits

| Question | Required evidence |
|---|---|
| Did the system capture the voter's intent? | Voter review plus the evaluated protocol's capture-verification mechanism; a hash match alone is insufficient |
| Is the committed ballot in the election record? | Independently checkable membership / inclusion evidence bound to the receipt |
| Did it contribute correctly to the result? | Valid tally proofs covering the exact included ballot set |
| Was the correct voter eligible, and was a ballot counted only once? | Separate eligibility controls, ballot accounting and reconciliation; receipts alone do not establish these |
| Was the paper retained and handled correctly? | Chain-of-custody records and audit procedures; cryptography alone does not establish custody |

The EAC identifies the three E2E verification properties and requires ballot secrecy, accessible methods and dispute resolution. Its receipt requirements prohibit showing selections or enabling proof of cast selections to others. [S1]

ElectionGuard is a reference candidate, not a selected or certified solution for this proposal. Its documentation describes confirmation codes, challenged ballots excluded from counting, and published encrypted artifacts and proofs. A challenge provides indirect evidence about correct capture; it does not reveal the choices of the cast ballot. [S2]

## Privacy and operational design questions

- How can the receipt secret be privately generated and delivered without a retained administrative mapping?
- Can verification occur locally from downloaded public evidence, reducing server knowledge of receipt lookups?
- How will printed ballot UIDs be protected from linking publicly released ballot images to individual selections?
- How will timestamps, small precincts, ballot styles, scan order and printer logs be tested for identity leakage?
- How will receipt copying, theft, coercion and malicious QR destinations be addressed without producing proof of candidate choices?
- How are rescans, spoiled ballots, provisional decisions, recounts and corrected tally versions linked without duplicate counting?
- What can a voter prove when a code is absent, and what evidence prevents a fabricated receipt from being treated as proof of a missing vote?
- How will service outages be distinguished from missing election evidence?
- What happens when someone loses a receipt? Counting must not depend on retaining it; identity-based replacement must not silently create a voter-to-ballot map.
- What independent review is necessary before claiming exclusive voter knowledge or end-to-end verification?

No cast-ballot candidate selections should be revealed by lookup. The security objective is verifiable inclusion and tally correctness without a transferable proof of choices.

## Lean Civics pilot and PDCA

**Plan:** Define the threat model, legal review needs, privacy tests, success criteria and stop conditions before selecting a protocol.

**Do:** Run a mock election with synthetic voters and no real electoral consequence. Test altered records, omitted ballots, duplicate entries, copied receipts, printer retention, inaccessible interfaces and unavailable verification services.

**Check:** Have independent reviewers attempt to reproduce verification and identify privacy leaks. Measure receipt usability, proof validation, dispute handling and reconciliation. Cost estimates remain unknown until measured.

**Act:** Revise the concept and publish findings. Stop deployment progression if secrecy, capture verification or independent tally verification cannot be demonstrated. Any real-election pilot requires separate authorization and applicable legal/certification review.

Suggested periodic review: assess verification uptake, unresolved complaints, accessibility, security findings and operating cost. Review cadence is a policy decision; four-month PDCA reporting may be evaluated without implying changes during an active election.

## Authority, controls and impact map

| Area | Status / next work |
|---|---|
| Kansas election authority and secret-ballot constraints | Research required; no statutory conclusions claimed |
| Federal requirements and certification | Review applicability; EAC sources are technical references, not a finding of approval |
| Constitutional-Engineering governance | Reference existing Office governance; no control documents modified |
| Legislative-Manager workflow | Intake concept only; CWC-CE, project specification, applicable KLS engineering and STD-008 progression pending |
| KLS-001 / KLS-004 / KLS-005 / KLS-006 | Assess bill, fiscal, definition and publication requirements before producing a formal package |
| Fiscal / local government impact | Hardware integration, printing, testing, training, accessibility, hosting, audits and support; amounts unknown |
| Runtime / UNBKE | No dependency; any future evidence viewer is separate from election authority and counting |
| Existing projects | Does not amend PRJ-001 or PRJ-002; no new project number reserved |

## Primary technical references

- **[S1] U.S. Election Assistance Commission:** [End to End (E2E) Protocol Evaluation Process](https://www.eac.gov/voting-equipment/end-end-e2e-protocol-evaluation-process). Technical goals, secrecy, dispute resolution and evaluation framework.
- **[S2] ElectionGuard:** [Creating a Verifiable Election](https://electionguard.vote/concepts/Verifiability/). Confirmation codes, challenge mechanism, offline operation and public verification evidence.

These sources informed the conversation and this idea. They do not establish that this proposed three-value arrangement is secure, approved or compliant with Kansas law.

## Next decision

Human Engineer review of the idea, followed by a separately authorized research / engineering work card if advanced. No operative bill text has been drafted.

## Version history

| Version | Date | Change |
|---|---|---|
| 0.1.0 | 2026-11-02 | Captured The Human Engineer's ballot UID, encrypted-ballot hash and private receipt UID concept as a non-operative bill idea. |
