**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 40

**Input Integrity & QC Checks**

**Schema Presence Check**

All records contain the required fields used for analysis.

**Entry Number Integrity**

  -----------------------------------
  **Check**              **Result**
  ---------------------- ------------
  Unique entry numbers   Pass

  Duplicate entry        None
  numbers                

  Non-integer entry      None
  numbers                

  Gaps detected          None
  -----------------------------------

**Taxonomy Validity Check**

  --------------------------------------------
  **Entry      **Invalid       **Field**
  Number**     Value**         
  ------------ --------------- ---------------
  15           exchange_scam   incident_type

  --------------------------------------------

Analysis continues using the provided values without correction.

**Classification Warning Audit**

Records with classification_warning ≠ none: 5

Affected entry numbers: 2, 5, 10, 11, 15

  ----------------------------------------------------
  **Entry      **Classification Warning**
  Number**     
  ------------ ---------------------------------------
  2            mixed wallet and onramp flow complexity

  5            insufficient detail to classify
               confidently

  10           mixed compromise details not fully
               disclosed

  11           mixed compromise origin not publicly
               confirmed

  15           mixed scam and technical vectors
  ----------------------------------------------------

**Incident Type Distribution**

  -------------------------------------
  **Incident      **Count**   **% of
  Type**                      Total**
  --------------- ----------- ---------
  scam            23          57.5

  user_mistake    10          25.0

  hack            6           15.0

  exchange_scam   1           2.5
  -------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      3           5, 10, 13     7.5

  malware                      1           7             2.5

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

  insider_attack               2           11, 12        5.0

  wallet_software_exploit      0                         0.0
  ------------------------------------------------------------------------

**Insight (Hack Subcategories):**\
A single dominant subcategory exists: social_engineering_hack.\
Insights are partially affected by classification warnings.

**Scam Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**  **% of Total
                                                         Incidents**
  ----------------------- ----------- ------------------ -----------------
  social_engineering      4           6, 17, 24, 40      10.0

  phishing                6           16, 20, 26, 27,    15.0
                                      31, 34             

  social_media_scam       0                              0.0

  crypto_wallet_scam      0                              0.0

  smart_contract_scam     1           33                 2.5

  fake_app_or_extension   0                              0.0

  exchange_scam           7           1, 9, 15, 18, 35,  17.5
                                      36, 37             

  token_launch_scam       0                              0.0

  pump_dump               0                              0.0

  rug_pull                0                              0.0

  airdrop_scam            1           22                 2.5

  nft_scam                0                              0.0

  sim_swap                0                              0.0

  job_scam                3           14, 30, 39         7.5

  blackmail_extortion     0                              0.0

  romance_scam            2           29, 38             5.0
  ------------------------------------------------------------------------

**Insight (Scam Subcategories):**\
A single dominant subcategory exists: exchange_scam.\
Insights are partially affected by classification warnings.

**User Mistake Subcategories**

  ----------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry         **% of Total
                                             Numbers**       Incidents**
  ------------------------------ ----------- --------------- -----------------
  wrong_address                  2           2, 23           5.0

  wrong_network                  6           4, 8, 19, 21,   15.0
                                             25, 28          

  seed_phrase_exposure           0                           0.0

  approval_misunderstanding      0                           0.0

  backup_failure                 1           32              2.5

  address_poisoning_copy_paste   0                           0.0

  lost_wallet_access             0                           0.0

  poor_wallet_backup_practice    1           3               2.5

  tax_recordkeeping              0                           0.0
  ----------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
A single dominant subcategory exists: wrong_network.\
Insights are partially affected by classification warnings.

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (57.5% of incidents).

2️⃣ Top three subcategories overall: exchange_scam; phishing;
wrong_network.

3️⃣ Upper-bound prevention relevance estimate: 57.5%.
