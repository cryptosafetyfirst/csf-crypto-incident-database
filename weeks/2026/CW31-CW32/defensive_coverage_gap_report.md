**Defensive Coverage Gap Report --- CW31 + CW32 2026**

**Purpose**

This report provides governance-only visibility into whether dominant
prevention failure points observed during CW31 + CW32 2026 are addressed
within the currently declared CSF Defensive Canon.

The report is non-public and informational only. It evaluates declared
coverage presence and does not validate effectiveness, certify
educational sufficiency, provide prevention guarantees, modify
governance rules, or expand the defensive canon.

**Inputs Declared**

- incidents.csv

- manifest.md

- taxonomy_report.md

- prevention_report.md

- governance_notes.md

- *Practical Crypto Web3 Safety Tools (Reference Guide)*

- *The Three-Wallet Model™: A Practical Guide to Safer Crypto and Web3
  Self-Custody*

- *The Crypto & Web3 User Mistakes Prevention Guidebook*

- *The Crypto and Web3 Scams Prevention Guidebook*

- *How to Keep Your Crypto and Digital Assets Safe from Hackers*

The declared dataset contains 62 incidents.

Prevention normalization mapped 41 incidents to at least one
standardized action. One incident contained vague or non-actionable
prevention text, while 20 contained prevention guidance that could not
be conservatively mapped to the standardized action set.

**Coverage Assessment**

The dominant normalized prevention failure points are avoiding
unsolicited contact, verifying platform legitimacy, testing transactions
with small amounts, refusing payments to unlock withdrawals, and
confirming network and address compatibility.

  -------------------------------------------------------------------------------------------------
  **Prevention     **Observed   **Coverage   **Coverage Basis**    **Coverage Type** **Canonical
  Failure Point**  Mappings**   Status**                                             Coverage
                                                                                     Sources**
  ---------------- ------------ ------------ --------------------- ----------------- --------------
  Failure to avoid 13           Covered      Canonical materials   Direct            *Crypto and
  unsolicited                                explicitly address    educational       Web3 Scams
  messages, calls,                           unsolicited support,  coverage          Prevention
  and DMs                                    direct messages,                        Guidebook*;
                                             impersonation,                          *How to Keep
                                             alternate-channel                       Your Crypto
                                             identity                                and Digital
                                             verification, and                       Assets Safe
                                             official                                from Hackers*
                                             communication                           
                                             channels.                               

  Failure to       12           Covered      Canonical scam        Direct            *Crypto and
  verify platform                            material explicitly   educational       Web3 Scams
  legitimacy                                 instructs users to    coverage          Prevention
  before use                                 verify exchange and                     Guidebook*;
                                             investment-platform                     *Practical
                                             legitimacy, conduct                     Crypto Web3
                                             independent research,                   Safety Tools*
                                             check platform                          
                                             history, and inspect                    
                                             domain information                      
                                             before depositing                       
                                             funds.                                  

  Failure to test  8            Covered      Canonical             Direct procedural *Crypto & Web3
  transactions                               user-mistake material coverage          User Mistakes
  with small                                 explicitly includes                     Prevention
  amounts first                              small test                              Guidebook*;
                                             transactions as part                    *The
                                             of safe sending and                     Three-Wallet
                                             pairs testing with                      Model™*
                                             address, network,                       
                                             token, and recipient                    
                                             verification.                           

  Payment of fees  7            Covered      Canonical scam        Direct            *Crypto and
  or additional                              material documents    scam-prevention   Web3 Scams
  funds to unlock                            withdrawal-lock and   coverage          Prevention
  withdrawals                                upfront-payment                         Guidebook*
                                             mechanisms and                          
                                             instructs users to                      
                                             treat blocked                           
                                             withdrawals and                         
                                             additional payment                      
                                             demands as scam                         
                                             indicators.                             

  Failure to       6            Covered      Canonical             Direct procedural *Crypto & Web3
  confirm network                            user-mistake material coverage          User Mistakes
  and address                                explicitly requires                     Prevention
  compatibility                              verification of the                     Guidebook*
  before transfers                           destination address,                    
                                             correct                                 
                                             blockchain/network,                     
                                             recipient token                         
                                             support, and small                      
                                             test transfers where                    
                                             appropriate.                            

  Weak             2            Covered      Declared safety       Tool and          *Practical
  authentication                             materials include     educational       Crypto Web3
  and account                                two-factor            coverage          Safety Tools*;
  security                                   authentication,                         *How to Keep
                                             hardware security                       Your Crypto
                                             keys, password                          and Digital
                                             managers, and                           Assets Safe
                                             account-security                        from Hackers*
                                             controls as defensive                   
                                             measures against                        
                                             account takeover.                       

  Recovery phrase  2            Covered      Canonical scam        Direct            *Crypto and
  or private-key                             material explicitly   educational       Web3 Scams
  disclosure                                 states that recovery  coverage          Prevention
                                             phrases should not be                   Guidebook*;
                                             shared and identifies                   *The
                                             requests for them                       Three-Wallet
                                             through fake support,                   Model™*
                                             websites, and                           
                                             recovery tools as                       
                                             hostile behavior.                       

  Incomplete       3            Covered      The declared          Tool and          *Practical
  transaction and                            safety-tools          operational       Crypto Web3
  tax records                                reference includes    coverage          Safety Tools*
                                             portfolio and tax                       
                                             trackers for                            
                                             consolidating                           
                                             multi-chain                             
                                             transactions and                        
                                             maintaining activity                    
                                             records needed for                      
                                             audits,                                 
                                             investigations, and                     
                                             tax reporting.                          
  -------------------------------------------------------------------------------------------------

The dataset also contains substantial prevention language outside the
standardized normalization set. Twenty incidents contained concrete
prevention guidance that was left unmapped rather than forced into an
unrelated standardized action.

This normalization friction does not itself establish a defensive canon
gap. The governance notes retain those cases for future review without
introducing taxonomy or prevention changes.

The incident taxonomy also shows significant wallet-related technical
exposure: wallet_software_exploit accounts for 13 incidents,
representing 86.7% of hack incidents in the dataset. Declared defensive
materials contain corresponding wallet-isolation, hardware-wallet,
official-source, device-security, and compartmentalization coverage. The
Three-Wallet Model, for example, separates long-term, everyday, and
higher-risk activity and provides dedicated security practices for each
exposure profile.

**Coverage Verdict**

  -------------------------------------------------------
  **Assessment Area**                       **Verdict**
  ----------------------------------------- -------------
  Avoiding unsolicited contact              Covered

  Platform legitimacy verification          Covered

  Small test transactions                   Covered

  Withdrawal-fee resistance                 Covered

  Network and address compatibility         Covered

  Authentication and account security       Covered

  Recovery phrase and private-key           Covered
  protection                                

  Transaction and tax recordkeeping         Covered

  Overall dominant prevention failure-point Covered
  coverage                                  
  -------------------------------------------------------

Coverage exists within currently available CSF materials.

No uncovered dominant prevention failure point identified.

The presence of unmapped prevention language does not establish absence
of defensive coverage because the normalization process deliberately
leaves guidance unmapped when it cannot be reliably fitted to the
standardized action set.

Coverage visibility remains informational only. It does not establish
prevention effectiveness, educational sufficiency, or defensive
completeness, and no new defensive canon entries are created by this
assessment.
