**FAQ Signal Report --- CW15 2026**

**Purpose**

This report evaluates whether the current evergreen FAQ remains aligned
with observed incident mechanisms from the current week. It is a
governance-only artifact and is not intended for public or educational
use.

**Inputs Declared**

- incidents.csv (CW15 2026)

- taxonomy_report.md (CW15 2026)

- prevention_report.md (CW15 2026)

- governance_notes.md (CW15 2026)

- manifest.md (CW15 2026)

- README.md (CW15 2026)

This is a bootstrap-aligned weekly evaluation.

Current evergreen FAQ corpus: Crypto Loss FAQ (rev17FEB2026)

**Governance Check**

No taxonomy reclassification occurred.\
No scope changes occurred.\
No prevention mapping definitions changed.

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**\
Status: reinforced\
Signals:

- wallet_software_exploit incidents present

- unauthorized transfers linked to prior approvals

- prevention mappings include approval revocation and permission review

**Why did connecting my wallet drain me? I thought connecting was
safe.**\
Status: reinforced\
Signals:

- smart_contract_scam and wallet interaction incidents observed

- malicious contract interactions leading to fund loss

- prevention mappings include contract permission awareness

**I had strong 2FA. How was my account still abused?**\
Status: reinforced\
Signals:

- exchange_vulnerability and account access abuse observed

- incidents referencing insufficient access controls

- prevention mappings include authentication and account security

**What is token approval abuse, and how can it drain funds later?**\
Status: reinforced\
Signals:

- wallet_software_exploit subtype dominant within hacks

- classification warnings tied to approval-based drain behavior

- prevention mappings include approval revocation

**What is "pay-to-withdraw," and why does it keep appearing?**\
Status: reinforced\
Signals:

- exchange_scam subtype present across multiple incidents

- repeated pattern of withdrawal fee requirements

- prevention mappings include refusal to pay withdrawal fees

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**\
Status: reinforced\
Signals:

- exchange_scam incidents involving verification and fee narratives

- prevention mappings include refusal of withdrawal-related payments

**If a platform shows profits, why can't I just withdraw smaller
amounts?**\
Status: reinforced\
Signals:

- scam incidents showing blocked withdrawals after deposits

- staged trust-building followed by restriction patterns

- prevention mappings include platform legitimacy verification

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**\
Status: reinforced\
Signals:

- phishing and impersonation incidents observed

- social_engineering subtype present

- prevention mappings include avoiding unsolicited contact

**Why are recovery services contacting victims almost always scams?**\
Status: absent\
Signals:

- no explicit recovery scam subtype or signals observed in CW15

**Why are physical letters, QR codes, and mailed notices used again?**\
Status: absent\
Signals:

- no incidents involving physical delivery vectors observed

**What is address poisoning, and why does it still work on large
transfers?**\
Status: reinforced\
Signals:

- address_poisoning_copy_paste subtype present

- user_mistake incidents involving address reuse behavior

- prevention mappings include address verification

**Why do wallets sometimes show zero balance after restore?**\
Status: reinforced\
Signals:

- lost_wallet_access subtype present

- incidents involving recovery and access confusion

- prevention mappings include recordkeeping and backup practices

**Why do wrong-network transfers become permanent losses even without a
scam?**\
Status: reinforced\
Signals:

- wrong_network subtype present

- user_mistake incidents involving incompatible transfers

- prevention mappings include network verification

**Can crypto sent to the wrong address be recovered?**\
Status: weakened\
Signals:

- no wrong_address subtype observed in CW15

**What happens if I lose my seed phrase but still have wallet access?**\
Status: reinforced\
Signals:

- lost_wallet_access subtype dominant within user_mistake

- incidents involving missing recovery credentials

- prevention mappings include backup and recordkeeping

**Candidate FAQ Additions**

none identified

**Candidate FAQ Removals**

none identified

**Verdict**

The evergreen FAQ remains broadly aligned with observed CW15 incident
mechanisms. No additions or removals are recommended. This week
reinforces existing coverage without introducing new FAQ requirements.
