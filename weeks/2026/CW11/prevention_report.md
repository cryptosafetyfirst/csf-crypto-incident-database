**Prevention Action Normalization Report**

**Dataset Scope**

Total incidents analyzed: **49**

------------------------------------------------------------------------

**Input Integrity & Data Checks**

  ---------------------------------------------------------
  **Check**               **Result**
  ----------------------- ---------------------------------
  Schema Presence         All required fields present in
                          all records

  Entry Number Integrity  All entry numbers unique integers

  Classification Warning  7 records contain classification
  Audit                   warnings
  ---------------------------------------------------------

Records with classification_warning ≠ none: **7**

Affected entry numbers: **5, 18, 29, 41, 46, 48, 49**

Missing prevention text: **0 records**

Present but unmappable prevention text: **5 records**

Affected entry numbers: **3, 12, 19, 27, 38**

Coverage values therefore represent a **lower bound** because some
prevention guidance could not be normalized to the locked action set.

------------------------------------------------------------------------

**Normalized Prevention Actions --- Coverage Table**

  --------------------------------------------------------------------------------
  **Prevention Action**                  **Count**   **Entry Numbers**   **% of
                                                                         Total**
  -------------------------------------- ----------- ------------------- ---------
  Verify platform legitimacy before use  9           1, 6, 13, 14, 20,   18.4
                                                     32, 35, 42, 47      

  Avoid unsolicited messages calls and   6           2, 7, 11, 26, 30,   12.2
  DMs                                                45                  

  Never share recovery phrases or        2           10, 23              4.1
  private keys                                                           

  Do not pay fees to unlock withdrawals  5           16, 28, 39, 40, 46  10.2

  Use hardware wallets for long term     1           19                  2.0
  storage                                                                

  Enable strong authentication and       3           15, 22, 36          6.1
  account security                                                       

  Confirm network and address            4           25, 43, 44, 41      8.2
  compatibility before transfers                                         

  Test transactions with small amounts   3           21, 24, 34          6.1
  first                                                                  

  Limit browser extensions and keep      1           8                   2.0
  browsers updated                                                       

  Revoke token approvals and review      2           29, 49              4.1
  permissions regularly                                                  

  Maintain complete transaction and tax  2           27, 33              4.1
  records                                                                

  Minimize public exposure of crypto     1           37                  2.0
  holdings                                                               
  --------------------------------------------------------------------------------

------------------------------------------------------------------------

**Prevention Insights**

Top three prevention actions by coverage:

  -------------------------------------------------------------------
  **Rank**   **Prevention Action**              **Count**   **% of
                                                            Total**
  ---------- ---------------------------------- ----------- ---------
  1          Verify platform legitimacy before  9           18.4
             use                                            

  2          Avoid unsolicited messages calls   6           12.2
             and DMs                                        

  3          Do not pay fees to unlock          5           10.2
             withdrawals                                    
  -------------------------------------------------------------------

Combined coverage of the top three actions: **40.8% of total incidents**

Coverage interpretation constraints:

- **Classification warnings are present in 7 incidents**, requiring
  conservative normalization.

- **Five incidents contain prevention guidance that could not be
  mapped** to the locked action set.

- No mapped actions conflict with the locked prevention guidance set.

------------------------------------------------------------------------

**Observational Notes**

  -----------------------------------------------------------------------
  **Observation**      **Details**
  -------------------- --------------------------------------------------
  Prevention coverage  Most mapped actions relate to platform legitimacy,
  concentration        unsolicited contact avoidance, and withdrawal fee
                       scams

  Long-tail prevention Several actions appear only once or twice,
  distribution         reflecting diverse incident mechanisms

  Mapping limitations  A small portion of prevention text is narrative or
                       incompatible with the locked action set
  -----------------------------------------------------------------------

------------------------------------------------------------------------

**Summary**

The dataset demonstrates a **moderate concentration of prevention
guidance** around three primary actions---platform verification,
unsolicited contact avoidance, and withdrawal fee scams---covering
**40.8% of incidents**.

However, normalization coverage is partially constrained by
classification warnings and a small number of prevention statements that
cannot be mapped to the locked action set.
