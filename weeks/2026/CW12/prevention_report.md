**Prevention Action Normalization Report**

**Dataset Scope**

Total incidents analyzed: 43.

**Input Integrity Checks**

Schema presence check: all 43 records contain all required fields.

Entry number integrity: all entry_number values are unique integers. No
duplicates or non-integer values detected.

Classification warning audit: 4 records contain classification_warning
values not equal to none.\
Affected entry numbers: 3, 4, 7, 14.

Normalization proceeded conservatively for these records.

**Prevention Action Normalization**

  ---------------------------------------------------------------------------------
  **Prevention Action**         **Count**   **Entry Numbers**             **% of
                                                                          Total**
  ----------------------------- ----------- ----------------------------- ---------
  Verify platform legitimacy    20          1, 2, 5, 6, 7, 9, 11, 12, 13, 46.5
  before use                                17, 18, 24, 25, 28, 31, 32,   
                                            36, 39, 40, 43                

  Avoid unsolicited messages    11          3, 10, 17, 24, 25, 30, 33,    25.6
  calls and DMs                             39, 40, 42, 43                

  Never share recovery phrases  6           4, 13, 15, 19, 20, 38         14.0
  or private keys                                                         

  Do not pay fees to unlock     1           31                            2.3
  withdrawals                                                             

  Use hardware wallets for long 0                                         0.0
  term storage                                                            

  Enable strong authentication  0                                         0.0
  and account security                                                    

  Confirm network and address   4           11, 29, 34, 41                9.3
  compatibility before                                                    
  transfers                                                               

  Test transactions with small  4           2, 6, 9, 28                   9.3
  amounts first                                                           

  Limit browser extensions and  0                                         0.0
  keep browsers updated                                                   

  Revoke token approvals and    4           3, 16, 22, 35                 9.3
  review permissions regularly                                            

  Maintain complete transaction 1           27                            2.3
  and tax records                                                         

  Minimize public exposure of   0                                         0.0
  crypto holdings                                                         
  ---------------------------------------------------------------------------------

**Prevention Insights**

Top 3 prevention actions by coverage:

1.  Verify platform legitimacy before use (20)

2.  Avoid unsolicited messages calls and DMs (11)

3.  Never share recovery phrases or private keys (6)

Combined coverage of top 3 actions: 86.1% of total incidents.

Coverage is affected by classification warnings, as 4 records required
conservative interpretation.

No records contained missing prevention text.

Several records contain partially vague or mixed prevention guidance,
but all included at least one mappable action. No fully unmappable
prevention text cases were identified.

No conflicts with previously established prevention action definitions
were observed.
