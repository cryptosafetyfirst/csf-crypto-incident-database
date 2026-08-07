**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

**Total incidents analyzed:** 62

**Input Integrity & QC Checks**

  -------------------------------------------
  **Check**              **Result**
  ---------------------- --------------------
  Required fields        Present in all 62
                         records

  Entry number           Pass
  uniqueness             

  Entry number sequence  Pass

  Non-integer entry      None
  numbers                

  Invalid incident types None

  Invalid incident       None
  subtypes               

  Classification         33 records
  warnings               
  -------------------------------------------

**Records with classification warnings:** 33\
**Affected entry numbers:** 1, 2, 6, 9, 10, 12, 13, 15, 16, 18, 21, 23,
24, 28, 29, 30, 32, 34, 37, 38, 39, 40, 43, 44, 45, 47, 48, 52, 56, 58,
59, 61, 62

The taxonomy requires zero-fill representation of all defined
subcategories and explicit disclosure of classification warnings.

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           32          51.6

  hack           15          24.2

  user_mistake   15          24.2
  ------------------------------------

**Hack Subcategories**

  -----------------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry Numbers**           **% of Total
                                                                       Incidents**
  ---------------------------- ----------- --------------------------- --------------
  social_engineering_hack      0                                       0.0

  malware                      0                                       0.0

  trojan                       0                                       0.0

  spyware                      0                                       0.0

  keylogger                    0                                       0.0

  clipboard_hijacker           0                                       0.0

  ransomware                   0                                       0.0

  cryptojacking                0                                       0.0

  network_mitm                 1           47                          1.6

  wifi_sniffing                0                                       0.0

  dns_spoofing                 0                                       0.0

  session_hijacking            1           48                          1.6

  ssl_stripping                0                                       0.0

  fake_app_or_extension_hack   0                                       0.0

  exchange_vulnerability       0                                       0.0

  insider_attack               0                                       0.0

  wallet_software_exploit      13          20, 21, 23, 29, 32, 37, 39, 21.0
                                           40, 44, 45, 56, 60, 62      
  -----------------------------------------------------------------------------------

**Insight:** A single dominant hack subcategory exists:
**wallet_software_exploit**, with 13 incidents representing 21.0% of the
total dataset and 86.7% of all hack incidents. This insight is affected
by classification warnings because multiple records within this
subcategory contain warnings.

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**            **% of Total
                                                                   Incidents**
  ----------------------- ----------- ---------------------------- -----------------
  social_engineering      7           2, 6, 7, 9, 15, 38, 52       11.3

  phishing                7           4, 11, 14, 18, 19, 43, 57    11.3

  social_media_scam       0                                        0.0

  crypto_wallet_scam      2           13, 42                       3.2

  smart_contract_scam     1           49                           1.6

  fake_app_or_extension   1           54                           1.6

  exchange_scam           10          1, 10, 12, 30, 31, 33, 35,   16.1
                                      36, 41, 61                   

  token_launch_scam       1           5                            1.6

  pump_dump               0                                        0.0

  rug_pull                0                                        0.0

  airdrop_scam            1           34                           1.6

  nft_scam                0                                        0.0

  sim_swap                0                                        0.0

  job_scam                1           50                           1.6

  blackmail_extortion     0                                        0.0

  romance_scam            1           24                           1.6
  ----------------------------------------------------------------------------------

**Insight:** A single dominant scam subcategory exists:
**exchange_scam**, with 10 incidents representing 16.1% of the total
dataset and 31.3% of scam incidents. **phishing** and
**social_engineering** are tied for second at 7 incidents each. The
insight is affected by classification warnings because several records
within the leading scam subcategories contain warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  2           17, 26        3.2

  wrong_network                  4           22, 25, 53,   6.5
                                             58            

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      2           27, 59        3.2

  backup_failure                 1           46            1.6

  address_poisoning_copy_paste   1           51            1.6

  lost_wallet_access             5           3, 8, 16, 28, 8.1
                                             55            

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

**Insight:** A single dominant user-mistake subcategory exists:
**lost_wallet_access**, with 5 incidents representing 8.1% of the total
dataset and 33.3% of user-mistake incidents. This insight is affected by
classification warnings because entries 16 and 28 carry classification
warnings.

**Classification Warning Audit**

  -----------------------------------------------
  **Metric**                          **Value**
  ----------------------------------- -----------
  Records with classification_warning 33
  ≠ none                              

  Records with classification_warning 29
  = none                              

  \% with classification warnings     53.2%
  -----------------------------------------------

**Affected entry numbers:** 1, 2, 6, 9, 10, 12, 13, 15, 16, 18, 21, 23,
24, 28, 29, 30, 32, 34, 37, 38, 39, 40, 43, 44, 45, 47, 48, 52, 56, 58,
59, 61, 62

Classification warnings are retained without changing the underlying
classifications, as required by the supplied analytical rules.

**Big-Picture Takeaways**

1.  **Dominant incident type:** **scam**, with 32 of 62 incidents
    (**51.6%**).

2.  **Top three subcategories overall:** **wallet_software_exploit** ---
    13 incidents; **exchange_scam** --- 10 incidents; **phishing** --- 7
    incidents. phishing and social_engineering are tied at 7; the
    required alphabetical tie-break places phishing third. The supplied
    methodology requires ranking by count and alphabetical resolution of
    ties.

3.  **Upper-bound prevention relevance estimate:** **51.6%**, based
    solely on the dominant incident type\'s share.
