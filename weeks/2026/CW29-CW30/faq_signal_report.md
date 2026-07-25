# FAQ Signal Report — CW29 + CW30 2026

## Purpose

This report assesses whether the current evergreen FAQ remains aligned with loss mechanisms observed in the current weekly package.

This report is non-public and governance-only.

## Inputs Declared

- incidents.csv — CW29 + CW30 2026
- taxonomy_report.md — CW29 + CW30 2026
- prevention_report.md — CW29 + CW30 2026
- governance_notes.md — CW29 + CW30 2026
- manifest.md — CW29 + CW30 2026
- README.md — CW29 + CW30 2026
- Evergreen FAQ corpus — revision dated 05 July 2026

Report type: Bootstrap

## Governance Check

- Taxonomy reclassification occurred: No.
- Scope changes occurred: No.
- Prevention mapping definitions changed: No.

## FAQ Signal Coverage Assessment

### If I never shared my seed phrase, how did funds still leave my wallet?

**Status:** reinforced

**Current-week signals:**
- Wallet losses occurred through malware, fake applications, session abuse, malicious approvals, and address replacement without seed phrase disclosure.
- Current-week records include unauthorized wallet or account execution where prior access or a compromised environment enabled the transfer.

**Dominant anchors:**
- Taxonomy labels: malware, session_hijacking, fake_app_or_extension_hack, smart_contract_scam
- Prevention failure mappings: Never share recovery phrases or private keys, Limit browser extensions and keep browsers updated, Revoke token approvals and review permissions regularly

### Why did connecting my wallet drain me? I thought connecting was safe.

**Status:** reinforced

**Current-week signals:**
- A current-week smart-contract scam involved a fraudulent website and wallet interaction.
- The prevention report includes approval review and platform legitimacy as mapped controls.

**Dominant anchors:**
- Taxonomy labels: smart_contract_scam
- Prevention failure mappings: Revoke token approvals and review permissions regularly, Verify platform legitimacy before use

### I had strong 2FA. How was my account still abused?

**Status:** reinforced

**Current-week signals:**
- A current-week gaming account was compromised despite two-factor authentication.
- The attacker acted through the compromised session and connected an external withdrawal wallet.

**Dominant anchors:**
- Taxonomy labels: session_hijacking
- Prevention failure mappings: Enable strong authentication and account security

### What is token approval abuse, and how can it drain funds later?

**Status:** reinforced

**Current-week signals:**
- A current-week smart-contract scam involved a fraudulent wallet interaction and unauthorized token movement.
- Approval review and permission revocation were retained as mapped prevention controls.

**Dominant anchors:**
- Taxonomy labels: smart_contract_scam
- Prevention failure mappings: Revoke token approvals and review permissions regularly

### Can a scammer steal my crypto just by knowing my wallet address?

**Status:** reinforced

**Current-week signals:**
- Current-week incidents distinguish public-address visibility from the separate actions that enabled loss.
- Observed losses required address substitution, social engineering, malicious software, or transaction authorization rather than knowledge of the address alone.

**Dominant anchors:**
- Taxonomy labels: crypto_wallet_scam, social_engineering, malware
- Prevention failure mappings: Confirm network and address compatibility before transfers, Verify platform legitimacy before use

### Can someone hack my wallet if they know my public address?

**Status:** reinforced

**Current-week signals:**
- Current-week wallet-address incidents involved additional mechanisms such as address poisoning, clipboard or note replacement, impersonation, or unauthorized access.
- No current-week record attributes wallet control to public-address knowledge alone.

**Dominant anchors:**
- Taxonomy labels: crypto_wallet_scam, social_engineering, wallet_compromise
- Prevention failure mappings: Confirm network and address compatibility before transfers, Never share recovery phrases or private keys

### What is “pay-to-withdraw,” and why does it keep appearing?

**Status:** reinforced

**Current-week signals:**
- Current-week exchange and social-engineering incidents repeatedly used fabricated balances and withdrawal blocks.
- Additional payments were framed as conditions for releasing displayed funds.

**Dominant anchors:**
- Taxonomy labels: exchange_scam, social_engineering
- Prevention failure mappings: Do not pay fees to unlock withdrawals, Verify platform legitimacy before use

### Are tax, AML, insurance, or verification fees before withdrawal ever legitimate?

**Status:** reinforced

**Current-week signals:**
- Current-week incidents used compliance, verification, recovery, and withdrawal narratives to demand additional payments.
- The prevention report maps these mechanisms to refusal of unlock fees.

**Dominant anchors:**
- Taxonomy labels: exchange_scam, social_engineering
- Prevention failure mappings: Do not pay fees to unlock withdrawals

### If a platform shows profits, why can’t I just withdraw smaller amounts?

**Status:** reinforced

**Current-week signals:**
- A current-week fraudulent platform allowed small withdrawals before blocking larger withdrawals.
- Other records displayed fabricated profits while introducing new payment conditions.

