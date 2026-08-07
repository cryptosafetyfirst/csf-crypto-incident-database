**FAQ Signal Report --- CW31 + CW32 2026**

**Purpose**

This report evaluates whether the current evergreen Crypto Loss FAQ
remains aligned with loss mechanisms observed in the CW31 + CW32 2026
dataset.

This report is **non-public and governance-only**. It does not create or
modify incident intelligence, taxonomy classifications, prevention
mappings, or public educational guidance.

**Inputs Declared --- CW31 + CW32 2026**

- incidents.csv --- CW31 + CW32 2026

- taxonomy_report.md --- CW31 + CW32 2026

- prevention_report.md --- CW31 + CW32 2026

- governance_notes.md --- CW31 + CW32 2026

- manifest.md --- CW31 + CW32 2026

- Current evergreen FAQ corpus --- Evergreen_FAQ_rev05JUL2026

- README.md --- not supplied with the current input set

The reporting scope is **CW31 + CW32 2026**, as declared by the
manifest.

This is a **bootstrap FAQ signal report**. No prior FAQ signal report
was used.

The current evergreen FAQ corpus contains questions covering technical
compromise and wallet drains, deception-driven loss patterns, and
irreversible user errors.

The absence of README.md does not prevent the assessment because weekly
scope is established by the manifest and the required analytical and
governance artifacts are available. No information was inferred from a
missing README.

**Governance Check**

**Taxonomy reclassification:** None identified. Classification warnings
remain surfaced without altering underlying classifications.

**Scope changes:** None identified. Dataset integrity conditions confirm
that no scope changes were made.

**Prevention mapping definition changes:** None identified. Prevention
normalization continued to use the established standardized action set,
with incompatible or unclear prevention language conservatively left
unmapped.

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

**Status:** reinforced

**CW31 + CW32 signals:**

- wallet drains without confirmed seed-phrase disclosure

- wallet software exploit classifications

- session-based compromise

- malicious or unsafe wallet/software interaction

**Dominant taxonomy anchors:** wallet_software_exploit,
session_hijacking, smart_contract_scam

**Prevention failure anchors:** account/session security;
wallet-software verification; transaction and interaction verification

The weekly taxonomy contains substantial wallet_software_exploit
representation alongside session_hijacking and smart_contract_scam.

**Why did connecting my wallet drain me? I thought connecting was
safe.**

**Status:** reinforced

**CW31 + CW32 signals:**

- smart-contract interaction

- unsolicited-token interaction

- misunderstood wallet authorization

- unfamiliar Web3 interaction

**Dominant taxonomy anchors:** smart_contract_scam,
approval_misunderstanding

**Prevention failure anchors:** transaction testing; interaction
verification

**I had strong 2FA. How was my account still abused?**

**Status:** reinforced

**CW31 + CW32 signals:**

- authenticated-session abuse

- account compromise occurring beyond initial authentication

- phishing affecting authenticated account environments

**Dominant taxonomy anchors:** session_hijacking, phishing

**Prevention failure anchors:** strong authentication and account
security

session_hijacking is explicitly represented in the weekly taxonomy,
while strong authentication and account security also receives a
prevention mapping.

**What is token approval abuse, and how can it drain funds later?**

**Status:** weakened

**CW31 + CW32 signals:**

- approval misunderstanding remains represented

- smart-contract interaction remains represented

- no standardized prevention mapping for recurring approval revocation

**Dominant taxonomy anchors:** approval_misunderstanding,
smart_contract_scam

**Prevention failure anchors:** transaction and interaction verification

The taxonomy retains approval_misunderstanding, but the standardized
prevention action for reviewing and revoking token approvals received no
mapping during this reporting period.

**Can a scammer steal my crypto just by knowing my wallet address?**

**Status:** reinforced

**CW31 + CW32 signals:**

- address poisoning

- unsolicited dust

- wallet-address-based social engineering

**Dominant taxonomy anchors:** address_poisoning_copy_paste,
network_mitm, social_engineering

**Prevention failure anchors:** destination-address verification

**Can someone hack my wallet if they know my public address?**

**Status:** reinforced

**CW31 + CW32 signals:**

- public-address exposure appears alongside address poisoning and
  unsolicited transfers

- observed loss mechanisms require additional compromise or
  authorization mechanisms

**Dominant taxonomy anchors:** address_poisoning_copy_paste,
network_mitm, wallet_software_exploit

**Prevention failure anchors:** destination-address verification

**What is "pay-to-withdraw," and why does it keep appearing?**

**Status:** reinforced

**CW31 + CW32 signals:**

- withdrawal-release payments

- fake platform balances

- additional payment requirements

- blocked withdrawals

**Dominant taxonomy anchors:** exchange_scam, social_engineering,
crypto_wallet_scam

**Prevention failure anchors:** do not pay fees to unlock withdrawals;
verify platform legitimacy

exchange_scam is the largest scam subtype in the weekly taxonomy, and
the prevention report explicitly maps incidents to avoiding payments
intended to unlock withdrawals.

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

**Status:** reinforced

**CW31 + CW32 signals:**

- purported tax payments required for withdrawal

- KYC requirements introduced after deposits

- additional payments tied to fund release

**Dominant taxonomy anchors:** exchange_scam, social_engineering

**Prevention failure anchors:** do not pay fees to unlock withdrawals;
verify platform legitimacy

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

**Status:** reinforced

**CW31 + CW32 signals:**

- displayed trading profits

- early withdrawal functionality used to establish confidence

- later withdrawal restrictions

- additional deposits tied to access

