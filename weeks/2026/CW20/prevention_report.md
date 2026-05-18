**CW20 Prevention Action Normalization Report**

Stage: Prevention Action Normalization (Publication)\
Scope: CW20 Crypto & Web3 Incident Dataset\
Total Incidents Analyzed: 55

**Purpose**

This report standardizes prevention guidance derived from real crypto
and Web3 incident records into a fixed prevention action set. The goal
is to measure prevention coverage consistently across incidents while
preserving deterministic and comparable mappings. All prevention
mappings are constrained to a locked action set and are derived only
from prevention text already present in the dataset.

**Methodology Summary**

Prevention actions were mapped conservatively using only the prevention
field provided in each incident record. Multiple prevention actions
could be assigned to a single incident when explicitly supported by the
prevention text. Vague, narrative, contradictory, or unmappable
prevention text was not force-mapped. Classification warnings were
treated conservatively during normalization.

**Data Integrity Notes**

  -------------------------------------------------------
  **Metric**                                  **Value**
  ------------------------------------------- -----------
  Total incidents analyzed                    55

  Incidents with classification warnings      3

  Affected entry numbers                      34, 44, 50

  Incidents with missing prevention text      0

  Incidents with present but unmappable       14
  prevention text                             

  Entry number integrity issues               None
  -------------------------------------------------------

Coverage values represent a lower bound because some prevention text was
present but could not be mapped conservatively to the locked prevention
action set.

**Normalized Prevention Actions --- Coverage Table**

  ---------------------------------------------------------------------
  **Prevention Action**                           **Count**   **% of
                                                              Total**
  ----------------------------------------------- ----------- ---------
  Verify platform legitimacy before use           23          41.8

  Avoid unsolicited messages calls and DMs        6           10.9

  Never share recovery phrases or private keys    2           3.6

  Do not pay fees to unlock withdrawals           2           3.6

  Use hardware wallets for long term storage      5           9.1

  Enable strong authentication and account        4           7.3
  security                                                    

  Confirm network and address compatibility       5           9.1
  before transfers                                            

  Test transactions with small amounts first      5           9.1

  Limit browser extensions and keep browsers      1           1.8
  updated                                                     

  Revoke token approvals and review permissions   6           10.9
  regularly                                                   

  Maintain complete transaction and tax records   0           0.0

  Minimize public exposure of crypto holdings     0           0.0
  ---------------------------------------------------------------------

**Key Findings**

The most frequently mapped prevention action was Verify platform
legitimacy before use, appearing in 41.8% of incidents. Avoid
unsolicited messages calls and DMs and Revoke token approvals and review
permissions regularly were tied as the second most common prevention
actions by coverage. Several prevention actions appeared infrequently or
not at all, including Maintain complete transaction and tax records and
Minimize public exposure of crypto holdings, both with zero observed
mappings.

**Top Prevention Actions by Coverage**

  -----------------------------------------------------------------------
  **Rank**   **Prevention Action**                         **Coverage**
  ---------- --------------------------------------------- --------------
  1          Verify platform legitimacy before use         41.8%

  2          Avoid unsolicited messages calls and DMs      10.9%

  3          Revoke token approvals and review permissions 10.9%
             regularly                                     
  -----------------------------------------------------------------------

Combined coverage of the top three prevention actions: 63.6%.

**Interpretation**

The prevention distribution is concentrated around legitimacy
verification and interaction hygiene. Several incidents contained
prevention text that could not be mapped conservatively to the locked
prevention action set, limiting measurable coverage. Classification
warnings were present in a small subset of incidents and were handled
conservatively during normalization.

**Role in the Weekly Series**

This report serves as a weekly snapshot of normalized prevention
coverage across the incident dataset. It supports longitudinal
comparison by preserving stable prevention action definitions,
deterministic mappings, and reproducible coverage metrics across
reporting periods.

**Bottom Line**

The dataset shows a measurable concentration around legitimacy
verification and interaction-related prevention language, while several
incidents contained prevention text that remained unmappable under the
locked action framework. The report measures explicit prevention
coverage only and does not attempt to infer unstated guidance or
completeness.
