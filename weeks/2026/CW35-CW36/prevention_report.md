**Prevention Action Normalization Report**

**Dataset Scope**

**Total incidents analyzed:** 73

**Input Integrity & Quality Control**

**Schema Presence**

All 73 records contain the required fields: entry_number, incident_type,
incident_subtype, summary, user_mistake, prevention, and
classification_warning.

**Entry Number Integrity**

All entry_number values are unique integers. No duplicate or non-integer
values are present.

**Classification Warning Audit**

**Records with classification_warning ≠ none:** 30

**Affected entry numbers:** 3, 8, 10, 12, 13, 14, 17, 20, 21, 22, 23,
24, 26, 27, 28, 29, 31, 32, 33, 36, 42, 49, 50, 58, 60, 61, 67, 70, 71,
72

Normalization was applied conservatively to records containing
classification warnings.

**Prevention Text Integrity**

**Missing prevention text:** 0 records

**Vague or non-actionable prevention text:** 1 record

**Affected entry number:** 42

**Present but unmappable prevention text:** 3 records

**Affected entry numbers:** 30, 34, 60

These records were not forced into prevention actions.

**Normalized Prevention Actions**

  ---------------------------------------------------------------------------------
  **Prevention Action**     **Count**   **Entry Numbers**                 **% of
                                                                          Total**
  ------------------------- ----------- --------------------------------- ---------
  Verify platform           28          1, 7, 9, 13, 14, 17, 20, 21, 24,  38.4
  legitimacy before use                 31, 35, 37, 41, 43, 44, 46, 47,   
                                        48, 52, 54, 55, 57, 58, 59, 63,   
                                        68, 71, 73                        

  Avoid unsolicited         14          6, 12, 19, 25, 26, 28, 29, 32,    19.2
  messages calls and DMs                33, 47, 48, 58, 62, 67            

  Never share recovery      11          3, 4, 8, 11, 16, 28, 35, 45, 52,  15.1
  phrases or private keys               53, 56                            

  Do not pay fees to unlock 13          6, 7, 10, 12, 19, 24, 31, 36, 39, 17.8
  withdrawals                           40, 61, 69, 70                    

  Use hardware wallets for  0                                             0.0
  long term storage                                                       

  Enable strong             1           62                                1.4
  authentication and                                                      
  account security                                                        

  Confirm network and       6           15, 18, 22, 23, 27, 51            8.2
  address compatibility                                                   
  before transfers                                                        

  Test transactions with    11          17, 18, 23, 25, 27, 37, 38, 44,   15.1
  small amounts first                   46, 49, 50                        

  Limit browser extensions  1           72                                1.4
  and keep browsers updated                                               

  Revoke token approvals    9           2, 5, 29, 41, 64, 65, 66, 71, 73  12.3
  and review permissions                                                  
  regularly                                                               

  Maintain complete         1           49                                1.4
  transaction and tax                                                     
  records                                                                 

  Minimize public exposure  1           67                                1.4
  of crypto holdings                                                      
  ---------------------------------------------------------------------------------

**Prevention Insights**

The top three prevention actions by coverage are:

1.  **Verify platform legitimacy before use** --- 28 incidents
    (**38.4%**)

2.  **Avoid unsolicited messages calls and DMs** --- 14 incidents
    (**19.2%**)

3.  **Do not pay fees to unlock withdrawals** --- 13 incidents
    (**17.8%**)

**Combined coverage:** **75.3% of total incidents**.

The combined percentage represents the sum of action-level coverage
percentages; individual incidents may map to more than one prevention
action.

Coverage is affected by **30 records with classification warnings**, **1
record with vague or non-actionable prevention text**, and **3 records
with present but unmappable prevention text**.

No prevention text is missing.

No mapped actions conflict with the supplied locked prevention guidance.
