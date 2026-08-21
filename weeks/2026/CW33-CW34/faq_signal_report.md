**FAQ Signal Report --- CW33 + CW34 2026**

**Purpose**

This report assesses whether the current evergreen Crypto Loss FAQ
remains aligned with loss mechanisms observed in the CW33 + CW34 2026
weekly incident dataset.

This report is **non-public and governance-only**. It does not create or
modify incident classifications, prevention mappings, or canonical
intelligence.

**Inputs Declared**

- incidents.csv --- CW33 + CW34 2026

- taxonomy_report.md --- CW33 + CW34 2026

- prevention_report.md --- CW33 + CW34 2026

- governance_notes.md --- CW33 + CW34 2026

- manifest.md --- CW33 + CW34 2026

- README.md --- CW33 + CW34 2026

- Current evergreen FAQ corpus --- **Crypto Loss FAQ --- Common
  Questions After Real-World Web3 Incidents**

The supplied weekly artifacts consistently identify the reporting period
as CW33 + CW34 2026.

**Report type:** Bootstrap.

The current evergreen FAQ corpus is used as the baseline FAQ question
set. No prior FAQ signal report is used as an input. The corpus
organizes existing questions around technical compromise and wallet
drains, deception-driven losses, and irreversible user errors.

**Governance Check**

**Taxonomy reclassification:** Not established by the supplied
governance inputs. No explicit confirmation that no reclassification
occurred is available.

**Scope changes:** Not established by the supplied governance inputs. No
explicit confirmation that no scope change occurred is available.

**Prevention mapping definition changes:** No change is declared in the
supplied prevention output. Prevention mappings use the fixed prevention
action set and conservative mapping methodology described for the
current dataset.

The governance inputs explicitly leave dataset-integrity confirmation
undeclared because the required conditions were not all explicitly
confirmed.

Classification ambiguity and prevention mapping friction are present.
Governance notes identify classification uncertainty and prevention
guidance that could not always be mapped conservatively to the available
prevention action set.

**FAQ Signal Coverage Assessment**

**If I never shared my seed phrase, how did funds still leave my
wallet?**

**Status:** reinforced

**CW33 + CW34 signals:**

- wallet drains occurred without a confirmed seed-phrase disclosure
  mechanism

- wallet_software_exploit is represented in the weekly taxonomy

- social_engineering_hack, fake_app_or_extension_hack, and spyware are
  also represented

- several wallet-drain records lack a confirmed initial compromise
  vector

**Dominant anchors:**

- Taxonomy: wallet_software_exploit, social_engineering_hack,
  fake_app_or_extension_hack, spyware

- Prevention: wallet/software legitimacy and recovery-phrase protection
  signals

The weekly taxonomy records five wallet_software_exploit incidents and
explicitly cautions that several lack a confirmed initial compromise
vector.

**Why did connecting my wallet drain me? I thought connecting was
safe.**

**Status:** absent

**CW33 + CW34 signals:**

- no stable current-week taxonomy subtype specifically identifies wallet
  connection or malicious approval as the loss mechanism

- no mapped prevention coverage exists for regular token-approval review
  or revocation

**Dominant anchors:**

- Taxonomy: none directly supporting the mechanism

- Prevention: Revoke token approvals and review permissions regularly
  --- no mapped incidents

The current prevention report records zero mappings for token-approval
and permission review.

**I had strong 2FA. How was my account still abused?**

**Status:** absent

**CW33 + CW34 signals:**

- no current-week stable subtype specifically identifies 2FA bypass or
  account-authentication failure

- strong authentication and account security has no mapped prevention
  incidents

**Dominant anchors:**

- Taxonomy: none directly supporting the mechanism

- Prevention: Enable strong authentication and account security --- no
  mapped incidents

The prevention report records zero current-week mappings for this
prevention action.

**What is token approval abuse, and how can it drain funds later?**

**Status:** absent

**CW33 + CW34 signals:**

- no token-approval-specific subtype is represented

- no prevention mappings relate to reviewing or revoking token approvals

**Dominant anchors:**

- Taxonomy: none directly supporting approval abuse

- Prevention: Revoke token approvals and review permissions regularly
  --- no mapped incidents

**Can a scammer steal my crypto just by knowing my wallet address?**

**Status:** absent

**CW33 + CW34 signals:**

- no current-week loss mechanism attributes theft to knowledge of a
  public wallet address alone

- no corresponding stable taxonomy subtype is represented

**Dominant anchors:**

- Taxonomy: none

- Prevention: none directly mapped

**Can someone hack my wallet if they know my public address?**

**Status:** absent

**CW33 + CW34 signals:**

