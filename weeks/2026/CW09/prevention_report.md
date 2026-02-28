**Prevention Action Normalization Report**

**Input Integrity & Checks**

**Schema Presence Check**

- Records missing one or more required fields (entry_number,
  incident_type, incident_subtype, summary, user_mistake, prevention,
  classification_warning): **0**

- Affected entry_number values: *(none)*

**Entry Number Integrity**

- Non-integer entry_number values: **0**

- Duplicate entry_number values: **0**

- Affected entry_number values: *(none)*

**Classification Warning Audit**

- Records where classification_warning ≠ none: **4**

- Affected entry_number values: **7, 37, 49, 54**

- Records with missing/null/empty classification_warning: **0**

- Normalization proceeded conservatively for warning-bearing records.

------------------------------------------------------------------------

**Dataset Scope**

Total incidents analyzed: **76**

------------------------------------------------------------------------

**Prevention Action Normalization Table**

  --------------------------------------------------------------------------------
  **Prevention Action**         **Count**   **Entry Numbers**            **% of
                                                                         Total**
  ----------------------------- ----------- ---------------------------- ---------
  Verify platform legitimacy    18          3, 6, 10, 15, 16, 17, 19,    23.7
  before use                                24, 28, 31, 34, 35, 41, 42,  
                                            50, 51, 52, 53               

  Avoid unsolicited messages    14          4, 7, 20, 21, 22, 23, 29,    18.4
  calls and DMs                             36, 37, 38, 39, 55, 56, 76   

  Never share recovery phrases  9           6, 12, 18, 34, 35, 42, 49,   11.8
  or private keys                           50, 54                       

  Do not pay fees to unlock     11          3, 15, 17, 19, 24, 28, 41,   14.5
  withdrawals                               44, 45, 46, 47               

  Use hardware wallets for long 5           9, 49, 54, 61, 70            6.6
  term storage                                                           

  Enable strong authentication  12          5, 12, 13, 18, 26, 27, 36,   15.8
  and account security                      56, 58, 59, 60, 76           

  Confirm network and address   4           69, 72, 74, 75               5.3
  compatibility before                                                   
  transfers                                                              

  Test transactions with small  2           69, 72                       2.6
  amounts first                                                          

  Limit browser extensions and  3           5, 13, 58                    3.9
  keep browsers updated                                                  

  Revoke token approvals and    6           9, 10, 31, 49, 54, 70        7.9
  review permissions regularly                                           

  Maintain complete transaction 5           2, 63, 68, 71, 73            6.6
  and tax records                                                        

  Minimize public exposure of   4           1, 64, 66, 74                5.3
  crypto holdings                                                        
  --------------------------------------------------------------------------------

------------------------------------------------------------------------

**Unmappable & Missing Prevention Text Disclosure**

- Incidents with missing prevention text: **0**

- Incidents with present but vague or non-actionable prevention text:
  **6** (entries **8, 11, 25, 30, 32, 33**)

- Incidents with present but unmappable prevention text (incompatible
  with locked action set): **4** (entries **40, 44, 45, 48**)

- Coverage percentages therefore represent a **lower bound**, as
  unmappable cases were not forced into any action category.

------------------------------------------------------------------------

**Prevention Insights**

Top three prevention actions by coverage (ranked by count; ties
alphabetically):

1.  **Verify platform legitimacy before use** --- 18 (23.7%)

2.  **Avoid unsolicited messages calls and DMs** --- 14 (18.4%)

3.  **Enable strong authentication and account security** --- 12 (15.8%)

Combined coverage of top three actions: **57.9%**

Coverage is affected by:

- **Classification warnings** (4 records; mapped conservatively)

- **Vague prevention text** (6 records)

- **Unmappable prevention text** (4 records)

No mapped prevention actions conflict with previously published guidance
within the locked action set.

------------------------------------------------------------------------

**Governance Note**

This normalization artifact:

- strictly maps only explicitly stated prevention text,

- preserves zero-fill comparability across all 12 locked actions,

- surfaces ambiguity and unmappable guidance without reinterpretation,

- supports deterministic, longitudinal prevention coverage analysis.

No prevention actions were added, removed, renamed, or inferred beyond
the locked set.
