**Defensive Coverage Gap Report --- CW13 2026**

**Purpose**

This report evaluates whether observed prevention failures in CW13 are
already addressed by the current CSF defensive corpus.\
This report is governance-only and non-public.

------------------------------------------------------------------------

**Inputs Declared (CW13)**

- incidents.csv (CW13)

- taxonomy_report.md (CW13)

- prevention_report.md (CW13)

- governance_notes.md (CW13)

- manifest.md (CW13)

Defensive canon sources (available and confirmed):

- How to Keep Your Crypto and Digital Assets Safe from Hackers (1st
  Edition, 2025)

- Crypto & Web3 Scams Prevention Guidebook (1st Edition, 2025)

- Crypto & Web3 User Mistakes Prevention Guidebook (1st Edition, 2025)

- The Three-Wallet Model (1st Edition, 2025)

- Practical Crypto & Web3 Safety Tools (canonical snapshot)

------------------------------------------------------------------------

**Coverage Assessment**

**Prevention Failure: Unverified platform interaction (fake platforms,
phishing sites)**

Coverage: covered\
Coverage Type: behavioral + tooling

Grounding:

- Scam guidebook explicitly addresses phishing, fake platforms, and
  impersonation patterns

- Safety tools reference includes domain verification and phishing
  detection tools

- Hacker guidebook outlines verification of URLs and communication
  channels

**Prevention Failure: Approval abuse and persistent wallet permissions**

Coverage: covered\
Coverage Type: tooling

Grounding:

- Safety tools reference includes approval auditing and revocation tools

- Scam guidebook addresses malicious smart contract interactions and
  approval misuse

------------------------------------------------------------------------

**Prevention Failure: Social engineering via unsolicited contact (DMs,
calls, impersonation)**

Coverage: covered\
Coverage Type: behavioral

Grounding:

- Scam guidebook details impersonation, vishing, and fake support flows

- Hacker guidebook outlines social engineering mechanics and recognition
  patterns

------------------------------------------------------------------------

**Prevention Failure: Weak account and authentication security**

Coverage: covered\
Coverage Type: behavioral + tooling

Grounding:

- Hacker guidebook includes strong password and authentication practices

- Safety tools reference includes 2FA and hardware security keys

------------------------------------------------------------------------

**Prevention Failure: Asset exposure from single-wallet usage (no
compartmentalization)**

Coverage: covered\
Coverage Type: structural

Grounding:

- Three-Wallet Model defines wallet segmentation to reduce single point
  of failure

- User mistakes guidebook highlights risks of all-in-one wallet setups

------------------------------------------------------------------------

**Prevention Failure: Incorrect network or transfer handling**

Coverage: covered\
Coverage Type: behavioral

Grounding:

- User mistakes guidebook addresses transaction errors and irreversible
  transfers

- Emphasis on verification before sending assets

------------------------------------------------------------------------

**Prevention Failure: Lack of approval review and ongoing wallet
maintenance**

Coverage: covered\
Coverage Type: behavioral + tooling

Grounding:

- Safety tools reference includes approval management tools

- User mistakes guidebook defines ongoing wallet review and maintenance
  practices

------------------------------------------------------------------------

**Prevention Failure: Exposure of sensitive credentials or key
material**

Coverage: covered\
Coverage Type: behavioral + structural

Grounding:

- Hacker guidebook explains risks of key exposure and malware

- Scam guidebook reinforces never sharing sensitive credentials

- Safety tools include hardware wallets and offline storage

------------------------------------------------------------------------

**Summary**

All dominant prevention failure points observed in CW13 are addressed
within the current CSF defensive canon.

Coverage spans:

- behavioral controls (verification, communication handling)

- tooling controls (approval management, authentication, detection
  tools)

- structural controls (wallet segmentation via the Three-Wallet Model)

No uncovered or partially covered prevention failures were identified
based on CW13 inputs and available canonical materials.
