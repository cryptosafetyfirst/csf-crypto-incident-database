**CW17 Prevention Action Normalization Report**

**Stage**

Prevention Action Normalization Publication

**Scope**

CW17 Crypto and Web3 Incident Dataset

**Total Incidents Analyzed**

37

**Purpose**

This report measures how incident prevention guidance maps to a fixed
prevention action set. Guidance is derived from structured incident
records and mapped conservatively without adding new advice.

**Methodology Summary**

Prevention mappings are based on the prevention field only. Summary and
user mistake fields are used only to clarify intent. Vague or unmappable
text is not forced into an action. One incident can map to more than one
prevention action. Records with classification warnings are handled
conservatively.

**Data Integrity Notes**

  -------------------------------------------------------------------
  **Metric**                        **Count**   **Entry Numbers**
  --------------------------------- ----------- ---------------------
  Total incidents analyzed          37          

  Classification warnings           8           4, 5, 13, 22, 26, 30,
                                                36, 37

  Missing prevention text           0           

  Present but unmappable prevention 5           2, 5, 13, 17, 21
  text                                          

  Entry number integrity issues     0           
  -------------------------------------------------------------------

Coverage represents a lower bound because present but unmappable
prevention text exists.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            14          37.8

  Avoid unsolicited messages calls and DMs         11          29.7

  Never share recovery phrases or private keys     2           5.4

  Do not pay fees to unlock withdrawals            6           16.2

  Use hardware wallets for long term storage       2           5.4

  Enable strong authentication and account         2           5.4
  security                                                     

  Confirm network and address compatibility before 3           8.1
  transfers                                                    

  Test transactions with small amounts first       1           2.7

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    2           5.4
  regularly                                                    

  Maintain complete transaction and tax records    0           0.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

The most frequently mapped prevention action is Verify platform
legitimacy before use at 37.8% of incidents.

Avoid unsolicited messages calls and DMs is the second most frequent
action at 29.7%.

Do not pay fees to unlock withdrawals is the third most frequent action
at 16.2%.

Several locked actions have zero mapped coverage in this dataset.

**Top Prevention Actions by Coverage**

  -------------------------------------------------------------------
  **Rank**   **Prevention Action**              **Count**   **% of
                                                            Total**
  ---------- ---------------------------------- ----------- ---------
  1          Verify platform legitimacy before  14          37.8
             use                                            

  2          Avoid unsolicited messages calls   11          29.7
             and DMs                                        

  3          Do not pay fees to unlock          6           16.2
             withdrawals                                    
  -------------------------------------------------------------------

Combined percentage of total incidents: 83.8%.

**Coverage Qualification**

  -----------------------------------------------------------------------
  **Coverage Factor**                      **Status**
  ---------------------------------------- ------------------------------
  Affected by classification warnings      Yes

  Affected by missing prevention text      No

  Affected by vague or unmappable          Yes
  prevention text                          

  Conflicts with previously published      None identified from provided
  guidance                                 inputs
  -----------------------------------------------------------------------

**Interpretation**

Prevention coverage is concentrated in platform verification and
unsolicited-contact avoidance. Withdrawal-fee avoidance also appears as
a recurring mapped action. Some incident prevention text is present but
does not map cleanly to the locked action set.

**Role in the Weekly Series**

This report serves as a weekly snapshot of normalized prevention
coverage. It supports longitudinal comparison by preserving consistent
action names, counts, and percentage calculations across weekly
datasets.

**Bottom Line**

CW17 prevention coverage is led by platform verification,
unsolicited-contact avoidance, and refusal to pay withdrawal-unlock
fees. The report measures mapped coverage only and does not represent
complete prevention coverage for every incident.
