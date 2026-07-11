**FAQ Signal Report --- CW27 + CW28 2026**

**Purpose**

This report assesses whether the current evergreen Crypto Loss FAQ
remains aligned with the observed mechanisms contained within the
current weekly dataset. It is a governance artifact intended to support
evidence-based maintenance of the FAQ corpus and is not intended for
publication.

------------------------------------------------------------------------

**Inputs Declared**

**Artifacts used**

- manifest.md

- incidents.csv

- taxonomy_report.md

- prevention_report.md

- governance_notes.md

- README.md

- Current Evergreen Crypto Loss FAQ corpus

**Report type**

Bootstrap report.

**Evergreen FAQ reference**

Current FAQ corpus dated **05 Jul 2026**.

------------------------------------------------------------------------

**Governance Check**

- Taxonomy reclassification: **No**

- Scope changes: **No**

- Prevention mapping definition changes: **No**

------------------------------------------------------------------------

**FAQ Signal Coverage Assessment**

  ------------------------------------------------------------------------------------
  **Existing FAQ         **Status**   **CW27+CW28       **Dominant Anchors**
  Question**                          Signal Basis**    
  ---------------------- ------------ ----------------- ------------------------------
  If I never shared my   Reinforced   Multiple wallet   smart_contract_scam, trojan,
  seed phrase, how did                drain cases       wallet_software_exploit;
  funds still leave my                without seed      approval permissions
  wallet?                             phrase disclosure 

  Why did connecting my  Reinforced   Wallet connection smart_contract_scam; platform
  wallet drain me? I                  phishing remained verification
  thought connecting was              present           
  safe.                                                 

  I had strong 2FA. How  Reinforced   Compromised       trojan, spyware
  was my account still                environments and  
  abused?                             malware remained  
                                      represented       

  What is token approval Reinforced   Multiple          smart_contract_scam; approval
  abuse, and how can it               approval-based    review
  drain funds later?                  wallet drains     
                                      observed          

  Can a scammer steal my Reinforced   Address-only      social_engineering, phishing
  crypto just by knowing              knowledge         
  my wallet address?                  remained          
                                      insufficient;     
                                      attacks required  
                                      authorization or  
                                      deception         

  Can someone hack my    Reinforced   No conflicting    phishing, smart_contract_scam
  wallet if they know my              observations      
  public address?                                       

  What is                Reinforced   Fake investment   exchange_scam; withdrawal-fee
  \"pay-to-withdraw,\"                platforms         failures
  and why does it keep                repeatedly        
  appearing?                          demanded          
                                      withdrawal        
                                      payments          

  Are tax, AML,          Reinforced   Withdrawal-fee    exchange_scam; withdrawal-fee
  insurance, or                       narratives        failures
  verification fees                   repeatedly        
  before withdrawal ever              appeared          
  legitimate?                                           

  If a platform shows    Reinforced   Fake balances and exchange_scam
  profits, why can\'t I               staged            
  just withdraw smaller               withdrawals       
  amounts?                            remained present  

  Why does the platform  Reinforced   Escalating        exchange_scam; withdrawal-fee
  keep asking for                     payment demands   failures
  another payment before              remained common   
  I can withdraw my                                     
  funds?                                                

  If a caller knows my   Reinforced   Impersonation and social_engineering, phishing
  details and claims to               support fraud     
  be support, doesn\'t                remained present  
  that prove it\'s real?                                

  Why are recovery       Reinforced   Recovery scam     social_engineering
  services contacting                 attempts          
  victims almost always               continued to      
  scams?                              appear            

  Why are physical       Reinforced   Physical Ledger   phishing
  letters, QR codes, and              phishing letters  
  mailed notices used                 reappeared        
  again?                                                

  What is address        Reinforced   Address poisoning address_poisoning_copy_paste
  poisoning, and why                  thefts were       
  does it still work on               observed          
  large transfers?                                      

  Why do wallets         Absent       No matching       ---
  sometimes show zero                 mechanism         
  balance after restore?              observed during   
                                      this reporting    
                                      period            

  Why do wrong-network   Absent       No observed       ---
  transfers become                    signal during     
  permanent losses even               this reporting    
  without a scam?                     period            

  Can crypto sent to the Absent       No direct         ---
  wrong address be                    observed signal   
  recovered?                          during this       
                                      reporting period  

  What happens if I lose Weakened     Limited evidence  lost_wallet_access
  my seed phrase but                  this reporting    
  still have wallet                   period            
  access?                                               
  ------------------------------------------------------------------------------------

Signal assignments are supported by the taxonomy distribution,
prevention normalization outputs, and governance observations.

------------------------------------------------------------------------

**Candidate FAQ Additions**

  -------------------------------------------------------------------------
  **Candidate Question**  **Supporting Signals**      **Dominant Anchors**
  ----------------------- --------------------------- ---------------------
  How can fake Google     Multiple phishing incidents phishing
  sponsored ads steal my  involving sponsored search  
  crypto?                 advertisements leading to   
                          cloned websites             

  How can fake job        Repeated developer          job_scam, trojan
  interviews compromise   recruitment and interview   
  my wallet or computer?  malware campaigns           

  Why are Telegram and    Multiple scam operations    social_engineering,
  WhatsApp crypto trading originated from messaging   exchange_scam
  groups so frequently    groups                      
  used in scams?                                      

  Why can signing a       Multiple approval phishing  smart_contract_scam
  transaction drain funds incidents involving         
  without revealing my    malicious transaction       
  seed phrase?            signatures                  
  -------------------------------------------------------------------------

------------------------------------------------------------------------

**Candidate FAQ Removals**

**None identified.**

------------------------------------------------------------------------

**Verdict**

The evergreen FAQ remains broadly aligned with the mechanisms observed
during CW27 + CW28. Most existing questions were reinforced by the
current dataset. Several additional mechanisms met the threshold for
consideration as future FAQ entries, while no existing question met the
threshold for removal. This report establishes the governance baseline
for future comparative FAQ signal assessments.
