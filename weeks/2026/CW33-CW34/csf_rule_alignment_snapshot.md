**SF Rule Alignment Snapshot --- CW33 + CW34 2026**

**Dataset Scope**

- Week: CW33 + CW34 2026

- Total incidents analyzed: 56

- Incidents aligned to at least one existing CSF rule: 46

- Residual or unmapped incidents: 10

**Rule Alignment Summary**

Recurrence remains concentrated within existing governance expectations.

Alignment is concentrated in the Scam Defense Rules layer. The most
recurrent individual alignments are project legitimacy verification,
withdrawal-loop protection, and independent identity verification.

Multiple incidents align to more than one existing rule; rule
occurrences therefore represent rule-level alignments rather than unique
incident totals.

Normalization friction remains visible where current prevention guidance
is more specific than an existing rule boundary, particularly for
token-network compatibility and post-compromise recovery actions.

No rules were created, modified, merged, or reinterpreted.

**Rule Coverage Table**

  -----------------------------------------------------------------------------
  **Rule**                                                    **Occurrences**
  ----------------------------------------------------------- -----------------
  GR-001 --- NEVER SHARE YOUR SEED PHRASE                     3

  GR-002 --- ALWAYS VERIFY THE FULL URL AND DOMAIN BEFORE     2
  CONNECTING YOUR WALLET TO ANY WEBSITE                       

  GR-003 --- ALWAYS USE A HARDWARE WALLET FOR LONG-TERM OR    0
  HIGH-VALUE CRYPTO STORAGE                                   

  GR-004 --- ALWAYS REVOKE UNUSED TOKEN APPROVALS AFTER       0
  INTERACTING WITH NEW SMART CONTRACTS                        

  GR-005 --- NEVER FOLLOW URGENT "SUPPORT" OR "SECURITY"      4
  INSTRUCTIONS. EXIT THE CHANNEL AND RE-ENTER THROUGH THE     
  OFFICIAL APP OR URL                                         

  GR-006 --- ALWAYS SEND A SMALL TEST TRANSACTION BEFORE      4
  TRANSFERRING LARGE AMOUNTS OF CRYPTO                        

  GR-007 --- NEVER STORE YOUR SEED PHRASE IN CLOUD STORAGE,   1
  EMAIL, OR SCREENSHOTS                                       

  GR-008 --- KEEP LONG-TERM HOLDINGS IN A VAULT WALLET. USE A 0
  SEPARATE WALLET FOR DAPPS, TRADING AND WEB3                 

  OR-001 --- TEST YOUR WALLET RECOVERY BEFORE TRUSTING IT     1

  OR-002 --- NEVER RELY ON A SINGLE SEED PHRASE BACKUP        0

  OR-003 --- DOCUMENT HOW YOUR WALLET WAS CREATED             1

  OR-004 --- NEVER STORE SEED PHRASES ONLY IN DIGITAL FORM    1

  OR-005 --- ALWAYS VERIFY THE DESTINATION BEFORE SENDING     3
  CRYPTO                                                      

  OR-006 --- MAINTAIN ACCESS TO YOUR AUTHENTICATION SYSTEMS   1

  OR-007 --- PLAN WALLET RECOVERY FOR EMERGENCIES AND         1
  INHERITANCE                                                 

  SDR-001 --- NEVER TRUST UNSOLICITED CRYPTO CONTACT          4

  SDR-002 --- NEVER SEND CRYPTO TO RECEIVE CRYPTO             3

  SDR-003 --- NEVER PAY TO UNLOCK OR WITHDRAW FUNDS           8

  SDR-004 --- VERIFY IDENTITIES OUTSIDE THE MESSAGE CHANNEL   8

  SDR-005 --- NEVER CONNECT YOUR WALLET TO UNKNOWN WEBSITES   1

  SDR-006 --- QUESTION URGENCY, HYPE, AND GUARANTEED PROFITS  1

  SDR-007 --- VERIFY PROJECTS BEFORE INVESTING                19

  SDR-008 --- NEVER TRUST SOCIAL MEDIA POPULARITY             0

  SDR-009 --- VERIFY ALL LINKS BEFORE LOGGING IN              0

  TSR-001 --- NEVER INSTALL CRYPTO SOFTWARE FROM UNOFFICIAL   2
  SOURCES                                                     

  TSR-002 --- ASSUME YOUR DEVICE CAN BE COMPROMISED           2

  TSR-003 --- AVOID PUBLIC WI-FI FOR CRYPTO OPERATIONS        0

  TSR-004 --- USE HARDWARE-BASED TWO-FACTOR AUTHENTICATION    0

  TSR-005 --- ENABLE WITHDRAWAL WHITELISTS ON EXCHANGES       0

  TSR-006 --- SEPARATE DEVICES AND ACCOUNTS FOR CRYPTO USE    2

  TSR-007 --- SLOW DOWN BEFORE CLICKING OR INSTALLING         1
  -----------------------------------------------------------------------------

**Layer Coverage Table**

  --------------------------------------
  **Defensive Layer**  **Occurrences**
  -------------------- -----------------
  Golden Rules         14

  Operational Rules    8

  Scam Defense Rules   44

  Technical Security   7
  Rules                
  --------------------------------------

**Residual / Uncertain Mappings**

Ten incidents did not align conservatively to an existing CSF rule:

- Entries 2, 18, 20, 26, and 33 contain post-compromise wallet migration
  and forensic-preservation guidance without a direct rule match.

- Entries 36, 40, 42, and 43 concern token-network or asset-network
  compatibility that is more specific than the existing
  destination-verification rule boundary.

- Entry 44 contains wallet-setup and credential-isolation guidance that
  does not map cleanly to an existing rule without broadening the rule
  meaning.

Partial alignment also remains visible where one prevention action maps
to an existing rule while another action in the same incident remains
outside the current canon. Network compatibility paired with a small
test transaction is one such case.

Residual mappings remain advisory only.

No governance escalation threshold identified from the supplied inputs.

**Method Note**

This report is a downstream governance visibility artifact only.

It does not modify canonical incident records, taxonomy classifications,
prevention mappings, the CSF Rule Registry, or any other canonical
artifact. Rule alignment was performed conservatively against the
existing locked rule set; no new rules were created or existing rules
changed.
