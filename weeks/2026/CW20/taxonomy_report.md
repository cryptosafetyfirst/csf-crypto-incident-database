**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 55

**Input Integrity & QC Checks**

**Schema Presence Check**

  ----------------------------------
  **Check**           **Result**
  ------------------- --------------
  Missing required    0 affected
  fields              records

  Affected entry      None
  numbers             
  ----------------------------------

**Entry Number Integrity**

  ----------------------------------
  **Check**             **Result**
  --------------------- ------------
  Duplicate entry       None
  numbers               

  Non-integer entry     None
  numbers               

  Gaps detected         None
  ----------------------------------

**Taxonomy Validity Check**

  --------------------------------------
  **Check**                 **Result**
  ------------------------- ------------
  Invalid incident_type     None
  values                    

  Invalid incident_subtype  None
  values                    

  Affected entry numbers    None
  --------------------------------------

**Classification Warning Audit**

  ----------------------------------------------
  **Metric**                         **Value**
  ---------------------------------- -----------
  Records with                       3
  classification_warning ≠ none      

  Affected entry numbers             34, 44, 50
  ----------------------------------------------

Taxonomy pressure signal detected due to repeated non-none warning
patterns.

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           35          63.6

  hack           13          23.6

  user_mistake   7           12.7
  ------------------------------------

**Hack Subcategories**

  --------------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry Numbers**      **% of Total
                                                                  Incidents**
  ---------------------------- ----------- ---------------------- ----------------
  social_engineering_hack      2           27,33                  3.6

  malware                      0                                  0.0

  trojan                       0                                  0.0

  spyware                      1           54                     1.8

  keylogger                    0                                  0.0

  clipboard_hijacker           0                                  0.0

  ransomware                   0                                  0.0

  cryptojacking                0                                  0.0

  network_mitm                 1           15                     1.8

  wifi_sniffing                0                                  0.0

  dns_spoofing                 0                                  0.0

  session_hijacking            2           19,36                  3.6

  ssl_stripping                0                                  0.0

  fake_app_or_extension_hack   0                                  0.0

  exchange_vulnerability       0                                  0.0

  insider_attack               0                                  0.0

  wallet_software_exploit      7           11,14,17,23,25,32,46   12.7
  --------------------------------------------------------------------------------

**Insight (Hack Subcategories):**\
A single dominant subcategory exists: wallet_software_exploit.\
Insights are not materially affected by classification warnings.

**Scam Subcategories**

  --------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**           **% of Total
                                                                  Incidents**
  ----------------------- ----------- --------------------------- ----------------
  social_engineering      4           22,40,42,55                 7.3

  phishing                7           2,13,24,26,29,37,39         12.7

  social_media_scam       0                                       0.0

  crypto_wallet_scam      3           8,21,53                     5.5

  smart_contract_scam     0                                       0.0

  fake_app_or_extension   1           41                          1.8

  exchange_scam           9           3,16,20,30,34,35,44,47,50   16.4

  token_launch_scam       1           51                          1.8

  pump_dump               1           49                          1.8

  rug_pull                1           45                          1.8

  airdrop_scam            2           5,12                        3.6

  nft_scam                0                                       0.0

  sim_swap                1           28                          1.8

  job_scam                2           9,31                        3.6

  blackmail_extortion     0                                       0.0

  romance_scam            3           38,43,48                    5.5
  --------------------------------------------------------------------------------

**Insight (Scam Subcategories):**\
A single dominant subcategory exists: exchange_scam.\
Insights are partially affected by classification warnings.

**User Mistake Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry      **% of Total
                                             Numbers**    Incidents**
  ------------------------------ ----------- ------------ ----------------
  wrong_address                  1           52           1.8

  wrong_network                  1           4            1.8

  seed_phrase_exposure           1           18           1.8

  approval_misunderstanding      0                        0.0

  backup_failure                 0                        0.0

  address_poisoning_copy_paste   1           6            1.8

  lost_wallet_access             3           1,7,10       5.5

  poor_wallet_backup_practice    0                        0.0

  tax_recordkeeping              0                        0.0
  ------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
A single dominant subcategory exists: lost_wallet_access.\
Insights are not materially affected by classification warnings.

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (63.6% of incidents).

2️⃣ Top three subcategories overall: exchange_scam; phishing;
wallet_software_exploit.

3️⃣ Upper-bound prevention relevance estimate: 63.6%.
