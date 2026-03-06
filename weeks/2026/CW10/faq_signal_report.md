**FAQ Signal Report --- CW10 2026**

**Purpose**

This report evaluates whether the current evergreen FAQ remains aligned
with the loss mechanisms observed in the CW10 incident dataset. It
serves as a governance-only artifact used to detect potential
misalignment between recurring incident patterns and the questions
addressed in the evergreen FAQ.

This report is non-public and governance-only.

------------------------------------------------------------------------

**Inputs Declared (CW10)**

The following CW10 artifacts were referenced:

- incidents.csv (CW10)

- taxonomy_report (CW10)

- prevention_report (CW10)

- governance_notes.md (CW10)

- manifest.md (CW10)

- README.md (CW10)

This report is produced as an **incremental report**.

The evaluation references the current evergreen FAQ corpus.

------------------------------------------------------------------------

**Governance Check**

Taxonomy reclassification: none observed.

Scope changes: none observed.

Prevention mapping definitions: no changes observed.

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

Status: **reinforced**

Signals:

- incident subtype: social_engineering_hack

- incident subtype: trojan

- incident subtype: fake_app_or_extension_hack

- prevention mapping: revoke token approvals and review permissions
  regularly

Dominant anchors:

- taxonomy: social_engineering_hack

- prevention mapping: approval / permission misuse patterns

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

Status: **reinforced**

Signals:

- incident subtype: social_engineering_hack

- prevention mapping: revoke token approvals and review permissions
  regularly

Dominant anchors:

- taxonomy: social_engineering_hack

- prevention mapping: permission and approval misuse

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

Status: **reinforced**

Signals:

- incident subtype: trojan

- incident subtype: social_engineering_hack

Dominant anchors:

- taxonomy: trojan

- taxonomy: social_engineering_hack

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

Status: **reinforced**

Signals:

- incident subtype: social_engineering_hack

- prevention mapping: revoke token approvals and review permissions
  regularly

Dominant anchors:

- taxonomy: social_engineering_hack

- prevention mapping: approval misuse

------------------------------------------------------------------------

**What is "pay-to-withdraw," and why does it keep appearing?**

Status: **reinforced**

Signals:

- incident subtype: exchange_scam

- prevention mapping: do not pay fees to unlock withdrawals

Dominant anchors:

- taxonomy: exchange_scam

- prevention mapping: withdrawal fee narratives

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

Status: **reinforced**

Signals:

- incident subtype: exchange_scam

- prevention mapping: do not pay fees to unlock withdrawals

Dominant anchors:

- taxonomy: exchange_scam

- prevention mapping: withdrawal fee narratives

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

Status: **reinforced**

Signals:

- incident subtype: exchange_scam

Dominant anchors:

- taxonomy: exchange_scam

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

Status: **reinforced**

Signals:

- incident subtype: social_engineering

Dominant anchors:

- taxonomy: social_engineering

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

Status: **reinforced**

Signals:

- incident subtype: social_engineering

Dominant anchors:

- taxonomy: social_engineering

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

Status: **absent**

Signals:

- no corresponding subtype signals observed

Dominant anchors:

- none observed in CW10

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

Status: **reinforced**

Signals:

- incident subtype: address_poisoning_copy_paste pattern observed
  through transaction-address confusion behavior

Dominant anchors:

- taxonomy: address verification failures

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

Status: **absent**

Signals:

- no corresponding subtype signals observed

Dominant anchors:

- none observed in CW10

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

Status: **reinforced**

Signals:

- incident subtype: wrong_network

- prevention mapping: confirm network and address compatibility before
  transfers

Dominant anchors:

- taxonomy: wrong_network

- prevention mapping: network compatibility verification

------------------------------------------------------------------------

**Can crypto sent to the wrong address be recovered?**

Status: **absent**

Signals:

- no wrong_address subtype observed in CW10

Dominant anchors:

- none observed in CW10

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

Status: **absent**

Signals:

- no seed_phrase_exposure or backup_failure subtype signals observed

Dominant anchors:

- none observed in CW10

------------------------------------------------------------------------

**Candidate FAQ Additions (CW10)**

none identified

------------------------------------------------------------------------

**Candidate FAQ Removals (CW10)**

none identified

------------------------------------------------------------------------

**Verdict (CW10)**

The evergreen FAQ remains aligned with the mechanisms observed in the
CW10 incident dataset.

No additions or removals are recommended based on CW10 signals.

This report does not establish a new baseline.
