**Dataset Scope**

**Week identifier:** CW35 + CW36 2026\
**Total incidents analyzed:** 73\
**Incidents aligned to at least one existing CSF rule:** 59\
**Residual / unmapped incidents:** 14

**Rule Alignment Summary**

Recurrence remains concentrated within existing governance expectations.

The most frequently aligned existing rule is **SDR-003 --- NEVER PAY TO
UNLOCK OR WITHDRAW FUNDS**, with 12 occurrences.

Alignment is concentrated in the behavioral rule layer, followed by the
structural and operational layers.

Normalization remains conservative. The prevention analysis records
vague or non-actionable prevention text and present but unmappable
prevention text, and those conditions were not converted into new rules.

No governance escalation threshold identified.

**Rule Coverage Table**

  -----------------------------------------------------------------------------
  **Rule**                                                    **Occurrences**
  ----------------------------------------------------------- -----------------
  GR-001 --- NEVER SHARE YOUR SEED PHRASE                     3

  GR-002 --- ALWAYS VERIFY THE FULL URL AND DOMAIN BEFORE     8
  CONNECTING YOUR WALLET TO ANY WEBSITE                       

  GR-003 --- ALWAYS USE A HARDWARE WALLET FOR LONG-TERM OR    0
  HIGH-VALUE CRYPTO STORAGE                                   

  GR-004 --- ALWAYS REVOKE UNUSED TOKEN APPROVALS AFTER       3
  INTERACTING WITH NEW SMART CONTRACTS                        

  GR-005 --- NEVER FOLLOW URGENT "SUPPORT" OR "SECURITY"      5
  INSTRUCTIONS. EXIT THE CHANNEL AND RE-ENTER THROUGH THE     
  OFFICIAL APP OR URL                                         

  GR-006 --- ALWAYS SEND A SMALL TEST TRANSACTION BEFORE      6
  TRANSFERRING LARGE AMOUNTS OF CRYPTO                        

  GR-007 --- NEVER STORE YOUR SEED PHRASE IN CLOUD STORAGE,   1
  EMAIL, OR SCREENSHOTS                                       

  GR-008 --- KEEP LONG-TERM HOLDINGS IN A VAULT WALLET. USE A 0
  SEPARATE WALLET FOR DAPPS, TRADING AND WEB3                 

  OR-001 --- TEST YOUR WALLET RECOVERY BEFORE TRUSTING IT     2

  OR-002 --- NEVER RELY ON A SINGLE SEED PHRASE BACKUP        0

  OR-003 --- DOCUMENT HOW YOUR WALLET WAS CREATED             0

  OR-004 --- NEVER STORE SEED PHRASES ONLY IN DIGITAL FORM    6

  OR-005 --- ALWAYS VERIFY THE DESTINATION BEFORE SENDING     2
  CRYPTO                                                      

  OR-006 --- MAINTAIN ACCESS TO YOUR AUTHENTICATION SYSTEMS   0

  OR-007 --- PLAN WALLET RECOVERY FOR EMERGENCIES AND         0
  INHERITANCE                                                 

  SDR-001 --- NEVER TRUST UNSOLICITED CRYPTO CONTACT          8

  SDR-002 --- NEVER SEND CRYPTO TO RECEIVE CRYPTO             1

  SDR-003 --- NEVER PAY TO UNLOCK OR WITHDRAW FUNDS           12

  SDR-004 --- VERIFY IDENTITIES OUTSIDE THE MESSAGE CHANNEL   7

  SDR-005 --- NEVER CONNECT YOUR WALLET TO UNKNOWN WEBSITES   3

  SDR-006 --- QUESTION URGENCY, HYPE, AND GUARANTEED PROFITS  2

  SDR-007 --- VERIFY PROJECTS BEFORE INVESTING                6

  SDR-008 --- NEVER TRUST SOCIAL MEDIA POPULARITY             6

  SDR-009 --- VERIFY ALL LINKS BEFORE LOGGING IN              2

  TSR-001 --- NEVER INSTALL CRYPTO SOFTWARE FROM UNOFFICIAL   5
  SOURCES                                                     

  TSR-002 --- ASSUME YOUR DEVICE CAN BE COMPROMISED           0

  TSR-003 --- AVOID PUBLIC WI-FI FOR CRYPTO OPERATIONS        0

  TSR-004 --- USE HARDWARE-BASED TWO-FACTOR AUTHENTICATION    0

  TSR-005 --- ENABLE WITHDRAWAL WHITELISTS ON EXCHANGES       0

  TSR-006 --- SEPARATE DEVICES AND ACCOUNTS FOR CRYPTO USE    0

  TSR-007 --- SLOW DOWN BEFORE CLICKING OR INSTALLING         0
  -----------------------------------------------------------------------------

**Layer Coverage Table**

  ---------------------------------
  **Defensive     **Occurrences**
  Layer**         
  --------------- -----------------
  behavioral      47

  tooling-based   5

  structural      26

  operational     10
  ---------------------------------

**Residual / Uncertain Mappings**

The following incidents contain prevention guidance that was not
conservatively aligned to an existing CSF rule:

- INC-20260823-a1e9f0dc44

- INC-20260822-5d0fc0f378

- INC-20260822-82af04a5fb

- INC-20260825-29756a77f8

- INC-20260831-0cf68dd33f

- INC-20260828-fbe1e3622d

- INC-20260828-32f53761cb

- INC-20260830-3c07e1e8e8

- INC-20260902-804db57bb9

- INC-20260901-d1fb06e35d

- INC-20260831-609dd172c1

- INC-20260831-1c8cf452f2

- INC-20260904-10942a8b0b

- INC-20260903-18d45f0805

No uncertain mapping was counted as a rule occurrence. Where
correspondence with an existing rule was insufficiently explicit, the
incident remained residual.

Normalization friction remains visible in the prevention output,
including vague or non-actionable prevention text and prevention text
that was present but unmappable. Classification ambiguity also remains
visible in the taxonomy output and was not resolved through rule
alignment.

Residual mappings remain advisory only.

**Method Note**

This report is a downstream governance visibility artifact only.

It does not modify canonical incident records, taxonomy classifications,
prevention mappings, or the CSF Rule Registry.

Only existing registry rules were eligible for alignment. No rules were
created, renamed, merged, expanded, or modified.

Defensive-layer occurrences aggregate existing rule-family alignments as
structural, operational, behavioral, and tooling-based.
