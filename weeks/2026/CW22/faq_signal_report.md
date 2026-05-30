**FAQ Signal Report --- CW22 2026**

**Purpose**

This report evaluates whether the current Crypto Loss FAQ remains
aligned with the loss mechanisms observed in the CW22 2026 incident
dataset.

The report compares the existing FAQ question set against the weekly
dataset, classification reporting, prevention reporting, governance
observations, and supporting weekly artifacts.

**Inputs Reviewed**

- incidents.csv

- taxonomy_report.md

- prevention_report.md

- governance_notes.md

- manifest.md

- README.md

- Current Crypto Loss FAQ question set

Report Type: Baseline Review

**Dataset Review**

- No reclassification identified

- No scope changes identified

- No prevention action changes identified

**FAQ Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

Status: Reinforced

Signals:

- social_engineering_hack

- phishing

- smart_contract_scam

- execution authority mechanisms

Anchors:

- social_engineering_hack

- phishing

- Revoke token approvals and review permissions regularly

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

Status: Reinforced

Signals:

- phishing

- smart_contract_scam

- malicious approval flows

Anchors:

- phishing

- smart_contract_scam

- Verify platform legitimacy before use

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

Status: Reinforced

Signals:

- social_engineering_hack

- insider_attack

- session-based compromise narratives

Anchors:

- social_engineering_hack

- insider_attack

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

Status: Reinforced

Signals:

- smart_contract_scam

- malicious approval mechanisms

Anchors:

- smart_contract_scam

- Revoke token approvals and review permissions regularly

------------------------------------------------------------------------

**What is "pay-to-withdraw," and why does it keep appearing?**

Status: Reinforced

Signals:

- exchange_scam

- recurring withdrawal restriction narratives

Anchors:

- exchange_scam

- Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

Status: Reinforced

Signals:

- exchange_scam

- withdrawal-fee narratives

Anchors:

- exchange_scam

- Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

Status: Reinforced

Signals:

- exchange_scam

- fabricated custody environments

Anchors:

- exchange_scam

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

Status: Reinforced

Signals:

- social_engineering

- phishing

- impersonation narratives

Anchors:

- social_engineering

- phishing

- Avoid unsolicited messages calls and DMs

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

Status: Reinforced

Signals:

- exchange_scam

- social_engineering

Anchors:

- exchange_scam

- social_engineering

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

Status: Reinforced

Signals:

- phishing

- social_engineering

- impersonation mechanisms

Anchors:

- phishing

- social_engineering

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

Status: Absent

Signals:

- no address_poisoning_copy_paste incidents observed

Anchors:

- none observed

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

Status: Weakened

Signals:

- limited wallet recovery and backup-related activity

Anchors:

- poor_wallet_backup_practice

- backup_failure

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

Status: Reinforced

Signals:

- wrong_network remained a dominant user-mistake subtype

Anchors:

- wrong_network

- Confirm network and address compatibility before transfers

**Can crypto sent to the wrong address be recovered?**

Status: Reinforced

Signals:

- wrong_address incidents observed

Anchors:

- wrong_address

- Confirm network and address compatibility before transfers

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

Status: Reinforced

Signals:

- poor_wallet_backup_practice

- backup_failure

Anchors:

- poor_wallet_backup_practice

- backup_failure

**Candidate FAQ Additions**

**Why do fake job offers increasingly lead to crypto losses?**

Justification:

- recurring job_scam activity observed

- stable taxonomy subtype present

- tied to recurring misunderstanding regarding employment-related
  payment requests

Anchors:

- job_scam

**Why do romance scams continue to result in crypto transfers?**

Justification:

- recurring romance_scam activity observed

- stable taxonomy subtype present

- tied to trust-based transfer authorization

Anchors:

- romance_scam

**Candidate FAQ Removals**

None identified.

**Verdict**

The current FAQ remains broadly aligned with the loss mechanisms
observed during CW22 2026.

Most existing questions were reinforced by observed incident behavior,
classification patterns, or prevention mappings.

Two candidate additions were identified based on recurring and stable
loss mechanisms observed during the reporting period.

No FAQ removals were identified.
