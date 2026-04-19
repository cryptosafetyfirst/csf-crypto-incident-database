**FAQ Signal Report --- CW16 2026**

**Purpose**

This report evaluates whether the current evergreen FAQ remains aligned
with observed loss mechanisms in the CW16 dataset. It functions as a
non-public, governance-only control artifact used to detect whether FAQ
content reflects current incident-derived signals.

**Inputs Declared (CW16)**

- incidents.csv (CW16)

- taxonomy_report (CW16)

- prevention_report (CW16)

- governance_notes (CW16)

- manifest.md (CW16)

- README.md (CW16)

Report type: bootstrap

Evergreen FAQ corpus: Crypto Loss FAQ --- Common Questions After
Real-World Web3 Incidents

------------------------------------------------------------------------

**Governance Check**

No taxonomy reclassification occurred.\
No scope changes occurred.\
No prevention mapping definitions changed.

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

- Status: reinforced

- Signals:

  - wallet_software_exploit subcategory present

  - prevention mapping includes token approval review signals

- Anchors:

  - taxonomy: wallet_software_exploit

  - prevention: revoke token approvals and review permissions regularly

**Why did connecting my wallet drain me? I thought connecting was
safe.**

- Status: reinforced

- Signals:

  - smart_contract_scam and fake_app_or_extension categories present

  - platform verification prevention dominant

- Anchors:

  - taxonomy: smart_contract_scam; fake_app_or_extension

  - prevention: verify platform legitimacy before use

**I had strong 2FA. How was my account still abused?**

- Status: reinforced

- Signals:

  - wallet_software_exploit and dns_spoofing present

  - authentication-related prevention minimally represented

- Anchors:

  - taxonomy: wallet_software_exploit; dns_spoofing

  - prevention: enable strong authentication and account security

**What is token approval abuse, and how can it drain funds later?**

- Status: reinforced

- Signals:

  - smart_contract_scam recurring

  - approval-related prevention present but low frequency

- Anchors:

  - taxonomy: smart_contract_scam

  - prevention: revoke token approvals and review permissions regularly

------------------------------------------------------------------------

**What is "pay-to-withdraw," and why does it keep appearing?**

- Status: reinforced

- Signals:

  - exchange_scam and crypto_wallet_scam present

  - fee-related prevention mapping present

- Anchors:

  - taxonomy: exchange_scam; crypto_wallet_scam

  - prevention: do not pay fees to unlock withdrawals

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

- Status: reinforced

- Signals:

  - exchange_scam present

  - fee-based deception patterns reflected in prevention mapping

- Anchors:

  - taxonomy: exchange_scam

  - prevention: do not pay fees to unlock withdrawals

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

- Status: reinforced

- Signals:

  - exchange_scam and social_engineering patterns present

  - platform legitimacy prevention dominant

- Anchors:

  - taxonomy: exchange_scam; social_engineering

  - prevention: verify platform legitimacy before use

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

- Status: reinforced

- Signals:

  - social_engineering dominant category

  - unsolicited contact avoidance present

- Anchors:

  - taxonomy: social_engineering

  - prevention: avoid unsolicited messages calls and DMs

**Why are recovery services contacting victims almost always scams?**

- Status: reinforced

- Signals:

  - social_engineering and follow-on scam patterns present

  - unsolicited contact avoidance present

- Anchors:

  - taxonomy: social_engineering

  - prevention: avoid unsolicited messages calls and DMs

**Why are physical letters, QR codes, and mailed notices used again?**

- Status: reinforced

- Signals:

  - social_engineering and phishing present

  - platform verification prevention dominant

- Anchors:

  - taxonomy: social_engineering; phishing

  - prevention: verify platform legitimacy before use

**What is address poisoning, and why does it still work on large
transfers?**

- Status: absent

- Signals:

  - no address_poisoning_copy_paste subtype observed

- Anchors:

  - taxonomy: none observed

  - prevention: none mapped

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

- Status: reinforced

- Signals:

  - backup_failure and lost_wallet_access present

  - recordkeeping prevention present

- Anchors:

  - taxonomy: backup_failure; lost_wallet_access

  - prevention: maintain complete transaction and tax records

**Why do wrong-network transfers become permanent losses even without a
scam?**

- Status: reinforced

- Signals:

  - wrong_network subtype present

  - network verification prevention present

- Anchors:

  - taxonomy: wrong_network

  - prevention: confirm network and address compatibility before
    transfers

**Can crypto sent to the wrong address be recovered?**

- Status: reinforced

- Signals:

  - wrong_address subtype present

  - transaction testing and verification prevention present

- Anchors:

  - taxonomy: wrong_address

  - prevention: test transactions with small amounts first

**What happens if I lose my seed phrase but still have wallet access?**

- Status: reinforced

- Signals:

  - backup_failure subtype present

  - hardware wallet and recordkeeping prevention present

- Anchors:

  - taxonomy: backup_failure

  - prevention: use hardware wallets for long term storage; maintain
    complete transaction and tax records

------------------------------------------------------------------------

**Candidate FAQ Additions (CW16)**

none identified

------------------------------------------------------------------------

**Candidate FAQ Removals (CW16)**

none identified

------------------------------------------------------------------------

**Verdict (CW16)**

The evergreen FAQ remains aligned with observed CW16 incident signals.\
No additions or removals are recommended.\
This week reinforces the existing FAQ baseline without introducing new
mechanisms.