**Dominant taxonomy anchors:** exchange_scam, social_engineering

**Prevention failure anchors:** verify platform legitimacy; test
transaction or withdrawal functionality

**Why does the platform keep asking for another payment before I can
withdraw my funds?**

**Status:** reinforced

**CW31 + CW32 signals:**

- repeated additional-payment demands

- withdrawal blocks

- displayed balances tied to further deposits

**Dominant taxonomy anchors:** exchange_scam, social_engineering,
job_scam

**Prevention failure anchors:** do not pay fees to unlock withdrawals;
verify platform legitimacy

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

**Status:** reinforced

**CW31 + CW32 signals:**

- unsolicited support impersonation

- callers demonstrating knowledge of account information

- instructions to transfer funds under an account-security narrative

**Dominant taxonomy anchors:** social_engineering, phishing

**Prevention failure anchors:** avoid unsolicited messages, calls and
DMs

Avoidance of unsolicited messages, calls, and DMs is explicitly
represented in the normalized prevention mappings.

**Why are recovery services contacting victims almost always scams?**

**Status:** absent

**CW31 + CW32 signals:**

- no stable recurring recovery-service mechanism established in the
  current weekly taxonomy

- no dedicated recurring prevention mapping establishing
  recovery-service activity for this reporting period

**Dominant taxonomy anchors:** none

**Prevention failure anchors:** none

**Why are physical letters, QR codes, and mailed notices used again?**

**Status:** reinforced

**CW31 + CW32 signals:**

- physical Ledger impersonation letters

- unsolicited security-update instructions

- QR-code-based phishing

- impersonation of trusted organizations

**Dominant taxonomy anchors:** phishing

**Prevention failure anchors:** avoid unsolicited communications; verify
official sources

The weekly taxonomy records phishing as a recurring scam subtype.

**What is address poisoning, and why does it still work on large
transfers?**

**Status:** reinforced

**CW31 + CW32 signals:**

- lookalike destination address inserted into transaction history

- destination copied from transaction history

- irreversible transfer to attacker-controlled address

**Dominant taxonomy anchors:** address_poisoning_copy_paste

**Prevention failure anchors:** confirm network and address
compatibility; test transactions with small amounts

address_poisoning_copy_paste is explicitly represented in the current
taxonomy.

**Why do wallets sometimes show zero balance after restore?**

**Status:** weakened

**CW31 + CW32 signals:**

- wallet-access and recovery problems remain represented

- recovery-context and wallet-compatibility issues remain visible

- no strong recurring current-week signal specifically establishes zero
  balance after restoration

**Dominant taxonomy anchors:** lost_wallet_access, backup_failure

**Prevention failure anchors:** no direct standardized prevention anchor

**Why do wrong-network transfers become permanent losses even without a
scam?**

**Status:** reinforced

**CW31 + CW32 signals:**

- unsupported receiving networks

- incompatible token/network combinations

- assets becoming inaccessible without attacker involvement

**Dominant taxonomy anchors:** wrong_network

**Prevention failure anchors:** confirm network and address
compatibility; test transactions with small amounts

wrong_network is explicitly represented in the weekly taxonomy, while
both network/address compatibility checks and small test transactions
appear in the prevention mappings.

**Can crypto sent to the wrong address be recovered?**

**Status:** reinforced

**CW31 + CW32 signals:**

- transfers to unintended addresses

- transfer to a token contract address

- address-poisoning loss

- irreversible valid transactions

**Dominant taxonomy anchors:** wrong_address,
address_poisoning_copy_paste

**Prevention failure anchors:** confirm destination address; test
transactions with small amounts

**What happens if I lose my seed phrase but still have wallet access?**

**Status:** weakened

**CW31 + CW32 signals:**

- wallet recovery failures remain represented

- backup identification failure remains represented

- lost-wallet-access incidents remain present

- no strong recurring current-week signal specifically establishes
  simultaneous active access and missing recovery phrase

**Dominant taxonomy anchors:** lost_wallet_access, backup_failure

**Prevention failure anchors:** no direct standardized prevention anchor

lost_wallet_access is the largest user-mistake subtype in the current
taxonomy, while backup_failure is also represented.

**Candidate FAQ Additions --- CW31 + CW32 2026**

**Can a hardware wallet vulnerability put funds at risk even if the
device was stored securely?**

**CW31 + CW32 basis:**

- recurring wallet-software-exploit classification

- repeated incidents involving wallets generated on affected hardware

- stable wallet_software_exploit taxonomy anchor

- preventable misunderstanding around the distinction between physical
  device protection and wallet-generation/software integrity

**Dominant taxonomy anchor:** wallet_software_exploit

**Prevention failure anchor:** manufacturer remediation and migration
from affected wallet environments

wallet_software_exploit is the dominant hack subtype in the current
taxonomy.

**Candidate FAQ Removals --- CW31 + CW32 2026**

**none identified**

Although the recovery-services FAQ is absent in the current reporting
period and several existing questions have weakened signals, the
supplied current-week evidence does not independently establish that
their underlying mechanisms no longer appear in the taxonomy or incident
data sufficiently to justify removal.

**Verdict --- CW31 + CW32 2026**

The evergreen FAQ remains **substantially aligned** with the mechanisms
represented in CW31 + CW32 2026.

Most existing FAQ questions are reinforced by current-week incident,
taxonomy, or prevention signals. A smaller set is weakened or absent
under the current-week evidence boundary.

**Candidate addition:** one identified.

**Candidate removals:** none identified.

This bootstrap report establishes the **CW31 + CW32 2026 FAQ signal
baseline** for subsequent governance comparison.