- no incident classification identifies public-address knowledge as the
  compromise mechanism

- current hack classifications concern wallet/software compromise,
  social engineering, fake applications/extensions, and spyware

**Dominant anchors:**

- Taxonomy: wallet_software_exploit, social_engineering_hack,
  fake_app_or_extension_hack, spyware

- Prevention: none directly mapped to public-address knowledge

**What is "pay-to-withdraw," and why does it keep appearing?**

**Status:** reinforced

**CW33 + CW34 signals:**

- exchange_scam is the largest taxonomy subtype

- fraudulent platforms repeatedly involve withdrawal restrictions and
  additional payments

- withdrawal-fee avoidance is one of the most frequently mapped
  prevention failures

**Dominant anchors:**

- Taxonomy: exchange_scam

- Prevention: Do not pay fees to unlock withdrawals

exchange_scam accounts for 17 incidents, with the taxonomy report
explicitly identifying withdrawal restrictions and additional tax or
verification payments among the recurring mechanisms.

**Are tax, AML, insurance, or verification fees before withdrawal ever
legitimate?**

**Status:** reinforced

**CW33 + CW34 signals:**

- withdrawal-related tax, verification, and additional-payment demands
  occur within current-week fraudulent-platform incidents

- withdrawal-fee avoidance maps across multiple incidents

**Dominant anchors:**

- Taxonomy: exchange_scam

- Prevention: Do not pay fees to unlock withdrawals

The prevention report maps this action to eight incidents.

**If a platform shows profits, why can't I just withdraw smaller
amounts?**

**Status:** reinforced

**CW33 + CW34 signals:**

- fraudulent investment and trading platforms displaying fabricated
  balances or profits recur within exchange_scam

- withdrawal restrictions remain explicitly represented

- platform legitimacy verification is the most frequently mapped
  prevention action

**Dominant anchors:**

- Taxonomy: exchange_scam

- Prevention: Verify platform legitimacy before use, Do not pay fees to
  unlock withdrawals

**Why does the platform keep asking for another payment before I can
withdraw my funds?**

**Status:** reinforced

**CW33 + CW34 signals:**

- repeated additional-payment demands occur in fraudulent platform cases

- withdrawal restrictions and verification/payment demands are
  explicitly represented

- withdrawal-fee avoidance remains strongly mapped

**Dominant anchors:**

- Taxonomy: exchange_scam

- Prevention: Do not pay fees to unlock withdrawals, Verify platform
  legitimacy before use

Platform verification is mapped to 21 incidents and withdrawal-fee
avoidance to eight.

**If a caller knows my details and claims to be support, doesn't that
prove it's real?**

**Status:** reinforced

**CW33 + CW34 signals:**

- impersonation and unsolicited-contact incidents are represented within
  social_engineering

- current incidents include authority and support impersonation

- avoidance of unsolicited messages, calls, and DMs is repeatedly mapped

- minimizing public exposure of crypto holdings is also represented

**Dominant anchors:**

- Taxonomy: social_engineering

- Prevention: Avoid unsolicited messages calls and DMs, Minimize public
  exposure of crypto holdings

social_engineering accounts for 10 incidents, while unsolicited-contact
avoidance maps to six incidents.

**Why are recovery services contacting victims almost always scams?**

**Status:** reinforced

**CW33 + CW34 signals:**

- recovery-related social-engineering cases occur in the weekly incident
  dataset

- unsolicited recovery approaches and upfront payment demands are
  represented

- these cases remain within the stable social_engineering taxonomy

**Dominant anchors:**

- Taxonomy: social_engineering

- Prevention: unsolicited-contact avoidance and platform/service
  legitimacy verification

**Why are physical letters, QR codes, and mailed notices used again?**

**Status:** absent

**CW33 + CW34 signals:**

- no stable current-week subtype establishes physical mail as a
  recurring loss mechanism

- isolated QR-code use does not establish recurring physical-letter or
  mailed-notice behavior for the current reporting period

**Dominant anchors:**

- Taxonomy: none specifically supporting physical-mail delivery

- Prevention: none specifically mapped

**What is address poisoning, and why does it still work on large
transfers?**

**Status:** absent

**CW33 + CW34 signals:**

- address poisoning is not represented as a stable current-week taxonomy
  subtype

- wrong-address incidents exist, but the weekly taxonomy does not
  establish address poisoning as their mechanism

**Dominant anchors:**

- Taxonomy: wrong_address does not independently establish address
  poisoning

- Prevention: full recipient-address verification and small test
  transactions are represented indirectly through the user-error cluster

**Why do wallets sometimes show zero balance after restore?**

**Status:** absent

**CW33 + CW34 signals:**

