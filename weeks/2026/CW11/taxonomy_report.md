**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: **49**

------------------------------------------------------------------------

**Input Integrity & QC Checks**

  -----------------------------------------------------------------
  **Check**               **Result**
  ----------------------- -----------------------------------------
  Schema Presence         All required fields present in all
                          records

  Entry Number Integrity  All entry numbers are unique integers

  Taxonomy Validity       All incident_type and incident_subtype
                          values valid

  Classification Warning  7 records contain classification warnings
  Audit                   
  -----------------------------------------------------------------

Records with classification_warning ≠ none: **7**

Affected entry numbers: **5, 18, 29, 41, 46, 48, 49**

------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           32          65.3

  user_mistake   11          22.4

  hack           6           12.2
  ------------------------------------

------------------------------------------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      0                         0.0

  malware                      1           24            2.0

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           1           34            2.0

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            0                         0.0

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   2           8, 18         4.1

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      1           33            2.0
  ------------------------------------------------------------------------

**Insight (Hack Subcategories):**\
A single dominant subcategory exists: **fake_app_or_extension_hack**.\
Insights are partially affected by classification warnings.

------------------------------------------------------------------------

**Scam Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**    **% of Total
                                                           Incidents**
  ----------------------- ----------- -------------------- -----------------
  social_engineering      7           2, 7, 10, 20, 23,    14.3
                                      37, 46               

  phishing                3           4, 12, 17            6.1

  social_media_scam       7           11, 26, 30, 31, 39,  14.3
                                      45, 47               

  crypto_wallet_scam      2           13, 28               4.1

  smart_contract_scam     3           29, 48, 49           6.1

  fake_app_or_extension   0                                0.0

  exchange_scam           7           1, 6, 14, 16, 32,    14.3
                                      35, 42               

  token_launch_scam       0                                0.0

  pump_dump               0                                0.0

  rug_pull                0                                0.0

  airdrop_scam            0                                0.0

  nft_scam                1           40                   2.0

  sim_swap                0                                0.0

  job_scam                0                                0.0

  blackmail_extortion     3           9, 21, 38            6.1

  romance_scam            0                                0.0
  --------------------------------------------------------------------------

**Insight (Scam Subcategories):**\
No single dominant subcategory exists. The following subcategories are
tied for highest share:\
**exchange_scam, social_engineering, social_media_scam**.\
Insights are partially affected by classification warnings.

------------------------------------------------------------------------

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  1           43            2.0

  wrong_network                  1           44            2.0

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      2           5, 41         4.1

  backup_failure                 1           19            2.0

  address_poisoning_copy_paste   1           25            2.0

  lost_wallet_access             2           15, 22        4.1

  poor_wallet_backup_practice    1           36            2.0

  tax_recordkeeping              2           3, 27         4.1
  --------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
No single dominant subcategory exists. The following subcategories are
tied for highest share:\
**approval_misunderstanding, lost_wallet_access, tax_recordkeeping**.\
Insights are partially affected by classification warnings.
