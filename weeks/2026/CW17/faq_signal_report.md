**FAQ Signal Report --- CW17 2026**

**Purpose**

This report evaluates whether the evergreen FAQ remains aligned with
current-week observed loss mechanisms using only CW17 inputs.\
This report is non-public and governance-only.

------------------------------------------------------------------------

**Inputs Declared (CW17)**

- incidents.csv (CW17)

- taxonomy_report.md (CW17)

- prevention_report.md (CW17)

- governance_notes.md (CW17)

- manifest.md (CW17)

- README.md (CW17)

Report type: bootstrap

Evergreen FAQ corpus: Crypto Loss FAQ (current version)

------------------------------------------------------------------------

**Governance Check**

- taxonomy reclassification occurred: no

- scope changes occurred: no

- prevention mapping definitions changed: no

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

- status: reinforced

- signals:

  - wallet_software_exploit and trojan presence in dataset

  - social_engineering_hack occurrences

- dominant anchors:

  - wallet_software_exploit

  - social_engineering_hack

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

- status: reinforced

- signals:

  - smart_contract_scam incidents present

  - phishing-driven approval behavior observed

- dominant anchors:

  - smart_contract_scam

  - phishing

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

- status: reinforced

- signals:

  - social_engineering_hack incidents involving account access

  - insider_attack involving credential compromise

- dominant anchors:

  - social_engineering_hack

  - insider_attack

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

- status: reinforced

- signals:

  - phishing incidents involving malicious approvals

  - smart_contract_scam involving permission misuse

- dominant anchors:

  - phishing

  - smart_contract_scam

**What is "pay-to-withdraw," and why does it keep appearing?**

- status: reinforced

- signals:

  - exchange_scam dominant subtype presence

  - repeated requirement of additional deposits for withdrawal

- dominant anchors:

  - exchange_scam

  - Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

- status: reinforced

- signals:

  - exchange_scam cases involving upfront payment requirements

  - prevention mapping includes withdrawal fee avoidance

- dominant anchors:

  - exchange_scam

  - Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

- status: reinforced

- signals:

  - exchange_scam cases with staged withdrawals and blocked access

  - romance_scam patterns leading to platform-controlled balances

- dominant anchors:

  - exchange_scam

  - romance_scam

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

- status: reinforced

- signals:

  - social_engineering subtype occurrences

  - blackmail_extortion involving impersonation

- dominant anchors:

  - social_engineering

  - blackmail_extortion

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

- status: absent

- signals:

  - no explicit recovery service incidents observed in dataset

- dominant anchors:

  - none

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

- status: absent

- signals:

  - no incidents involving physical delivery vectors observed

- dominant anchors:

  - none

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

- status: absent

- signals:

  - no address_poisoning_copy_paste subtype present

- dominant anchors:

  - none

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

- status: reinforced

- signals:

  - lost_wallet_access incidents present

- dominant anchors:

  - lost_wallet_access

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

- status: reinforced

- signals:

  - wrong_network user_mistake incidents observed

- dominant anchors:

  - wrong_network

------------------------------------------------------------------------

**Can crypto sent to the wrong address be recovered?**

- status: absent

- signals:

  - no wrong_address subtype present

- dominant anchors:

  - none

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

- status: absent

- signals:

  - no seed_phrase_exposure or backup_failure subtype present

- dominant anchors:

  - none

------------------------------------------------------------------------

**Candidate FAQ Additions (CW17)**

none identified

------------------------------------------------------------------------

**Candidate FAQ Removals (CW17)**

none identified

------------------------------------------------------------------------

**Verdict (CW17)**

The evergreen FAQ remains broadly aligned with CW17 observed loss
mechanisms.\
No additions or removals are recommended.\
This week establishes a valid baseline alignment for ongoing comparison.
