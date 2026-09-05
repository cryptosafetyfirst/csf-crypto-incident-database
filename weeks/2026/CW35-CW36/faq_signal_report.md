**FAQ Signal Report --- CW35 + CW36 2026**

This report assesses whether the current evergreen Crypto Loss FAQ
remains aligned with loss mechanisms observed in the current weekly
package.

This report is **non-public and governance-only**.

**Inputs Declared --- CW35 + CW36 2026**

- incidents.csv --- current weekly incident dataset.

- taxonomy_report.md --- current taxonomy analytical output.

- prevention_report.md --- current prevention analytical output.

- governance_notes.md --- current governance observations.

- manifest.md --- current weekly scope anchor.

- README.md --- current weekly package orientation.

- Current evergreen FAQ corpus --- Evergreen_FAQ_rev05JUL2026.

The manifest identifies the package as **CW35 + CW36 2026**.

This is a **bootstrap report**. No prior FAQ signal report is used as an
input.

The current evergreen corpus contains questions covering technical
compromise and wallet drains, deception-driven losses, and irreversible
user errors.

**Governance Check**

- **Taxonomy reclassification occurred:** no.

- **Scope changes occurred:** no.

- **Prevention mapping definitions changed:** no.

The weekly governance record explicitly confirms no reclassification, no
scope changes, and no post-generation edits.

Classification ambiguity, taxonomy pressure, and prevention mapping
friction are present as governance signals but do not modify the
underlying classifications or mappings.

**FAQ Signal Coverage Assessment**

**Technical Compromise & Wallet Drains**

  --------------------------------------------------------------------------------------------
  **Existing   **Status**   **CW35 + CW36          **Dominant Taxonomy        **Prevention
  FAQ                       Signals**              Anchors**                  Failure
  Question**                                                                  Anchors**
  ------------ ------------ ---------------------- -------------------------- ----------------
  If I never   reinforced   Wallet software        wallet_software_exploit;   Never share
  shared my                 exploitation, malware, malware; phishing          recovery phrases
  seed phrase,              phishing, malicious                               or private keys;
  how did                   permissions, and                                  Revoke token
  funds still               compromised                                       approvals and
  leave my                  environments are                                  review
  wallet?                   present in the current                            permissions
                            package.                                          regularly;
                                                                              Verify platform
                                                                              legitimacy
                                                                              before use

  Why did      reinforced   Phishing and           phishing                   Revoke token
  connecting                malicious-permission                              approvals and
  my wallet                 mechanisms remain                                 review
  drain me? I               represented in                                    permissions
  thought                   current-week records.                             regularly;
  connecting                                                                  Verify platform
  was safe.                                                                   legitimacy
                                                                              before use

  I had strong reinforced   Malware and session    malware; session_hijacking Enable strong
  2FA. How was              hijacking are present,                            authentication
  my account                including compromise                              and account
  still                     mechanisms operating                              security; Verify
  abused?                   outside ordinary login                            platform
                            protection.                                       legitimacy
                                                                              before use

  What is      reinforced   Current records map    phishing                   Revoke token
  token                     repeatedly to                                     approvals and
  approval                  permission and                                    review
  abuse, and                token-approval review                             permissions
  how can it                failures.                                         regularly
  drain funds                                                                 
  later?                                                                      

  Can a        reinforced   Current records        social_engineering         Minimize public
  scammer                   include                                           exposure of
  steal my                  social-engineering                                crypto holdings;
  crypto just               exposure and possible                             Confirm network
  by knowing                address-poisoning                                 and address
  my wallet                 behavior associated                               compatibility
  address?                  with public wallet                                before transfers
                            activity.                                         

  Can someone  reinforced   Current records        malware;                   Never share
  hack my                   distinguish compromise wallet_software_exploit;   recovery phrases
  wallet if                 mechanisms such as     phishing;                  or private keys;
  they know my              malware, wallet        social_engineering         Verify platform
  public                    software exploitation,                            legitimacy
  address?                  phishing, and social                              before use;
                            engineering from                                  Minimize public
                            possession of a public                            exposure of
                            address alone.                                    crypto holdings
  --------------------------------------------------------------------------------------------

The current taxonomy output contains malware, session hijacking, wallet
software exploitation, phishing, and social-engineering classifications
supporting these signals.

