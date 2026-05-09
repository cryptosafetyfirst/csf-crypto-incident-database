**FAQ Signal Report --- CW19 2026**

**Purpose**

This report evaluates whether the evergreen FAQ corpus remains aligned
with observed CW19 2026 incident mechanisms and normalized prevention
signals.

This report is governance-only and non-public.

**Inputs Declared --- CW19 2026**

Artifacts used:

- incidents.csv

- taxonomy_report.docx

- prevention_report.docx

- governance_notes.docx

- manifest.md

- README.md

Evergreen FAQ corpus referenced:

- Evergreen_FAQ_rev17FEB2026.docx

Report mode:

- bootstrap report

**Governance Check**

- taxonomy reclassification occurred: no

- scope changes occurred: no

- prevention mapping definitions changed: no

**FAQ Signal Coverage Assessment**

  ---------------------------------------------------------------------------------------------------
  **FAQ Question**  **Status**   **CW19 Signal         **Dominant Taxonomy Anchors**  **Dominant
                                 Anchors**                                            Prevention
                                                                                      Failure
                                                                                      Anchors**
  ----------------- ------------ --------------------- ------------------------------ ---------------
  If I never shared reinforced   wallet drain          wallet_software_exploit        Never share
  my seed phrase                 incidents and                                        recovery
  how did funds                  compromised wallet                                   phrases or
  still leave my                 environments observed                                private keys
  wallet?                                                                             

  Why did           reinforced   smart contract        smart_contract_scam            Revoke token
  connecting my                  approval exposure and                                approvals and
  wallet drain me I              wallet connection                                    review
  thought                        risk observed                                        permissions
  connecting was                                                                      regularly
  safe?                                                                               

  I had strong 2FA  absent       no direct session     none dominant                  none dominant
  How was my                     persistence or 2FA                                   
  account still                  bypass incidents                                     
  abused?                        identified                                           

  What is token     reinforced   approval persistence  smart_contract_scam            Revoke token
  approval abuse                 and smart contract                                   approvals and
  and how can it                 permission exposure                                  review
  drain funds                    observed                                             permissions
  later?                                                                              regularly

  What is           reinforced   withdrawal            exchange_scam                  Do not pay fees
  pay-to-withdraw                restriction                                          to unlock
  and why does it                narratives and                                       withdrawals
  keep appearing?                additional payment                                   
                                 framing observed                                     

  Are tax AML       reinforced   withdrawal            exchange_scam                  Do not pay fees
  insurance or                   restriction and                                      to unlock
  verification fees              compliance payment                                   withdrawals
  before withdrawal              narratives observed                                  
  ever legitimate?                                                                    

  If a platform     reinforced   fake platform custody exchange_scam                  Verify platform
  shows profits why              and blocked                                          legitimacy
  can't I just                   withdrawal behavior                                  before use
  withdraw smaller               observed                                             
  amounts?                                                                            

  If a caller knows absent       no direct             none dominant                  none dominant
  my details and                 impersonation                                        
  claims to be                   support-call                                         
  support doesn't                mechanism identified                                 
  that prove it's                                                                     
  real?                                                                               

  Why are recovery  weakened     secondary recovery    social_engineering             Avoid
  services                       scam references                                      unsolicited
  contacting                     appeared only                                        messages calls
  victims almost                 indirectly                                           and DMs
  always scams?                                                                       

  Why are physical  absent       no physical-mail      none dominant                  none dominant
  letters QR codes               phishing mechanisms                                  
  and mailed                     identified                                           
  notices used                                                                        
  again?                                                                              

  What is address   reinforced   address poisoning and address_poisoning_copy_paste   Confirm network
  poisoning and why              lookalike recipient                                  and address
  does it still                  misuse observed                                      compatibility
  work on large                                                                       before
  transfers?                                                                          transfers

  Why do wallets    absent       no restore-context    none dominant                  none dominant
  sometimes show                 wallet recovery                                      
  zero balance                   confusion incidents                                  
  after restore?                 identified                                           

  Why do            reinforced   unsupported network   wrong_network                  Confirm network
  wrong-network                  transfer loss                                        and address
  transfers become               observed                                             compatibility
  permanent losses                                                                    before
  even without a                                                                      transfers
  scam?                                                                               

  Can crypto sent   weakened     wrong-address         wrong_network                  Confirm network
  to the wrong                   finality appeared                                    and address
  address be                     indirectly through                                   compatibility
  recovered?                     transfer                                             before
                                 compatibility                                        transfers
                                 incidents                                            

  What happens if I absent       no                    none dominant                  none dominant
  lose my seed                   recoverability-loss                                  
  phrase but still               incidents identified                                 
  have wallet                                                                         
  access?                                                                             
  ---------------------------------------------------------------------------------------------------

**Candidate FAQ Additions --- CW19 2026**

  -----------------------------------------------------------------------
  **Candidate Question**            **Justification**
  --------------------------------- -------------------------------------
  Why do fake exchanges keep using  recurring exchange_scam incidents
  account review and withdrawal     involving blocked withdrawals and
  restriction narratives?           unverifiable custody

  Why can wallet drains still occur recurring smart contract approval
  after approving a smart contract  persistence and delayed-drain
  only once?                        concerns
  -----------------------------------------------------------------------

**Candidate FAQ Removals --- CW19 2026**

none identified

**Verdict --- CW19 2026**

The evergreen FAQ remains broadly aligned with observed CW19 2026 loss
mechanisms and normalized prevention mappings.

Reinforcement signals were strongest for exchange withdrawal scams
wallet authorization abuse address poisoning and wrong-network transfer
failures.

Two candidate additions were identified based on recurring exchange
custody restriction narratives and persistent smart contract approval
exposure.

No FAQ removals are currently justified.
