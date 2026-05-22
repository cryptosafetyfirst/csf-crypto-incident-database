\# FAQ Signal Report --- CW21 2026

\## Purpose

This report evaluates whether the current evergreen FAQ coverage remains
aligned with recurring loss mechanisms observed during the CW21 2026
reporting cycle.

This report is governance-only and non-public.

\-\--

\## Inputs Declared

Artifacts used for this review:

\- \`incidents.csv\`

\- \`manifest.md\`

\- \`taxonomy_report.md\`

\- \`prevention_report.md\`

\- \`governance_notes.md\`

\- \`README.md\`

Reference corpus used:

\- Current evergreen Crypto Loss FAQ page

Report mode:

\- Bootstrap report

\-\--

\## Governance Check

\- No taxonomy reclassification performed

\- No scope changes identified

\- No prevention mapping definition changes identified

\-\--

\## FAQ Signal Coverage Assessment

\### If I never shared my seed phrase, how did funds still leave my
wallet?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- phishing

\- social_engineering_hack

\- execution authority misuse

\- approval-related transaction behavior

\*\*Dominant Anchors\*\*

\- taxonomy: phishing, social_engineering_hack

\- prevention mappings: account security, legitimacy verification

\-\--

\### Why did connecting my wallet drain me? I thought connecting was
safe.

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- phishing-driven wallet interaction

\- malicious interaction flow patterns

\- transaction approval misuse signals

\*\*Dominant Anchors\*\*

\- taxonomy: phishing

\- prevention mappings: legitimacy verification

\-\--

\### I had strong 2FA. How was my account still abused?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- compromised-session style behavior

\- social engineering assisted compromise

\*\*Dominant Anchors\*\*

\- taxonomy: social_engineering_hack

\- prevention mappings: strong authentication and account security

\-\--

\### What is token approval abuse, and how can it drain funds later?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- approval persistence behavior

\- authorization misuse mechanisms

\*\*Dominant Anchors\*\*

\- taxonomy: phishing

\- prevention mappings: revoke approvals and review permissions
regularly

\-\--

\### What is "pay-to-withdraw," and why does it keep appearing?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- fake exchange behavior

\- withdrawal fee narratives

\- staged payment escalation patterns

\*\*Dominant Anchors\*\*

\- taxonomy: exchange_scam

\- prevention mappings: do not pay fees to unlock withdrawals

\-\--

\### Are tax, AML, insurance, or verification fees before withdrawal
ever legitimate?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- compliance-fee extraction narratives

\- fake custody behavior

\*\*Dominant Anchors\*\*

\- taxonomy: exchange_scam

\- prevention mappings: do not pay fees to unlock withdrawals

\-\--

\### If a platform shows profits, why can't I just withdraw smaller
amounts?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- staged trust-building withdrawals

\- escalating withdrawal barriers

\*\*Dominant Anchors\*\*

\- taxonomy: exchange_scam

\- prevention mappings: verify platform legitimacy before use

\-\--

\### If a caller knows my details and claims to be support, doesn't that
prove it's real?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- impersonation behavior

\- phishing-assisted trust exploitation

\*\*Dominant Anchors\*\*

\- taxonomy: phishing, social_engineering

\- prevention mappings: avoid unsolicited messages, calls, and DMs

\-\--

\### Why are recovery services contacting victims almost always scams?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- recovery scam behavior

\- secondary extraction attempts

\*\*Dominant Anchors\*\*

\- taxonomy: recovery_scam

\- prevention mappings: verify platform legitimacy before use

\-\--

\### Why are physical letters, QR codes, and mailed notices used again?

\*\*Status:\*\* absent

\*\*CW21 Signals\*\*

\- no directly observed mailed impersonation mechanism identified

\*\*Dominant Anchors\*\*

\- taxonomy: none dominant

\- prevention mappings: none dominant

\-\--

\### What is address poisoning, and why does it still work on large
transfers?

\*\*Status:\*\* weakened

\*\*CW21 Signals\*\*

\- transfer validation failures present

\- no dominant poisoning-specific mechanism identified

\*\*Dominant Anchors\*\*

\- taxonomy: wrong_address

\- prevention mappings: confirm network and address compatibility before
transfers

\-\--

\### Why do wallets sometimes show zero balance after restore?

\*\*Status:\*\* weakened

\*\*CW21 Signals\*\*

\- wallet access and recovery confusion signals present

\- no dominant derivation-path pattern identified

\*\*Dominant Anchors\*\*

\- taxonomy: lost_wallet_access

\- prevention mappings: none dominant

\-\--

\### Why do wrong-network transfers become permanent losses even without
a scam?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- recurring wrong-network transfer behavior

\- compatibility validation failures

\*\*Dominant Anchors\*\*

\- taxonomy: wrong_network

\- prevention mappings: confirm network and address compatibility before
transfers

\-\--

\### Can crypto sent to the wrong address be recovered?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- irreversible transfer behavior

\- destination validation failures

\*\*Dominant Anchors\*\*

\- taxonomy: wrong_address

\- prevention mappings: confirm network and address compatibility before
transfers

\-\--

\### What happens if I lose my seed phrase but still have wallet access?

\*\*Status:\*\* reinforced

\*\*CW21 Signals\*\*

\- recoverability failures

\- wallet access continuity issues

\*\*Dominant Anchors\*\*

\- taxonomy: lost_wallet_access

\- prevention mappings: hardware wallet usage and backup integrity
practices

\-\--

\## Candidate FAQ Additions

\### Candidate: Why do fake exchanges continue to succeed even when the
interface looks professional?

\*\*Justification Signals\*\*

\- recurring exchange scam patterns

\- legitimacy confusion

\- repeated fake custody narratives

\*\*Dominant Anchors\*\*

\- taxonomy: exchange_scam

\- prevention mappings: verify platform legitimacy before use

\-\--

\## Candidate FAQ Removals

none identified

\-\--

\## Verdict

The evergreen FAQ remains materially aligned with CW21 2026 observed
loss mechanisms.

Most existing FAQ entries were reinforced by recurring phishing,
exchange scam, social engineering, and transfer validation behaviors
observed in the current reporting cycle.

One FAQ entry was assessed as absent for this cycle, while two entries
were assessed as weakened but still relevant to the broader loss
landscape.

One candidate FAQ addition was identified relating to fake exchange
legitimacy narratives.

This report establishes a valid CW21 2026 FAQ alignment baseline.
