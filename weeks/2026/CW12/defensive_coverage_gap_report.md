**Defensive Coverage Gap Report --- CW12 2026**

**Purpose**

This report evaluates whether the dominant prevention failure points
observed in the current weekly dataset are already addressed by the
existing CSF defensive corpus.\
It is a non-public, governance-only artifact and does not introduce
analysis, recommendations, or new defensive constructs.

------------------------------------------------------------------------

**Inputs Declared (CW12)**

- incidents.csv (CW12)

- taxonomy report (CW12)

- prevention report (CW12)

- governance notes (CW12)

- manifest (CW12)

------------------------------------------------------------------------

**Defensive Canon --- Source Availability**

The following canonical defensive materials are identified and
available:

- Practical Crypto & Web3 Safety Tools --- rev16JAN2026

- Three-Wallet Model --- 1st Edition 2025

- Hack mechanisms book --- 1st Edition 2025

- Scam mechanisms book --- 1st Edition 2025

- User mistake prevention book --- 1st Edition 2025

All required defensive canon sources are present and unambiguously
identifiable.

------------------------------------------------------------------------

**Defensive Coverage Assessment**

  -------------------------------------------------------------------------
  **Prevention Failure   **Observed Signal       **Coverage in **Coverage
  Point**                (CW12)**                Defensive     Type**
                                                 Canon**       
  ---------------------- ----------------------- ------------- ------------
  Failure to verify      Dominant mapping (20    covered       behavioral /
  platform legitimacy    incidents)                            tooling
  before use                                                   

  Engagement with        Second-highest mapping  covered       behavioral
  unsolicited messages   (11 incidents)                        
  and contact channels                                         

  Exposure of sensitive  Present across multiple covered       behavioral /
  credentials (seed      incidents (6 cases)                   structural
  phrases / private                                            
  keys)                                                        

  Incorrect transaction  Present                 covered       behavioral
  network or address     (wrong_network +                      
  validation             compatibility failures)               

  Failure to test        Present (4 incidents)   covered       behavioral
  transactions before                                          
  execution                                                    

  Persistent token       Present (4 incidents)   covered       tooling
  approval exposure                                            

  Payment of fees to     Present (exchange scam  covered       behavioral
  unlock withdrawals     pattern)                              

  Loss of wallet access  Present                 covered       structural /
  due to poor recovery   (lost_wallet_access                   behavioral
  or backup practices    cases)                                
  -------------------------------------------------------------------------

------------------------------------------------------------------------

**Coverage Determination Summary**

- All dominant prevention failure points observed in CW12 are
  **covered** by one or more elements of the CSF Defensive Canon.

- Coverage spans:

  - behavioral controls (decision-point verification, interaction
    discipline)

  - tooling controls (approval management, platform verification tools)

  - structural controls (wallet segmentation, recovery and custody
    design)

No prevention failure point requires classification as partially covered
or uncovered based on available canonical materials.

------------------------------------------------------------------------

**Verdict**

The current CSF defensive canon addresses the earliest preventable
failure points observed in CW12.

No defensive coverage gaps are identified for this dataset.
