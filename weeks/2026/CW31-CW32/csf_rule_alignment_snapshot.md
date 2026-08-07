**CSF Rule Alignment Snapshot --- CW31 + CW32 2026**

**Dataset Scope**

  ---------------------------------------------------
  **Metric**                        **Occurrences**
  --------------------------------- -----------------
  Total incidents analyzed          62

  Incidents aligned to at least one 52
  CSF rule                          

  Residual / unmapped incidents     10
  ---------------------------------------------------

The current dataset contains 62 incidents. The taxonomy records 32
scams, 15 hacks, and 15 user mistakes.

**Rule Alignment Summary**

Rule recurrence remains concentrated within the existing CSF Defensive
Rule Canon.

The highest recurrence is associated with independent platform
verification, unsolicited-contact resistance, transaction testing,
compromised-device assumptions, withdrawal-fee resistance,
official-channel verification, and destination verification.

Multiple rules may align with a single incident. Rule occurrence counts
therefore represent rule mappings rather than distinct incidents.

Normalization remains conservative. The prevention normalization report
records 41 incidents mapped to its narrower standardized
prevention-action set and identifies 21 incidents whose prevention text
did not produce a standardized action mapping. This does not preclude
alignment with the broader locked CSF Rule Registry where the incident
prevention text directly corresponds to an existing rule.

No rules were created or modified.

**Rule Coverage Table**

  -----------------------------------------------------------------------------
  **Rule**                                                    **Occurrences**
  ----------------------------------------------------------- -----------------
  SDR-007 --- VERIFY PROJECTS BEFORE INVESTING                10

  SDR-001 --- NEVER TRUST UNSOLICITED CRYPTO CONTACT          8

  GR-006 --- ALWAYS SEND A SMALL TEST TRANSACTION BEFORE      7
  TRANSFERRING LARGE AMOUNTS OF CRYPTO                        

  TSR-002 --- ASSUME YOUR DEVICE CAN BE COMPROMISED           7

  GR-005 --- NEVER FOLLOW URGENT "SUPPORT" OR "SECURITY"      6
  INSTRUCTIONS. EXIT THE CHANNEL AND RE-ENTER THROUGH THE     
  OFFICIAL APP OR URL                                         

  OR-005 --- ALWAYS VERIFY THE DESTINATION BEFORE SENDING     6
  CRYPTO                                                      

  SDR-003 --- NEVER PAY TO UNLOCK OR WITHDRAW FUNDS           6

  OR-001 --- TEST YOUR WALLET RECOVERY BEFORE TRUSTING IT     3

  OR-007 --- PLAN WALLET RECOVERY FOR EMERGENCIES AND         3
  INHERITANCE                                                 

  SDR-006 --- QUESTION URGENCY, HYPE, AND GUARANTEED PROFITS  3

  TSR-001 --- NEVER INSTALL CRYPTO SOFTWARE FROM UNOFFICIAL   3
  SOURCES                                                     

  TSR-007 --- SLOW DOWN BEFORE CLICKING OR INSTALLING         3

  GR-001 --- NEVER SHARE YOUR SEED PHRASE                     2

  OR-003 --- DOCUMENT HOW YOUR WALLET WAS CREATED             2

  SDR-002 --- NEVER SEND CRYPTO TO RECEIVE CRYPTO             2

  SDR-004 --- VERIFY IDENTITIES OUTSIDE THE MESSAGE CHANNEL   2

  GR-003 --- ALWAYS USE A HARDWARE WALLET FOR LONG-TERM OR    1
  HIGH-VALUE CRYPTO STORAGE                                   

  GR-008 --- KEEP LONG-TERM HOLDINGS IN A VAULT WALLET. USE A 1
  SEPARATE WALLET FOR DAPPS, TRADING AND WEB3                 

  OR-002 --- NEVER RELY ON A SINGLE SEED PHRASE BACKUP        1
  -----------------------------------------------------------------------------

**Layer Coverage Table**

  --------------------------------------
  **Defensive Layer**  **Occurrences**
  -------------------- -----------------
  Scam Defense Rules   31

  Golden Rules         17

  Operational Rules    15

  Technical Security   13
  Rules                
  --------------------------------------

Layer occurrences total 76 because individual incidents may align with
more than one rule and therefore more than one defensive layer.

**Residual / Uncertain Mappings**

  -----------------------------------------------------------------------------
  **Residual / Uncertain Mapping**                            **Occurrences**
  ----------------------------------------------------------- -----------------
  Residual / unmapped incidents                               10

  Incidents carrying taxonomy classification warnings         33

  Prevention records vague or non-actionable under            1
  standardized normalization                                  

  Prevention records present but unmappable under             20
  standardized normalization                                  
  -----------------------------------------------------------------------------

Classification warnings affect 33 of the 62 incidents and are retained
without changing the underlying taxonomy classifications.

The prevention normalization process identifies one vague or
non-actionable prevention record and 20 records containing prevention
guidance that does not correspond to its standardized action set. These
were left unmapped rather than forced into unrelated categories.

Residual rule mappings remain advisory only. Prevention statements
without sufficiently direct correspondence to a locked CSF rule were not
forced into the Rule Coverage Table.

No governance escalation threshold is identified.

**Method Note**

This report is a downstream governance visibility artifact only.

It does not modify canonical incident records, taxonomy classifications,
prevention mappings, the CSF Rule Registry, or any other canonical
artifact.
