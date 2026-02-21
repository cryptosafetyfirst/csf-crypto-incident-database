**faq_signal_report.md --- CW08 2026**

**Purpose**

This report identifies **FAQ-relevant misconception signals** observed
in CW08 and evaluates whether they:

- reinforce existing evergreen FAQ questions

- introduce new candidate questions

- show weakening or disappearance of prior signals

This report is **non-public**, **non-educational**, and
**non-analytical**.\
It exists solely to govern the evergreen FAQ page.

------------------------------------------------------------------------

**Inputs Declared (CW08)**

- incidents.csv (CW08)

- taxonomy_report.md (CW08)

- prevention_report.md (CW08)

- governance_notes.md (CW08)

- manifest.md (CW08)

- README.md (CW08)

Baseline FAQ reference:

- Evergreen FAQ corpus (15 questions)

This is an incremental report.

------------------------------------------------------------------------

**Governance Check**

- No taxonomy reclassification reported

- No scope changes reported

- No prevention mapping changes reported

CW08 signals are comparable to prior weeks.

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment (CW08)**

Each entry below evaluates whether CW08 incidents reinforce an existing
FAQ question.

------------------------------------------------------------------------

**FAQ 1**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

Status:

- reinforced

CW08 signals:

- fake_app_or_extension_hack incident present

- wallet interaction within unverified environments

- exchange_scam involving execution authority assumptions

Dominant anchors:

- taxonomy: fake_app_or_extension_hack

- taxonomy: exchange_scam

- prevention: platform legitimacy verification failure

------------------------------------------------------------------------

**FAQ 2**

**Why did connecting my wallet drain me? I thought connecting was
safe.**

Status:

- reinforced

CW08 signals:

- single-interaction malicious environment cases

- execution authority misunderstanding

Dominant anchors:

- taxonomy: fake_app_or_extension_hack

- prevention: platform legitimacy verification failure

------------------------------------------------------------------------

**FAQ 3**

**I had strong 2FA. How was my account still abused?**

Status:

- absent

CW08 signals:

- no session persistence abuse subtype

- no 2FA bypass mechanism observed

Dominant anchors:

- none observed in CW08

------------------------------------------------------------------------

**FAQ 4**

**What is token approval abuse, and how can it drain funds later?**

Status:

- absent

CW08 signals:

- no approval-related dominant subtype

- no approval revocation mapping in prevention normalization

Dominant anchors:

- none observed in CW08

------------------------------------------------------------------------

**FAQ 5**

**What is "pay-to-withdraw," and why does it keep appearing?**

Status:

- reinforced

CW08 signals:

- exchange_scam dominant subtype

- deposit-to-unlock withdrawal mechanics

- prevention mapping: Do not pay fees to unlock withdrawals

Dominant anchors:

- taxonomy: exchange_scam

------------------------------------------------------------------------

**FAQ 6**

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

Status:

- reinforced

CW08 signals:

- externally required withdrawal fees

- compliance-framed extraction narratives

Dominant anchors:

- taxonomy: exchange_scam

- prevention: Do not pay fees to unlock withdrawals

------------------------------------------------------------------------

**FAQ 7**

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

Status:

- reinforced

CW08 signals:

- staged withdrawal progression

- escalating requirements tied to displayed balances

Dominant anchors:

- taxonomy: exchange_scam

- prevention: platform legitimacy verification failure

------------------------------------------------------------------------

**FAQ 8**

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

Status:

- reinforced

CW08 signals:

- impersonation patterns

- unsolicited contact exploitation

Dominant anchors:

- taxonomy: social_engineering

- prevention: Avoid unsolicited messages calls and DMs

------------------------------------------------------------------------

**FAQ 9**

**Why are recovery services contacting victims almost always scams?**

Status:

- reinforced

CW08 signals:

- second-stage extraction after prior loss

- fabricated recovery narratives

- additional fee demands

Dominant anchors:

- taxonomy: exchange_scam

- taxonomy: social_engineering

- prevention: refusal of fee-based recovery

------------------------------------------------------------------------

**FAQ 10**

**Why are physical letters, QR codes, and mailed notices used again?**

Status:

- weakened

CW08 signals:

- no explicit mailed impersonation subtype

- no QR-based subtype labeling

Dominant anchors:

- none explicitly labeled in CW08

------------------------------------------------------------------------

**FAQ 11**

**What is address poisoning, and why does it still work on large
transfers?**

Status:

- reinforced

CW08 signals:

- address_poisoning_copy_paste incidents

- losses occurring without attacker interaction at transfer time

Dominant anchors:

- taxonomy: address_poisoning_copy_paste

- prevention: network and address verification failure

------------------------------------------------------------------------

**FAQ 12**

**Why do wallets sometimes show zero balance after restore?**

Status:

- absent

CW08 signals:

- no dominant lost_wallet_access subtype

- no restore-context failure pattern observed

Dominant anchors:

- none observed in CW08

------------------------------------------------------------------------

**FAQ 13**

**Why do wrong-network transfers become permanent losses even without a
scam?**

Status:

- reinforced

CW08 signals:

- wrong_network incidents present

- transfers executed correctly but unrecoverable

Dominant anchors:

- taxonomy: wrong_network

- prevention: network compatibility verification

------------------------------------------------------------------------

**FAQ 14**

**Can crypto sent to the wrong address be recovered?**

Status:

- reinforced

CW08 signals:

- wrong_address incidents present

Dominant anchors:

- taxonomy: wrong_address

------------------------------------------------------------------------

**FAQ 15**

**What happens if I lose my seed phrase but still have wallet access?**

Status:

- absent

CW08 signals:

- no dominant seed_phrase_exposure

- no custody-loss signal dominance

Dominant anchors:

- none observed in CW08

------------------------------------------------------------------------

**Candidate FAQ Additions (CW08)**

**Candidate Question:**

- What is a token launch scam, and how does it extract deposits?

Justification:

- token_launch_scam present and recurring in CW08

- visible in incidents.csv (CW08)

- tied to preventable misunderstanding of token legitimacy

------------------------------------------------------------------------

**Candidate FAQ Removals (CW08)**

- none identified

No baseline FAQ question has fully disappeared in structural relevance.

------------------------------------------------------------------------

**Verdict (CW08)**

- Multiple deception-driven FAQs are reinforced

- Several technical-compromise--specific FAQs are absent this week but
  remain structurally valid

- One candidate addition identified (token_launch_scam)

- No removals recommended

Evergreen FAQ remains aligned with CW08 observed loss mechanisms.
