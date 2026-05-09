**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 27

**Input Integrity and QC Checks**

  ---------------------------------------------------------
  **Check**              **Result**   **Affected Entry
                                      Numbers**
  ---------------------- ------------ ---------------------
  Schema presence issues 0            

  Duplicate entry        0            
  numbers                             

  Entry number gaps      0            

  Non-integer entry      0            
  numbers                             

  Invalid taxonomy       0            
  values                              
  ---------------------------------------------------------

**Incident Type Distribution**

  --------------------------------------------
  **Incident     **Count**   **% of Total
  Type**                     Incidents**
  -------------- ----------- -----------------
  scam           17          63.0

  hack           6           22.2

  user_mistake   4           14.8
  --------------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      1           5             3.7

  malware                      0                         0.0

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           1           16            3.7

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            0                         0.0

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   0                         0.0

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      4           10, 11, 14,   14.8
                                           27            
  ------------------------------------------------------------------------

Insight: A single dominant subcategory exists: wallet_software_exploit.
Insights are affected by classification warnings.

**Scam Subcategories**

  -------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry       **% of Total
                                      Numbers**     Incidents**
  ----------------------- ----------- ------------- -----------------
  social_engineering      5           8, 9, 13, 18, 18.5
                                      20            

  phishing                1           4             3.7

  social_media_scam       0                         0.0

  crypto_wallet_scam      1           19            3.7

  smart_contract_scam     1           26            3.7

  fake_app_or_extension   0                         0.0

  exchange_scam           5           1, 2, 6, 24,  18.5
                                      25            

  token_launch_scam       0                         0.0

  pump_dump               0                         0.0

  rug_pull                0                         0.0

  airdrop_scam            0                         0.0

  nft_scam                0                         0.0

  sim_swap                0                         0.0

  job_scam                2           7, 12         7.4

  blackmail_extortion     0                         0.0

  romance_scam            2           3, 21         7.4
  -------------------------------------------------------------------

Insight: No single dominant subcategory exists. Tied subcategories:
exchange_scam, social_engineering. Insights are affected by
classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  1           23            3.7

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      1           17            3.7

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   2           15, 22        7.4

  lost_wallet_access             0                         0.0

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

Insight: A single dominant subcategory exists:
address_poisoning_copy_paste. Insights are partially affected by
classification warnings.

**Classification Warning Audit**

  ---------------------------------------------------------------------------
  **Metric**                          **Count**   **Affected Entry Numbers**
  ----------------------------------- ----------- ---------------------------
  Records with classification_warning 10          5, 8, 10, 11, 14, 17, 18,
  ≠ none                                          24, 26, 27

  ---------------------------------------------------------------------------

  ----------------------------------------------------------
  **Warning**                      **Count**   **Entry
                                               Numbers**
  -------------------------------- ----------- -------------
  insufficient detail to classify  5           5, 8, 11, 14,
  confidently                                  18

  mixed technical vectors          1           10

  taxonomy pressure resolved       1           17

  mixed community verification     1           24
  signals                                      

  insufficient loss detail         1           26

  initial compromise vector        1           27
  unknown                                      
  ----------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (63.0% of incidents).

2️⃣ Top three subcategories overall: exchange_scam; social_engineering;
wallet_software_exploit.

3️⃣ Upper-bound prevention relevance estimate: 63.0%.
