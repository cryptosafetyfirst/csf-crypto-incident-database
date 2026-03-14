**FAQ Signal Report --- CW11 2026**

**Purpose**

This report evaluates whether the current evergreen Crypto Loss FAQ
remains aligned with loss mechanisms observed in the CW11 2026 incident
dataset.

The report functions as a governance-only artifact used to detect
whether the FAQ continues to reflect mechanisms present in the weekly
dataset.

This report is **non-public** and **governance-only**. It does not
provide educational content, guidance, or analysis beyond signal
validation.

------------------------------------------------------------------------

**Inputs Declared (CW11)**

The following CW11 artifacts were used as inputs:

- incidents.csv (CW11)

- taxonomy_report.md (CW11)

- prevention_report.md (CW11)

- governance_notes.md (CW11)

- manifest.md (CW11)

- README.md (CW11)

The current evergreen FAQ corpus referenced for evaluation is the
**Crypto Loss FAQ --- Common Questions After Real-World Web3
Incidents**.

This report is an **incremental report**, not a bootstrap report.

------------------------------------------------------------------------

**Governance Check**

Taxonomy reclassification:\
No reclassification occurred during the CW11 dataset cycle.

Scope changes:\
No scope changes were introduced during the CW11 reporting cycle.

Prevention mapping definitions:\
No prevention action definitions changed during CW11.

Dataset integrity conditions were confirmed during weekly governance
review.

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

**Status:** reinforced

**CW11 Signals**

- incidents involving malicious approvals and wallet interaction flows

- incidents mapped to smart_contract_scam and fake_app_or_extension_hack

- prevention mappings referencing token approval revocation and
  permission abuse

**Dominant Anchors**

- taxonomy labels: smart_contract_scam, fake_app_or_extension_hack

- prevention mappings: revoke token approvals and review permissions
  regularly

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

**Status:** reinforced

**CW11 Signals**

- incidents involving malicious or compromised websites prompting wallet
  interaction

- wallet drain behavior after signing transactions on compromised
  interfaces

**Dominant Anchors**

- taxonomy labels: smart_contract_scam

- prevention mappings: verify platform legitimacy before use

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

**Status:** reinforced

**CW11 Signals**

- incidents involving malware and compromised environments

- account compromise without credential disclosure

**Dominant Anchors**

- taxonomy labels: malware

- prevention mappings: enable strong authentication and account security

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

**Status:** reinforced

**CW11 Signals**

- incidents involving prior token approval permissions later used to
  transfer funds

- wallet drains executed through previously authorized contracts

**Dominant Anchors**

- taxonomy labels: smart_contract_scam

- prevention mappings: revoke token approvals and review permissions
  regularly

------------------------------------------------------------------------

**Deception-Driven Loss Patterns**

**What is "pay-to-withdraw," and why does it keep appearing?**

**Status:** reinforced

**CW11 Signals**

- incidents involving fake exchanges and withdrawal fee requirements

- repeated fee escalation narratives before withdrawals

**Dominant Anchors**

- taxonomy labels: exchange_scam

- prevention mappings: do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

**Status:** reinforced

**CW11 Signals**

- incidents involving required payments framed as compliance or
  verification

- escalating fee narratives blocking withdrawals

**Dominant Anchors**

- taxonomy labels: exchange_scam

- prevention mappings: do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

**Status:** reinforced

**CW11 Signals**

- incidents involving fake dashboards displaying balances

- withdrawal attempts blocked despite displayed profits

**Dominant Anchors**

- taxonomy labels: exchange_scam

- prevention mappings: verify platform legitimacy before use

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

**Status:** reinforced

**CW11 Signals**

- incidents involving impersonation or deceptive contact narratives

**Dominant Anchors**

- taxonomy labels: social_engineering

- prevention mappings: avoid unsolicited messages calls and DMs

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

**Status:** reinforced

**CW11 Signals**

- incidents involving follow-on payment requests after an initial loss

- narratives involving recovery or fund retrieval services

**Dominant Anchors**

- taxonomy labels: social_engineering

- prevention mappings: verify platform legitimacy before use

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

**Status:** absent

**CW11 Signals**

- no incidents referencing physical mail delivery or QR-code letters

**Dominant Anchors**

- none observed in CW11 taxonomy or prevention mappings

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

**Status:** reinforced

**CW11 Signals**

- incidents involving address poisoning and copied transaction history
  addresses

**Dominant Anchors**

- taxonomy labels: address_poisoning_copy_paste

- prevention mappings: confirm network and address compatibility before
  transfers

------------------------------------------------------------------------

**Irreversible User Errors**

**Why do wallets sometimes show zero balance after restore?**

**Status:** reinforced

**CW11 Signals**

- incidents involving wallet recovery confusion and incorrect
  restoration conditions

**Dominant Anchors**

- taxonomy labels: lost_wallet_access

- prevention mappings: enable strong authentication and account security

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

**Status:** reinforced

**CW11 Signals**

- incidents involving transfers sent on unsupported networks

**Dominant Anchors**

- taxonomy labels: wrong_network

- prevention mappings: confirm network and address compatibility before
  transfers

------------------------------------------------------------------------

**Can crypto sent to the wrong address be recovered?**

**Status:** reinforced

**CW11 Signals**

- incidents involving incorrect destination addresses resulting in
  permanent loss

**Dominant Anchors**

- taxonomy labels: wrong_address

- prevention mappings: confirm network and address compatibility before
  transfers

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

**Status:** reinforced

**CW11 Signals**

- incidents involving poor wallet backup practices and loss of recovery
  capability

**Dominant Anchors**

- taxonomy labels: poor_wallet_backup_practice

- prevention mappings: use hardware wallets for long term storage

------------------------------------------------------------------------

**Candidate FAQ Additions (CW11)**

none identified

All observed CW11 loss mechanisms map to existing FAQ questions.

------------------------------------------------------------------------

**Candidate FAQ Removals (CW11)**

none identified

All existing FAQ mechanisms continue to appear within the CW11 dataset.

------------------------------------------------------------------------

**Verdict (CW11)**

The evergreen FAQ remains aligned with the mechanisms observed in the
CW11 incident dataset.

No FAQ additions or removals are recommended based on CW11 signals.

CW11 continues to reinforce the existing FAQ structure without
introducing new loss mechanisms that require additional FAQ coverage.
