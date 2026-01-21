\# CW02 Prevention Action Normalization Report

\*\*Stage:\*\* Prevention Action Normalization

\*\*Status:\*\* Hardened (Non-breaking)

\*\*Scope:\*\* CW02 Crypto & Web3 Incident Dataset

\*\*Total Incidents Analyzed:\*\* 68

\-\--

\## Purpose

This report normalizes prevention guidance across real-world crypto and
Web3 loss incidents observed during \*\*CW02\*\* into a fixed,
comparable set of prevention actions.

Its purpose is not to expand advice, but to \*\*measure where losses
were preventable\*\*, where prevention guidance was ambiguous or
missing, and which decision points consistently preceded loss.

All mappings are constrained to a \*\*locked prevention action set\*\*
to ensure longitudinal consistency across weeks.

\-\--

\## Methodology Summary

\- Prevention actions were mapped \*\*only from the \`prevention\`
field\*\* of each CW02 incident record.

\- \`summary\` and \`user_mistake\` fields were used \*\*only to clarify
intent\*\*, never to invent actions.

\- Incidents with vague, narrative, or unmappable prevention text were
\*\*explicitly excluded from forced classification\*\*.

\- Incidents with \`classification_warning ≠ none\` were mapped
conservatively.

\- Each incident may map to multiple prevention actions, but only once
per action.

\-\--

\## Data Integrity Notes

\- All 68 CW02 records contained prevention text.

\- \*\*32 incidents contained prevention text that was present but not
safely mappable\*\* to the locked action set.

\- \*\*13 incidents included classification warnings\*\*, limiting
confident attribution.

\- No duplicate or malformed entry numbers were detected.

This means measured prevention coverage represents a \*\*lower
bound\*\*, not an overstatement.

\-\--

\## Normalized Prevention Actions --- Coverage Table (CW02)

\| Prevention Action \| Count \| % of Total \|

\|\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\-\--\|\-\-\-\-\--:\|\-\-\-\-\-\-\-\-\-\--:\|

\| Avoid unsolicited messages, calls, and DMs \| 24 \| 35.3% \|

\| Verify platform legitimacy before use \| 10 \| 14.7% \|

\| Do not pay fees to unlock withdrawals \| 5 \| 7.4% \|

\| Confirm network and address compatibility before transfers \| 3 \|
4.4% \|

\| Maintain complete transaction and tax records \| 2 \| 2.9% \|

\| Never share recovery phrases or private keys \| 2 \| 2.9% \|

\| Use hardware wallets for long-term storage \| 1 \| 1.5% \|

\| Enable strong authentication and account security \| 1 \| 1.5% \|

\| Test transactions with small amounts first \| 0 \| 0.0% \|

\| Limit browser extensions and keep browsers updated \| 0 \| 0.0% \|

\| Revoke token approvals and review permissions regularly \| 0 \| 0.0%
\|

\| Minimize public exposure of crypto holdings \| 0 \| 0.0% \|

Percentages are based on total CW02 incidents (n=68).

Zero-count actions are included intentionally for longitudinal tracking.

\-\--

\## Key Findings (CW02)

\### 1. Social-Channel Exposure Is the Dominant Preventable Entry Point

The most frequently mapped prevention action in CW02 is \*\*avoiding
unsolicited messages, calls, and DMs\*\*, appearing in over one-third of
incidents.

This aligns with CW02's dominant loss mechanisms:

\- fake exchanges and dashboards

\- pig-butchering investment funnels

\- impersonation and recovery scams

Losses typically began \*\*before any technical interaction\*\*, at the
moment a private channel was trusted.

\-\--

\### 2. Platform Legitimacy Verification Is the Second Major Failure
Point

Failure to \*\*verify platform legitimacy before use\*\* appears in
nearly 15% of CW02 incidents.

Victims validated:

\- interfaces

\- branding

\- support narratives

instead of verifying custody, history, or on-chain reality.

This supports treating \*\*manufactured legitimacy\*\* as a primary
threat class.

\-\--

\### 3. Pay-to-Withdraw Demands Are a Clear, Repeatable Extraction
Mechanism

Although smaller in raw count, \*\*pay-to-withdraw schemes\*\* in CW02
were:

\- unambiguous

\- repeatable

\- never resolved successfully

Each instance involved escalating deposits framed as tax, AML,
risk-control, or verification requirements.

\-\--

\### 4. Significant Gaps in Explicit Prevention Language

Several prevention actions registered \*\*zero coverage\*\*, including:

\- limiting browser extensions

\- reviewing token approvals

\- test transactions

\- minimizing public exposure

This does not imply irrelevance --- it indicates that \*\*incident-level
prevention narratives rarely name these actions explicitly\*\*, even
when tooling or endpoint compromise was involved.

\-\--

\### 5. Vague Prevention Text Is a Structural Limitation

Nearly half of CW02 incidents included prevention text that was:

\- narrative rather than actionable

\- cautionary without a clear decision point

\- incompatible with the locked action set

This limits retrospective measurability and reinforces the need for
\*\*standardized prevention phrasing\*\* in future datasets.

\-\--

\## Top Prevention Actions by Coverage (CW02)

Ranked by incident coverage:

1\. \*\*Avoid unsolicited messages, calls, and DMs\*\*

2\. \*\*Verify platform legitimacy before use\*\*

3\. \*\*Do not pay fees to unlock withdrawals\*\*

\*\*Combined coverage:\*\* 44.1% of CW02 incidents

Even with conservative mapping, fewer than half of incidents explicitly
named their earliest preventable decision point.

\-\--

\## Interpretation (Non-Speculative)

\- CW02 losses cluster around \*\*trust and context failures\*\*, not
cryptographic or protocol failure.

\- When prevention guidance is explicit, it is \*\*simple and
behavioral\*\*, not technical.

\- Absence of explicit prevention language is itself a recurring failure
mode.

This report does not add new advice.

It documents where CW02 prevention signals were \*\*visible, weak, or
missing\*\*.

\-\--

\## Role in the Weekly Series

This CW02 normalization report serves as:

\- the \*\*baseline prevention distribution\*\* for the series

\- a reference point for CW03+ prevention deltas

\- a consistency anchor for prevention percentages cited in weekly
digests

Future weeks should be compared against this distribution to identify:

\- shifts in dominant failure points

\- emergence of new entry vectors

\- improvements (or regressions) in prevention clarity

\-\--

\## Bottom Line

CW02 shows that most losses were \*\*preventable at the first
interaction\*\*, not the final transaction.

Where prevention guidance was explicit, it was simple.

Where losses compounded, prevention language was vague or absent.

Normalization makes that gap measurable.