- lost_wallet_access is represented

- current-week taxonomy does not establish derivation-path,
  account-index, or post-restore zero-balance behavior as a recurring
  mechanism

**Dominant anchors:**

- Taxonomy: lost_wallet_access

- Prevention: no stable normalized action directly maps to post-restore
  zero-balance diagnosis

lost_wallet_access accounts for three current-week incidents, but the
taxonomy does not establish the more specific zero-balance-after-restore
mechanism.

**Why do wrong-network transfers become permanent losses even without a
scam?**

**Status:** reinforced

**CW33 + CW34 signals:**

- wrong_network is the largest user-mistake subtype

- multiple cases concern incomplete asset-and-network compatibility

- network and address compatibility is one of the highest mapped
  prevention failures

**Dominant anchors:**

- Taxonomy: wrong_network

- Prevention: Confirm network and address compatibility before
  transfers, Test transactions with small amounts first

wrong_network accounts for six incidents and half of all user mistakes.
The report specifically identifies cases where the blockchain was
supported but the particular asset on that blockchain was not.

**Can crypto sent to the wrong address be recovered?**

**Status:** reinforced

**CW33 + CW34 signals:**

- wrong_address is represented in the current dataset

- transfer-execution errors remain a defined user-mistake cluster

- network/address compatibility and test transactions are mapped
  prevention failures

**Dominant anchors:**

- Taxonomy: wrong_address

- Prevention: Confirm network and address compatibility before
  transfers, Test transactions with small amounts first

The weekly taxonomy records two wrong_address incidents. Together,
wrong_network and wrong_address account for eight of the twelve
user-mistake incidents.

**What happens if I lose my seed phrase but still have wallet access?**

**Status:** reinforced

**CW33 + CW34 signals:**

- lost_wallet_access remains represented

- current incidents include failures involving unavailable recovery
  information

- recovery and access continuity remain observable within the
  user-mistake dataset

**Dominant anchors:**

- Taxonomy: lost_wallet_access

- Prevention: no dedicated normalized recovery-backup action in the
  current fixed prevention set

**Candidate FAQ Additions**

**Why can a crypto deposit fail even when the receiving platform
supports that blockchain?**

**CW33 + CW34 basis:**

- recurring within the reporting period

- directly represented by multiple wrong_network incidents

- stable taxonomy anchor: wrong_network

- tied to the recurring misunderstanding that blockchain support does
  not necessarily mean that every token on that blockchain is supported

The taxonomy report explicitly identifies this distinction: several
cases involved receiving platforms that supported the blockchain but not
the specific asset on that blockchain.

**Prevention anchors:**

- Confirm network and address compatibility before transfers

- Test transactions with small amounts first

**Can installing software or a browser extension during a fake
recruitment process compromise my crypto?**

**CW33 + CW34 basis:**

- malicious software/extension installation occurs repeatedly in the
  current dataset

- job_scam is represented as a stable taxonomy subtype

- fake_app_or_extension_hack is also represented

- the mechanism is tied to a preventable misunderstanding around
  software installation and authenticity

**Taxonomy anchors:**

- job_scam

- fake_app_or_extension_hack

**Prevention anchors:**

- Limit browser extensions and keep browsers updated

- platform/software legitimacy verification

job_scam appears twice in the current taxonomy and
fake_app_or_extension_hack is separately represented within hack
classifications.

**Candidate FAQ Removals**

**none identified**

Several existing FAQ mechanisms are absent from the current reporting
period, but current-week absence alone does not establish that those
mechanisms no longer appear in the incident system. The supplied inputs
therefore do not support a removal determination.

**Verdict**

The evergreen FAQ remains **materially aligned with CW33 + CW34 2026**.

Current-week evidence reinforces major existing FAQ coverage concerning:

- fraudulent platforms and pay-to-withdraw mechanisms

- fabricated withdrawal requirements

- support and authority impersonation

- recovery-service scams

- wallet drains without a confirmed seed-phrase disclosure mechanism

- wrong-network transfers

- wrong-address transfers

- loss of wallet recovery access

Current-week evidence does not reinforce several existing questions
concerning token approval abuse, 2FA bypass, public-address
misconceptions, physical-mail attacks, address poisoning, or
post-restore zero balances. Their absence in this reporting period does
not independently justify removal.

Two candidate additions are supported by the current reporting-period
inputs:

- **Why can a crypto deposit fail even when the receiving platform
  supports that blockchain?**

- **Can installing software or a browser extension during a fake
  recruitment process compromise my crypto?**

No FAQ removals are supported.

**CW33 + CW34 2026 establishes the bootstrap baseline for subsequent FAQ
signal assessment.**
