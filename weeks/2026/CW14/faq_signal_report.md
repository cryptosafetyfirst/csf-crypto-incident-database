**FAQ Signal Report --- CW14 2026**

**Purpose**

This report evaluates whether the current evergreen FAQ remains aligned
with observed loss mechanisms for the week. It is a governance-only
artifact used to detect alignment or drift based strictly on weekly
canonical inputs.

This report is non-public and intended for governance use only.

------------------------------------------------------------------------

**Inputs Declared (CW14)**

- incidents.csv (CW14)

- taxonomy_report.md (CW14)

- prevention_report.md (CW14)

- governance_notes.md (CW14)

- manifest.md (CW14)

- README.md (CW14)

Report type: bootstrap

Evergreen FAQ corpus: Crypto Loss FAQ (rev17FEB2026)

------------------------------------------------------------------------

**Governance Check**

- No taxonomy reclassification occurred

- No scope changes occurred

- No prevention mapping definitions changed

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

Status: absent

Signals:

- No dominant hack subtypes involving execution authority or approvals

- Hack activity limited and not related to approval abuse or session
  compromise

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

Status: absent

Signals:

- No observed subtypes linked to wallet connection abuse

- No prevention mappings referencing connection-based risk

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

Status: absent

Signals:

- No dominant patterns involving session hijacking or authentication
  bypass

- Hack subtype distribution does not reflect account-layer compromise

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

Status: absent

Signals:

- No observed subtypes indicating approval misuse

- No prevention mappings referencing approval revocation or permissions

------------------------------------------------------------------------

**What is "pay-to-withdraw," and why does it keep appearing?**

Status: reinforced

Signals:

- exchange_scam subtype present and recurring

- Prevention mappings include fee-related restrictions and platform
  verification

Dominant anchors:

- exchange_scam

- Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

Status: reinforced

Signals:

- exchange_scam subtype present

- Prevention mappings explicitly include withdrawal fee avoidance

Dominant anchors:

- exchange_scam

- Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

Status: reinforced

Signals:

- exchange_scam subtype present with withdrawal blocking patterns

- Platform legitimacy checks appear in prevention mappings

Dominant anchors:

- exchange_scam

- Verify platform legitimacy before use

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

Status: reinforced

Signals:

- social_engineering subtype is dominant

- Prevention mappings include unsolicited contact avoidance

Dominant anchors:

- social_engineering

- Avoid unsolicited messages calls and DMs

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

Status: reinforced

Signals:

- social_engineering subtype present and recurring

- Prevention mappings include unsolicited contact avoidance

Dominant anchors:

- social_engineering

- Avoid unsolicited messages calls and DMs

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

Status: absent

Signals:

- No observed incidents involving physical delivery vectors

- No taxonomy or prevention signals referencing this mechanism

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

Status: absent

Signals:

- No observed subtype for address poisoning or copy-paste manipulation

- User mistake categories do not include this behavior for this week

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

Status: reinforced

Signals:

- lost_wallet_access subtype present

- Prevention mappings include platform verification and transaction
  validation

Dominant anchors:

- lost_wallet_access

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

Status: reinforced

Signals:

- wrong_network subtype present

- Prevention mappings include network compatibility confirmation

Dominant anchors:

- wrong_network

- Confirm network and address compatibility before transfers

------------------------------------------------------------------------

**Can crypto sent to the wrong address be recovered?**

Status: absent

Signals:

- No wrong_address subtype observed

- No prevention mappings referencing address misdirection

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

Status: reinforced

Signals:

- poor_wallet_backup_practice subtype present

- User error patterns reflect recoverability issues

Dominant anchors:

- poor_wallet_backup_practice

------------------------------------------------------------------------

**Candidate FAQ Additions (CW14)**

none identified

------------------------------------------------------------------------

**Candidate FAQ Removals (CW14)**

none identified

------------------------------------------------------------------------

**Verdict (CW14)**

The evergreen FAQ remains broadly aligned with observed CW14 loss
mechanisms.\
No additions or removals are recommended.\
This week reinforces existing deception-driven and user-error patterns
without introducing new FAQ coverage requirements.
