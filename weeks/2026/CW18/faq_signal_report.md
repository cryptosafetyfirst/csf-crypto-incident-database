**FAQ Signal Report --- CW18 2026**

**Purpose**

This report evaluates whether the current evergreen FAQ remains aligned
with CW18 observed crypto and Web3 loss mechanisms using only
current-week canonical artifacts. It is governance-only, non-public, and
intended solely for evidence-bound FAQ maintenance.

**Inputs Declared (CW18)**

Artifacts used:

- incidents.csv (CW18)

- taxonomy_report.md (CW18)

- prevention_report.md (CW18)

- governance_notes.md (available but week label mismatch noted; used
  only as advisory context)

- manifest.md (CW18)

- README.md (CW18)

- Evergreen FAQ corpus snapshot

Report type: Bootstrap report

Evergreen FAQ corpus reference: Current Crypto Loss FAQ question set
provided in uploaded FAQ corpus.

**Governance Check**

- Taxonomy reclassification occurred: No

- Scope changes occurred: No

- Prevention mapping definitions changed: No

No governance-plane changes affecting FAQ comparability were identified.

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

**Status:** reinforced\
**CW18 Signals:** wallet_software_exploit, smart_contract_scam,
crypto_wallet_scam, phishing\
**Dominant Anchors:** wallet drains without direct seed exposure;
malicious approvals; compromised wallet authority; execution via prior
authorization

**Why did connecting my wallet drain me? I thought connecting was
safe.**

**Status:** reinforced\
**CW18 Signals:** smart_contract_scam, malicious contract approvals,
wallet connection abuse\
**Dominant Anchors:** smart_contract_scam; revoke permissions gaps;
approval misunderstanding pathways

**I had strong 2FA. How was my account still abused?**

**Status:** reinforced\
**CW18 Signals:** phishing, compromised account via fraudulent support
or verification flows\
**Dominant Anchors:** phishing; environment/session compromise over
credential-only assumptions

**What is token approval abuse, and how can it drain funds later?**

**Status:** reinforced\
**CW18 Signals:** smart_contract_scam, suspicious token interactions,
malicious approval chains\
**Dominant Anchors:** smart_contract_scam; approval persistence;
permission misuse

**What is "pay-to-withdraw," and why does it keep appearing?**

**Status:** reinforced\
**CW18 Signals:** exchange_scam dominance, fake platforms, withdrawal
unlock fees\
**Dominant Anchors:** exchange_scam; do not pay fees to unlock
withdrawals; fabricated custody

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

**Status:** reinforced\
**CW18 Signals:** advance-fee withdrawal barriers, fake compliance
narratives\
**Dominant Anchors:** exchange_scam; withdrawal fee scam mechanics

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

**Status:** reinforced\
**CW18 Signals:** staged small withdrawals followed by blocked larger
balances\
**Dominant Anchors:** exchange_scam; fake dashboard manipulation

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

**Status:** reinforced\
**CW18 Signals:** Ledger-style support impersonation, phishing,
authority abuse\
**Dominant Anchors:** phishing; social engineering; impersonation
credibility abuse

**Why are recovery services contacting victims almost always scams?**

**Status:** reinforced\
**CW18 Signals:** recurring second-stage recovery narratives in scam
victim threads\
**Dominant Anchors:** social_engineering; repeated victim targeting;
false recovery extraction

**Why are physical letters, QR codes, and mailed notices used again?**

**Status:** absent\
**CW18 Signals:** no direct CW18 recurring mailed phishing or QR-mail
incidents observed\
**Dominant Anchors:** no material CW18 reinforcement

**What is address poisoning, and why does it still work on large
transfers?**

**Status:** absent\
**CW18 Signals:** no dominant CW18 address_poisoning_copy_paste
incidents\
**Dominant Anchors:** absent in current taxonomy distribution

**Why do wallets sometimes show zero balance after restore?**

**Status:** weakened\
**CW18 Signals:** limited related wallet confusion, but no dominant
restore-path recurrence\
**Dominant Anchors:** wallet software ambiguity present but not
restore-centric

**Why do wrong-network transfers become permanent losses even without a
scam?**

**Status:** reinforced\
**CW18 Signals:** wrong_network user mistake present\
**Dominant Anchors:** wrong_network; network compatibility failures

**Can crypto sent to the wrong address be recovered?**

**Status:** weakened\
**CW18 Signals:** wrong_address absent this week\
**Dominant Anchors:** no direct wrong_address recurrence

**What happens if I lose my seed phrase but still have wallet access?**

**Status:** weakened\
**CW18 Signals:** seed_phrase_exposure present, but backup-loss pathway
not dominant\
**Dominant Anchors:** seed phrase misuse more visible than seed-loss
custody failure

**Candidate FAQ Additions (CW18)**

**Candidate: Why do fake token deposits or unsolicited "reward" tokens
appear in wallets?**

**Justification:** recurring airdrop_scam and fake token bait incidents
involving unsolicited deposits, fake balances, and token-linked wallet
traps\
**Anchors:** airdrop_scam; smart_contract_scam; crypto_wallet_scam\
**Preventable Misunderstanding:** users misinterpret unsolicited token
presence as legitimate value or rewards

**Candidate: Why do dating apps and WhatsApp investment contacts keep
leading to crypto losses?**

**Justification:** recurring romance_scam + social_engineering +
WhatsApp trading group pathways\
**Anchors:** romance_scam; social_engineering; avoidance of unsolicited
contact\
**Preventable Misunderstanding:** social grooming used as custody
extraction

**Candidate FAQ Removals (CW18)**

None identified.

**Verdict (CW18)**

The evergreen FAQ remains broadly aligned with current-week dominant
loss mechanisms, particularly exchange scams, phishing, wallet authority
abuse, and deception-driven extraction. Multiple existing FAQ questions
were reinforced by CW18 evidence. Candidate additions are justified for
unsolicited fake token deposits and messaging-platform investment
grooming. No removals are supported by CW18 inputs. This report
establishes a valid governance baseline for FAQ signal alignment.
