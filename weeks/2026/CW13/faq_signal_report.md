**FAQ Signal Report --- CW13 2026**

**Purpose**

This report evaluates whether the evergreen FAQ remains aligned with
current-week observed loss mechanisms based solely on canonical weekly
inputs.\
This report is governance-only and non-public.

------------------------------------------------------------------------

**Inputs Declared (CW13)**

- incidents.csv (CW13)

- taxonomy_report.md (CW13)

- prevention_report.md (CW13)

- governance_notes.md (CW13)

- manifest.md (CW13)

- README.md (CW13)

Report type: bootstrap

Evergreen FAQ corpus: Crypto Loss FAQ (current published version)

------------------------------------------------------------------------

**Governance Check**

- Taxonomy reclassification: none observed

- Scope changes: none observed

- Prevention mapping definitions: unchanged

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

Status: reinforced\
Signals:

- wallet_software_exploit; malware; session_hijacking

- prevention mappings related to key exposure and approvals

------------------------------------------------------------------------

**Why did connecting my wallet drain me? I thought connecting was
safe.**

Status: reinforced\
Signals:

- phishing; malicious site interaction patterns

- prevention mappings involving approval revocation and connection risk

------------------------------------------------------------------------

**I had strong 2FA. How was my account still abused?**

Status: reinforced\
Signals:

- malware; session_hijacking

- prevention mappings related to authentication limitations

------------------------------------------------------------------------

**What is token approval abuse, and how can it drain funds later?**

Status: reinforced\
Signals:

- approval-based compromise patterns observed

- prevention mappings related to approval revocation

------------------------------------------------------------------------

**What is "pay-to-withdraw," and why does it keep appearing?**

Status: reinforced\
Signals:

- crypto_wallet_scam; exchange_scam

- prevention mappings aligned with withdrawal fee patterns

------------------------------------------------------------------------

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

Status: reinforced\
Signals:

- crypto_wallet_scam; exchange_scam

- prevention mappings involving withdrawal fee refusal

------------------------------------------------------------------------

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

Status: reinforced\
Signals:

- crypto_wallet_scam dominance

- prevention mappings aligned with staged withdrawal blocking

------------------------------------------------------------------------

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

Status: reinforced\
Signals:

- social_engineering; phishing

- prevention mappings involving unsolicited contact

------------------------------------------------------------------------

**Why are recovery services contacting victims almost always scams?**

Status: reinforced\
Signals:

- multi-stage scam patterns observed

- prevention mappings involving repeated payment refusal

------------------------------------------------------------------------

**Why are physical letters, QR codes, and mailed notices used again?**

Status: absent\
Signals:

- no corresponding subtype or incident pattern observed in CW13

------------------------------------------------------------------------

**What is address poisoning, and why does it still work on large
transfers?**

Status: absent\
Signals:

- no address_poisoning_copy_paste subtype observed

------------------------------------------------------------------------

**Why do wallets sometimes show zero balance after restore?**

Status: absent\
Signals:

- no matching subtype or incident pattern observed

------------------------------------------------------------------------

**Why do wrong-network transfers become permanent losses even without a
scam?**

Status: reinforced\
Signals:

- wrong_network dominant within user_mistake

- prevention mappings aligned with network mismatch

------------------------------------------------------------------------

**Can crypto sent to the wrong address be recovered?**

Status: reinforced\
Signals:

- wrong_network and transfer error incidents

- prevention mappings aligned with transfer validation

------------------------------------------------------------------------

**What happens if I lose my seed phrase but still have wallet access?**

Status: reinforced\
Signals:

- seed_phrase_exposure; wallet compromise patterns

- prevention mappings aligned with key handling

------------------------------------------------------------------------

**Candidate FAQ Additions (CW13)**

- Why do fake presales allow deposits but never enable claiming or
  trading?\
  Signals:

  - token_launch_scam

  - prevention mappings related to platform verification and liquidity
    absence

------------------------------------------------------------------------

**Candidate FAQ Removals (CW13)**

none identified

------------------------------------------------------------------------

**Verdict (CW13)**

The evergreen FAQ remains broadly aligned with observed CW13 incident
mechanisms.\
One candidate addition is supported by recurring token launch scam
patterns.\
No removals are justified.\
This week establishes a valid baseline for FAQ signal alignment.
