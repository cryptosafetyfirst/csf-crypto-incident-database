**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 33

**Integrity Checks**

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

  Invalid taxonomy       0            
  values                              
  ---------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           29          87.9

  hack           2           6.1

  user_mistake   2           6.1
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      0                         0.0

  malware                      0                         0.0

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

  fake_app_or_extension_hack   0                         0.0

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      2           1, 27         6.1
  ------------------------------------------------------------------------

Insight: A single dominant hack subcategory exists:
wallet_software_exploit. Insights are affected by classification
warnings.

**Scam Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**  **% of Total
                                                         Incidents**
  ----------------------- ----------- ------------------ -----------------
  social_engineering      5           4, 8, 13, 21, 24   15.2

  phishing                3           5, 10, 31          9.1

  social_media_scam       1           14                 3.0

  crypto_wallet_scam      2           2, 33              6.1

  smart_contract_scam     4           7, 17, 18, 32      12.1

  fake_app_or_extension   1           29                 3.0

  exchange_scam           7           6, 9, 11, 12, 15,  21.2
                                      20, 28             

  token_launch_scam       2           23, 26             6.1

  pump_dump               1           25                 3.0

  rug_pull                0                              0.0

  airdrop_scam            1           22                 3.0

  nft_scam                0                              0.0

  sim_swap                0                              0.0

  job_scam                1           3                  3.0

  blackmail_extortion     0                              0.0

  romance_scam            1           30                 3.0
  ------------------------------------------------------------------------

Insight: A single dominant scam subcategory exists: exchange_scam.
Insights are affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  1           19            3.0

  seed_phrase_exposure           1           16            3.0

  approval_misunderstanding      0                         0.0

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             0                         0.0

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

Insight: No single dominant user mistake subcategory exists. Tied
subcategories: seed_phrase_exposure, wrong_network. Insights are
affected by classification warnings.

**Classification Warning Audit**

  -----------------------------------------------------------------------------
  **Metric**                            **Count**   **Entry Numbers**
  ------------------------------------- ----------- ---------------------------
  Records with classification_warning   13          1, 2, 3, 5, 13, 16, 18, 23,
  not equal to none                                 24, 25, 26, 27, 29

  Missing, null, or empty warning       0           
  fields                                            
  -----------------------------------------------------------------------------

  ----------------------------------------------------------------
  **Warning**                      **Count**   **Entry Numbers**
  -------------------------------- ----------- -------------------
  insufficient detail to classify  6           2, 16, 18, 23, 24,
  confidently                                  26, 27

  taxonomy pressure resolved       4           1, 3, 25, 29

  mixed scam and technical vectors 1           5

  multiple victims summarized      1           13
  ----------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam with 29 incidents and 87.9% of total
incidents.

2️⃣ Top three subcategories overall: exchange_scam, social_engineering,
smart_contract_scam.

3️⃣ Upper-bound prevention relevance estimate: 87.9%.
