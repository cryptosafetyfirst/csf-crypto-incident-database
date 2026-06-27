**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 74

**Input Integrity and QC Checks**

  ---------------------------------------------------------
  **Check**              **Result**   **Affected Entry
                                      Numbers**
  ---------------------- ------------ ---------------------
  Schema presence issues 0            none

  Duplicate entry        0            none
  numbers                             

  Entry number gaps      0            none

  Non-integer entry      0            none
  numbers                             

  Invalid taxonomy       0            none
  values                              
  ---------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           60          81.1

  hack           3           4.1

  user_mistake   11          14.9
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      1           35            1.4

  malware                      1           34            1.4

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           0                         0.0

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            0                         0.0

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   1           50            1.4

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      0                         0.0
  ------------------------------------------------------------------------

Insight: No single dominant hack subcategory exists. Tied subcategories:
fake_app_or_extension_hack, malware, social_engineering_hack. Insights
are affected by classification warnings.

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**                **% of Total
                                                                       Incidents**
  ----------------------- ----------- -------------------------------- -------------
  social_engineering      13          1, 10, 19, 24, 39, 42, 44, 48,   17.6
                                      52, 56, 59, 60, 69               

  phishing                7           6, 21, 27, 36, 45, 51, 67        9.5

  social_media_scam       3           20, 38, 40                       4.1

  crypto_wallet_scam      1           73                               1.4

  smart_contract_scam     1           55                               1.4

  fake_app_or_extension   0                                            0.0

  exchange_scam           19          4, 8, 17, 28, 29, 37, 41, 43,    25.7
                                      47, 53, 54, 57, 58, 61, 62, 63,  
                                      68, 71, 72                       

  token_launch_scam       1           3                                1.4

  pump_dump               1           70                               1.4

  rug_pull                0                                            0.0

  airdrop_scam            0                                            0.0

  nft_scam                0                                            0.0

  sim_swap                0                                            0.0

  job_scam                5           9, 16, 26, 32, 49                6.8

  blackmail_extortion     0                                            0.0

  romance_scam            9           2, 7, 11, 12, 13, 23, 30, 66, 74 12.2
  ----------------------------------------------------------------------------------

Insight: A single dominant scam subcategory exists: exchange_scam.
Insights are affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry Numbers**   **% of Total
                                                                 Incidents**
  ------------------------------ ----------- ------------------- -----------------
  wrong_address                  0                               0.0

  wrong_network                  0                               0.0

  seed_phrase_exposure           1           14                  1.4

  approval_misunderstanding      0                               0.0

  backup_failure                 0                               0.0

  address_poisoning_copy_paste   2           33, 65              2.7

  lost_wallet_access             7           5, 15, 18, 22, 25,  9.5
                                             31, 64              

  poor_wallet_backup_practice    0                               0.0

  tax_recordkeeping              1           46                  1.4
  --------------------------------------------------------------------------------

Insight: A single dominant user mistake subcategory exists:
lost_wallet_access. Insights are affected by classification warnings.

**Classification Warning Audit**

Records with classification_warning ≠ none: 41

Affected entry numbers: 1, 2, 4, 7, 8, 10, 11, 12, 13, 16, 17, 19, 23,
26, 28, 29, 30, 35, 37, 38, 39, 40, 41, 42, 43, 44, 46, 47, 48, 52, 53,
54, 57, 58, 60, 61, 62, 63, 68, 69, 73

  ------------------------------------------------------------------------------
  **Classification     **Count**   **Entry Numbers**
  Warning**                        
  -------------------- ----------- ---------------------------------------------
  insufficient detail  3           35, 52, 73
  to classify                      
  confidently                      

  taxonomy pressure    38          1, 2, 4, 7, 8, 10, 11, 12, 13, 16, 17, 19,
  resolved                         23, 26, 28, 29, 30, 37, 38, 39, 40, 41, 42,
                                   43, 44, 46, 47, 48, 53, 54, 57, 58, 60, 61,
                                   62, 63, 68, 69
  ------------------------------------------------------------------------------

Taxonomy pressure signal: taxonomy pressure resolved appears across
multiple records.

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (81.1% of incidents).

2️⃣ Top three subcategories overall: exchange_scam; social_engineering;
romance_scam.

3️⃣ Upper-bound prevention relevance estimate: 81.1%.
