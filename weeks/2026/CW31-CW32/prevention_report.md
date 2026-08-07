**CW31 + CW32 Prevention Action Normalization Report**

**Scope:** CW31 + CW32 2026 Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** 62

**Purpose**

This report measures how prevention guidance recorded across the
incident dataset maps to a fixed set of standardized prevention actions.
Guidance is derived from the prevention text associated with the
incidents and normalized conservatively so that coverage can be compared
consistently across reporting periods.

**Methodology Summary**

Prevention actions were mapped from the prevention field only. Summary
and user-mistake information were used only where necessary to clarify
the meaning of the existing prevention text. Multiple prevention actions
may apply to a single incident, but an incident is counted no more than
once under the same action. Prevention language that is vague,
non-actionable, missing, or incompatible with the standardized action
set was not forced into a category.

**Data Integrity Notes**

  --------------------------------------------------------
  **Integrity Check**                         **Result**
  ------------------------------------------- ------------
  Total incidents analyzed                    62

  Required fields missing                     0

  Duplicate entry numbers                     0

  Non-integer entry numbers                   0

  Incidents with classification warnings      33

  Missing prevention text                     0

  Vague or non-actionable prevention text     1

  Present but unmappable prevention text      20

  Incidents mapped to at least one            41
  standardized action                         
  --------------------------------------------------------

Classification warnings occur in **33 of 62 incidents (53.2%)**,
requiring conservative treatment of the associated prevention mappings.

No incident has a missing prevention field. Entry **62** contains
none_obvious and therefore provides no actionable prevention text for
normalization. A further **20 incidents** contain concrete prevention
guidance that does not correspond to the standardized action set and was
therefore left unmapped rather than forced into an unrelated category.

Because vague/non-actionable and present-but-unmappable prevention text
exists, the standardized coverage figures represent a **lower bound** on
the prevention guidance contained in the dataset.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            12          19.4%

  Avoid unsolicited messages calls and DMs         13          21.0%

  Never share recovery phrases or private keys     2           3.2%

  Do not pay fees to unlock withdrawals            7           11.3%

  Use hardware wallets for long term storage       0           0.0%

  Enable strong authentication and account         2           3.2%
  security                                                     

  Confirm network and address compatibility before 6           9.7%
  transfers                                                    

  Test transactions with small amounts first       8           12.9%

  Limit browser extensions and keep browsers       0           0.0%
  updated                                                      

  Revoke token approvals and review permissions    0           0.0%
  regularly                                                    

  Maintain complete transaction and tax records    3           4.8%

  Minimize public exposure of crypto holdings      0           0.0%
  ----------------------------------------------------------------------

**Prevention Action Traceability**

  ------------------------------------------------------------------------------
  **Prevention Action**                  **Count**   **Entry Numbers**
  -------------------------------------- ----------- ---------------------------
  Verify platform legitimacy before use  12          1, 5, 10, 30, 31, 33, 35,
                                                     36, 41, 54, 57, 61

  Avoid unsolicited messages calls and   13          4, 6, 7, 11, 14, 15, 19,
  DMs                                                34, 38, 43, 49, 52, 56

  Never share recovery phrases or        2           54, 57
  private keys                                       

  Do not pay fees to unlock withdrawals  7           2, 9, 31, 35, 41, 42, 50

  Use hardware wallets for long term     0           
  storage                                            

  Enable strong authentication and       2           18, 48
  account security                                   

  Confirm network and address            6           17, 26, 27, 51, 53, 58
  compatibility before transfers                     

  Test transactions with small amounts   8           13, 14, 17, 26, 27, 33, 53,
  first                                              58

  Limit browser extensions and keep      0           
  browsers updated                                   

  Revoke token approvals and review      0           
  permissions regularly                              

  Maintain complete transaction and tax  3           21, 39, 40
  records                                            

  Minimize public exposure of crypto     0           
  holdings                                           
  ------------------------------------------------------------------------------

**Key Findings**

The most frequently represented standardized prevention action was
**Avoid unsolicited messages calls and DMs**, mapped to 13 incidents
(21.0%). **Verify platform legitimacy before use** followed with 12
incidents (19.4%), while **Test transactions with small amounts first**
mapped to 8 incidents (12.9%).

The next most represented actions were **Do not pay fees to unlock
withdrawals** with 7 incidents (11.3%) and **Confirm network and address
compatibility before transfers** with 6 incidents (9.7%).

Four standardized prevention actions received no mappings during this
reporting period: **Use hardware wallets for long term storage**,
**Limit browser extensions and keep browsers updated**, **Revoke token
approvals and review permissions regularly**, and **Minimize public
exposure of crypto holdings**.

**Top Prevention Actions by Coverage**

  -------------------------------------------------------------------
  **Rank**   **Prevention Action**              **Count**   **% of
                                                            Total**
  ---------- ---------------------------------- ----------- ---------
  1          Avoid unsolicited messages calls   13          21.0%
             and DMs                                        

  2          Verify platform legitimacy before  12          19.4%
             use                                            

  3          Test transactions with small       8           12.9%
             amounts first                                  
  -------------------------------------------------------------------

The top three actions account for **33 normalized action mappings,
equivalent to 53.2% of the 62-incident dataset when action coverage
percentages are combined**. Because individual incidents may map to more
than one action, this figure represents combined action coverage rather
than 33 necessarily distinct incidents.

**Interpretation**

Prevention coverage is concentrated most strongly around avoiding
unsolicited contact, verifying platforms before use, and testing
transactions with small amounts. The remaining mapped actions occur less
frequently across the dataset.

Coverage is affected by the presence of classification warnings in 33
incidents and by 21 incidents whose prevention fields did not produce a
standardized mapping. Consequently, absence from the standardized action
table does not establish absence of prevention guidance from the
underlying incident records.

No conflict between the mapped standardized actions and the prevention
guidance contained in the supplied dataset was identified.

**Role in the Weekly Series**

This report provides a standardized snapshot of prevention-action
coverage for the reporting period. Maintaining the same prevention
action set and normalization approach supports longitudinal comparison
and provides a consistent anchor for measuring how frequently
standardized prevention themes occur across weekly incident datasets.

**Bottom Line**

The strongest normalized prevention coverage in this 62-incident dataset
centers on **avoiding unsolicited contact, verifying platform
legitimacy, and testing transactions with small amounts**. Coverage
remains deliberately conservative: prevention language that could not be
mapped reliably to the standardized action set was left unmapped rather
than reinterpreted, preserving measurability and comparability over
completeness.