**Dominant anchors:**
- Taxonomy labels: exchange_scam
- Prevention failure mappings: Do not pay fees to unlock withdrawals, Verify platform legitimacy before use

### Why does the platform keep asking for another payment before I can withdraw my funds?

**Status:** reinforced

**Current-week signals:**
- Repeated-payment extraction appears across current-week exchange scams, recovery scams, and task schemes.
- Payment conditions changed after earlier deposits or apparent account gains.

**Dominant anchors:**
- Taxonomy labels: exchange_scam, social_engineering, job_scam
- Prevention failure mappings: Do not pay fees to unlock withdrawals, Verify platform legitimacy before use

### If a caller knows my details and claims to be support, doesn’t that prove it’s real?

**Status:** reinforced

**Current-week signals:**
- Current-week impersonation incidents used exchange, verification-team, regulator, and assistance narratives.
- Possession of personal or transaction details was part of the credibility mechanism rather than proof of authority.

**Dominant anchors:**
- Taxonomy labels: social_engineering, phishing
- Prevention failure mappings: Avoid unsolicited messages calls and DMs, Verify platform legitimacy before use

### Why are recovery services contacting victims almost always scams?

**Status:** reinforced

**Current-week signals:**
- Current-week recovery scammers contacted people after earlier losses and claimed that funds had been located or recovered.
- Release of the supposed recovered assets depended on additional payment.

**Dominant anchors:**
- Taxonomy labels: social_engineering
- Prevention failure mappings: Do not pay fees to unlock withdrawals, Avoid unsolicited messages calls and DMs

### Why are physical letters, QR codes, and mailed notices used again?

**Status:** reinforced

**Current-week signals:**
- Multiple current-week phishing records used physical letters impersonating wallet vendors or exchanges.
- The letters directed recipients toward QR codes, links, or recovery-phrase capture flows.

**Dominant anchors:**
- Taxonomy labels: phishing
- Prevention failure mappings: Verify platform legitimacy before use, Never share recovery phrases or private keys

### What is address poisoning, and why does it still work on large transfers?

**Status:** reinforced

**Current-week signals:**
- A current-week incident used tiny transfers from lookalike addresses to poison transaction history.
- Another current-week loss involved a lookalike address selected for a large transfer.

**Dominant anchors:**
- Taxonomy labels: crypto_wallet_scam, wrong_address
- Prevention failure mappings: Confirm network and address compatibility before transfers, Test transactions with small amounts first

### Why do wallets sometimes show zero balance after restore?

**Status:** weakened

**Current-week signals:**
- Current-week lost-access records support recovery-context and wallet-access risk.
- The current-week inputs do not directly document a confirmed zero-balance-after-restore mechanism.

**Dominant anchors:**
- Taxonomy labels: lost_wallet_access
- Prevention failure mappings: Never share recovery phrases or private keys

### Why do wrong-network transfers become permanent losses even without a scam?

**Status:** reinforced

**Current-week signals:**
- Multiple current-week user-error records involved tokens sent over unsupported or mismatched networks.
- Transactions succeeded on-chain while the receiving service could not credit the intended asset.

**Dominant anchors:**
- Taxonomy labels: wrong_network
- Prevention failure mappings: Confirm network and address compatibility before transfers, Test transactions with small amounts first

### Can crypto sent to the wrong address be recovered?

**Status:** reinforced

**Current-week signals:**
- Current-week wrong-address incidents involved valid transfers to unintended or lookalike destinations.
- Recovery depended on recipient or platform control rather than reversal by the network.

**Dominant anchors:**
- Taxonomy labels: wrong_address, crypto_wallet_scam
- Prevention failure mappings: Confirm network and address compatibility before transfers, Test transactions with small amounts first

### What happens if I lose my seed phrase but still have wallet access?

**Status:** reinforced

**Current-week signals:**
- Current-week lost-wallet-access records include users who retained partial or temporary wallet access while recovery capability was missing or uncertain.
- The records preserve the distinction between current access and recoverable custody.

**Dominant anchors:**
- Taxonomy labels: lost_wallet_access
- Prevention failure mappings: Never share recovery phrases or private keys

## Candidate FAQ Additions — CW29 + CW30 2026

### Why do fake task jobs require deposits before earnings can be released?

- Recurring within the current weekly dataset.
- Visible across multiple job-scam records involving task platforms and repeated deposits.
- Stable taxonomy anchor: job_scam.
- Prevention failure anchors: Verify platform legitimacy before use; Do not pay fees to unlock withdrawals.

## Candidate FAQ Removals — CW29 + CW30 2026

None identified.

## Verdict — CW29 + CW30 2026

The evergreen FAQ remains aligned with the current weekly package.

One candidate addition is supported.

No candidate removals are supported.

This bootstrap report establishes the initial FAQ signal baseline.