**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 37

**Input Integrity Checks**

  ---------------------------------------------------------
  **Check**              **Result**   **Affected Entry
                                      Numbers**
  ---------------------- ------------ ---------------------
  Missing required       0            
  fields                              

  Duplicate entry        0            
  numbers                             

  Entry number gaps      0            

  Non-integer entry      0            
  numbers                             

  Invalid taxonomy       2            19, 31
  values                              
  ---------------------------------------------------------

  ---------------------------------
  **Entry      **Invalid Value**
  Number**     
  ------------ --------------------
  19           scam /
               investment_scam

  31           scam /
               investment_scam
  ---------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           26          70.3

  hack           7           18.9

  user_mistake   4           10.8
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      2           22, 26        5.4

  malware                      1           5             2.7

  trojan                       1           16            2.7

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

  fake_app_or_extension_hack   0                         0.0

  exchange_vulnerability       0                         0.0

  insider_attack               2           12, 36        5.4

  wallet_software_exploit      1           37            2.7
  ------------------------------------------------------------------------

Insight: No single dominant subcategory exists. Tied subcategories:
insider_attack, social_engineering_hack. Insights are affected by
classification warnings.

**Scam Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**  **% of Total
                                                         Incidents**
  ----------------------- ----------- ------------------ -----------------
  social_engineering      6           3, 8, 17, 27, 28,  16.2
                                      32                 

  phishing                2           20, 23             5.4

  social_media_scam       1           1                  2.7

  crypto_wallet_scam      2           9, 11              5.4

  smart_contract_scam     1           35                 2.7

  fake_app_or_extension   0                              0.0

  exchange_scam           7           4, 7, 18, 21, 24,  18.9
                                      30, 34             

  token_launch_scam       0                              0.0

  pump_dump               0                              0.0

  rug_pull                1           2                  2.7

  airdrop_scam            0                              0.0

  nft_scam                0                              0.0

  sim_swap                0                              0.0

  job_scam                0                              0.0

  blackmail_extortion     1           29                 2.7

  romance_scam            3           15, 25, 33         8.1
  ------------------------------------------------------------------------

Insight: A single dominant subcategory exists: exchange_scam. Insights
are affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  3           6, 10, 14     8.1

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      0                         0.0

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             1           13            2.7

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

Insight: A single dominant subcategory exists: wrong_network. Insights
are not affected by classification warnings.

**Classification Warning Audit**

  -----------------------------------------------
  **Metric**                          **Value**
  ----------------------------------- -----------
  Records with classification_warning 8
  ≠ none                              

  -----------------------------------------------

  ---------------------------------------------------------------
  **Warning**                      **Entry Numbers**  **Count**
  -------------------------------- ------------------ -----------
  insufficient detail to classify  4, 5, 13, 22, 26,  7
  confidently                      30, 37             

  private key compromise details   36                 1
  limited                                             
  ---------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (70.3% of incidents).

2️⃣ Top three subcategories overall: exchange_scam; social_engineering;
romance_scam.

3️⃣ Upper-bound prevention relevance estimate: 70.3%.
