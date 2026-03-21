**FAQ Signal Report --- CW12 2026**

**Purpose**

This report evaluates whether the current evergreen FAQ remains aligned
with observed loss mechanisms in the current weekly dataset.\
It is a governance-only artifact and is not intended for public use or
educational purposes.

**Inputs Declared (CW12)**

- incidents.csv (CW12)

- taxonomy report (CW12)

- prevention report (CW12)

- governance notes (CW12)

- manifest (CW12)

- README (CW12)

Report type: bootstrap

Evergreen FAQ corpus referenced: Crypto Loss FAQ (rev17FEB2026)

------------------------------------------------------------------------

**Governance Check**

- Taxonomy reclassification: none

- Scope changes: none

- Prevention mapping definition changes: none

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

Status: reinforced

Signals:

- Hack subcategories present: keylogger, clipboard_hijacker, malware

- Prevention gaps: lack of authentication hardening and environment
  protection actions (0 coverage for authentication/security actions)

Dominant anchors:

- clipboard_hijacker, keylogger, malware

- absence of mapped security hardening actions

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

Status: weakened

Signals:

- No dominant presence of fake_app_or_extension or approval-related hack
  subcategories

- Limited direct prevention mapping to browser/extension control (0
  coverage)

Dominant anchors:

- absence of fake_app_or_extension_hack

- absence of browser-extension prevention mapping

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

Status: absent

Signals:

- No incidents mapped to authentication failure or bypass categories

- No prevention mappings to authentication or account security (0
  coverage)

Dominant anchors:

- absence of authentication-related taxonomy signals

- zero coverage for authentication security actions

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

Status: weakened

Signals:

- Some presence of smart_contract_scam (1 case)

- Limited mapping to approval revocation actions (4 cases)

Dominant anchors:

- smart_contract_scam

- revoke token approvals action

------------------------------------------------------------------------

**What is "pay-to-withdraw," and why does it keep appearing?**

Status: reinforced

Signals:

- Exchange scam occurrences (4 cases)

- Direct mapping to "Do not pay fees to unlock withdrawals"

Dominant anchors:

- exchange_scam

- do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

Status: reinforced

Signals:

- Exchange scam subtype presence (4 cases)

- Explicit prevention mapping to withdrawal fee avoidance

Dominant anchors:

- exchange_scam

- do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

Status: reinforced

Signals:

- Exchange scam subtype recurrence (4 cases)

- Platform legitimacy verification is the highest mapped prevention
  action (20 cases)

Dominant anchors:

- exchange_scam

- verify platform legitimacy

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

Status: reinforced

Signals:

- Social engineering scam presence (4 cases)

- Prevention mapping to avoiding unsolicited contact (11 cases)

Dominant anchors:

- social_engineering

- avoid unsolicited messages

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

Status: reinforced

Signals:

- Social engineering and scam dominance overall (74.4%)

- High mapping to unsolicited contact avoidance and platform legitimacy
  checks

Dominant anchors:

- social_engineering

- avoid unsolicited messages, verify platform legitimacy

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

Status: weakened

Signals:

- No explicit taxonomy subtype for physical-mail-based attacks

- No direct prevention mapping tied to this vector

Dominant anchors:

- absence of taxonomy coverage

- absence of prevention mapping

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

Status: absent

Signals:

- No address_poisoning_copy_paste incidents recorded

- No prevention mappings related to clipboard/address validation beyond
  general compatibility checks

Dominant anchors:

- absence of address_poisoning_copy_paste

- absence of direct prevention mapping

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

Status: absent

Signals:

- No incidents mapped to seed_phrase_exposure or recovery
  misinterpretation

- No prevention mappings related to recovery verification behavior

Dominant anchors:

- absence of recovery-related taxonomy signals

- absence of mapped prevention actions

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

Status: reinforced

Signals:

- wrong_network subtype present (1 case)

- Direct prevention mapping to network/address compatibility (4 cases)

Dominant anchors:

- wrong_network

- confirm network and address compatibility

------------------------------------------------------------------------

**Can crypto sent to the wrong address be recovered?**

Status: absent

Signals:

- No wrong_address subtype incidents recorded

- No prevention mapping specific to wrong-address recovery

Dominant anchors:

- absence of wrong_address

- absence of prevention mapping

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

Status: weakened

Signals:

- lost_wallet_access present (4 cases)

- Minimal prevention mapping to backup practices (1 case)

Dominant anchors:

- lost_wallet_access

- weak representation of backup-related prevention actions

------------------------------------------------------------------------

**Candidate FAQ Additions (CW12)**

none identified

------------------------------------------------------------------------

**Candidate FAQ Removals (CW12)**

none identified

------------------------------------------------------------------------

**Verdict (CW12)**

The evergreen FAQ remains broadly aligned with current-week observed
loss mechanisms.

No additions or removals are recommended.

This week establishes a valid baseline for ongoing FAQ signal
evaluation.