**Deception-Driven Loss Patterns**

  ----------------------------------------------------------------------------------------------
  **Existing FAQ       **Status**   **CW35 + CW36          **Dominant Taxonomy   **Prevention
  Question**                        Signals**              Anchors**             Failure
                                                                                 Anchors**
  -------------------- ------------ ---------------------- --------------------- ---------------
  What is              reinforced   Current-week           exchange_scam;        Do not pay fees
  "pay-to-withdraw,"                prevention mappings    social_engineering;   to unlock
  and why does it keep              repeatedly identify    romance_scam          withdrawals;
  appearing?                        demands for payments                         Verify platform
                                    to unlock withdrawals.                       legitimacy
                                                                                 before use

  Are tax, AML,        reinforced   Current incidents      exchange_scam;        Do not pay fees
  insurance, or                     include                social_engineering    to unlock
  verification fees                 withdrawal-payment                           withdrawals
  before withdrawal                 narratives mapped                            
  ever legitimate?                  directly to refusal of                       
                                    fees required to                             
                                    unlock funds.                                

  If a platform shows  reinforced   Fake-platform and      exchange_scam         Verify platform
  profits, why can't I              exchange-scam                                legitimacy
  just withdraw                     mechanisms remain                            before use; Do
  smaller amounts?                  represented in the                           not pay fees to
                                    current dataset.                             unlock
                                                                                 withdrawals

  Why does the         reinforced   Repeated-payment and   exchange_scam;        Do not pay fees
  platform keep asking              withdrawal-unlock      social_engineering;   to unlock
  for another payment               mechanisms are         romance_scam          withdrawals
  before I can                      explicitly represented                       
  withdraw my funds?                in current prevention                        
                                    mappings.                                    

  If a caller knows my reinforced   Social engineering and social_engineering;   Avoid
  details and claims                multi-channel          phishing              unsolicited
  to be support,                    impersonation remain                         messages calls
  doesn't that prove                present in                                   and DMs; Verify
  it's real?                        current-week                                 platform
                                    classifications.                             legitimacy
                                                                                 before use

  Why are recovery     reinforced   Current classification airdrop_scam;         Avoid
  services contacting               warnings include a     social_engineering    unsolicited
  victims almost                    secondary                                    messages calls
  always scams?                     recovery-scam                                and DMs; Do not
                                    mechanism following an                       pay fees to
                                    initial scam.                                unlock
                                                                                 withdrawals

  Why are physical     reinforced   A current              phishing              Verify platform
  letters, QR codes,                classification warning                       legitimacy
  and mailed notices                explicitly records a                         before use
  used again?                       physical-mail QR-code                        
                                    phishing campaign.                           

  What is address      reinforced   Current-week records   wrong_address         Confirm network
  poisoning, and why                include possible                             and address
  does it still work                address-poisoning                            compatibility
  on large transfers?               behavior and                                 before
                                    address-verification                         transfers; Test
                                    failure signals.                             transactions
                                                                                 with small
                                                                                 amounts first
  ----------------------------------------------------------------------------------------------

The current taxonomy output identifies phishing, social engineering,
exchange scams, airdrop scams, romance scams, and a specific
physical-mail QR-code phishing signal. Address-poisoning uncertainty is
also explicitly retained rather than reclassified.

**Irreversible User Errors**

  ---------------------------------------------------------------------------------------
  **Existing FAQ  **Status**   **CW35 + CW36        **Dominant Taxonomy  **Prevention
  Question**                   Signals**            Anchors**            Failure
                                                                         Anchors**
  --------------- ------------ -------------------- -------------------- ----------------
  Why do wallets  reinforced   Lost-wallet-access   lost_wallet_access   Never share
  sometimes show               incidents remain                          recovery phrases
  zero balance                 represented in the                        or private keys
  after restore?               current package.                          

  Why do          reinforced   Wrong-network        wrong_network        Confirm network
  wrong-network                incidents are                             and address
  transfers                    explicitly present                        compatibility
  become                       in current taxonomy                       before
  permanent                    output.                                   transfers; Test
  losses even                                                            transactions
  without a scam?                                                        with small
                                                                         amounts first

  Can crypto sent reinforced   Wrong-address and    wrong_address;       Confirm network
  to the wrong                 wrong-network        wrong_network        and address
  address be                   incidents are                             compatibility
  recovered?                   present in the                            before
                               current package.                          transfers; Test
                                                                         transactions
                                                                         with small
                                                                         amounts first

  What happens if reinforced   Lost-wallet-access   lost_wallet_access   Never share
  I lose my seed               remains the                               recovery phrases
  phrase but                   principal                                 or private keys
  still have                   current-week                              
  wallet access?               user-mistake subtype                      
                               represented in the                        
                               taxonomy output.                          
  ---------------------------------------------------------------------------------------

The current taxonomy output records wrong_address, wrong_network, and
lost_wallet_access within the user-mistake classifications.

The prevention output independently maps current records to
address/network compatibility checks, small test transactions,
recovery-phrase protection, permission review, platform verification,
and withdrawal-payment refusal.

**Candidate FAQ Additions --- CW35 + CW36 2026**

**None identified.**

Current recurring mechanisms with stable taxonomy and prevention anchors
are already represented by the existing evergreen FAQ corpus. No
additional question is required solely from the current-week evidence.

**Candidate FAQ Removals --- CW35 + CW36 2026**

**None identified.**

No existing FAQ mechanism is unsupported by the current-week package
strongly enough to justify a removal signal.

**Verdict --- CW35 + CW36 2026**

The evergreen Crypto Loss FAQ remains aligned with the current weekly
evidence.

**Additions recommended:** none identified.

**Removals recommended:** none identified.

As this is the bootstrap FAQ signal report, **CW35 + CW36 2026
establishes the initial FAQ governance baseline**.
