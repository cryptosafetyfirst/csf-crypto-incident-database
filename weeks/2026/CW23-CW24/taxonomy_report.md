**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 86

**Input Integrity & QC Checks**

**Schema Presence Check**

All records contain the required fields:

- entry_number

- incident_type

- incident_subtype

- classification_warning

**Entry Number Integrity**

- Entry numbers are unique integers.

- No duplicate entry numbers detected.

**Taxonomy Validity Check**

- No invalid incident_type values detected.

- No invalid incident_subtype values detected.

**Classification Warning Audit**

Records with classification_warning ≠ none: 14

Affected entry numbers:

6, 9, 20, 21, 35, 38, 44, 62, 68, 70, 72, 73, 74, 79

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           62          72.1

  user_mistake   15          17.4

  hack           9           10.5
  ------------------------------------

**Hack Subcategories**

  ----------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry Numbers** **% of Total
                                                             Incidents**
  ---------------------------- ----------- ----------------- -----------------
  social_engineering_hack      0                             0.0

  malware                      0                             0.0

  trojan                       0                             0.0

  spyware                      0                             0.0

  keylogger                    0                             0.0

  clipboard_hijacker           0                             0.0

  ransomware                   0                             0.0

  cryptojacking                0                             0.0

  network_mitm                 0                             0.0

  wifi_sniffing                0                             0.0

  dns_spoofing                 0                             0.0

  session_hijacking            1           70                1.2

  ssl_stripping                0                             0.0

  fake_app_or_extension_hack   0                             0.0

  exchange_vulnerability       1           9                 1.2

  insider_attack               0                             0.0

  wallet_software_exploit      6           62, 68, 72, 74,   7.0
                                           78, 79            
  ----------------------------------------------------------------------------

**Insight (Hack Subcategories):**

A single dominant subcategory exists: wallet_software_exploit.

Insights are partially affected by classification warnings.

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**                **% of Total
                                                                       Incidents**
  ----------------------- ----------- -------------------------------- -------------
  social_engineering      17          3, 12, 23, 25, 26, 27, 33, 35,   19.8
                                      36, 47, 51, 56, 57, 58, 61, 76,  
                                      82                               

  phishing                10          2, 7, 10, 13, 21, 22, 34, 39,    11.6
                                      46, 77                           

  social_media_scam       2           75, 81                           2.3

  crypto_wallet_scam      2           28, 31                           2.3

  smart_contract_scam     2           24, 48                           2.3

  fake_app_or_extension   0                                            0.0

  exchange_scam           11          8, 15, 20, 32, 53, 54, 55, 64,   12.8
                                      69, 71, 84                       

  token_launch_scam       0                                            0.0

  pump_dump               0                                            0.0

  rug_pull                0                                            0.0

  airdrop_scam            1           80                               1.2

  nft_scam                0                                            0.0

  sim_swap                0                                            0.0

  job_scam                9           1, 4, 11, 14, 16, 50, 66, 83, 86 10.5

  blackmail_extortion     0                                            0.0

  romance_scam            3           5, 6, 65                         3.5
  ----------------------------------------------------------------------------------

**Insight (Scam Subcategories):**

A single dominant subcategory exists: social_engineering.

Insights are partially affected by classification warnings.

**User Mistake Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry Numbers**      **% of Total
                                                                    Incidents**
  ------------------------------ ----------- ---------------------- ----------------
  wrong_address                  1           17                     1.2

  wrong_network                  2           52, 59                 2.3

  seed_phrase_exposure           0                                  0.0

  approval_misunderstanding      0                                  0.0

  backup_failure                 0                                  0.0

  address_poisoning_copy_paste   1           67                     1.2

  lost_wallet_access             8           18, 19, 29, 30, 37,    9.3
                                             60, 63, 85             

  poor_wallet_backup_practice    0                                  0.0

  tax_recordkeeping              1           73                     1.2
  ----------------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**

A single dominant subcategory exists: lost_wallet_access.

Insights are partially affected by classification warnings.

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (72.1% of incidents).

2️⃣ Top three subcategories overall:

- social_engineering (17)

- exchange_scam (11)

- phishing (10)

3️⃣ Upper-bound prevention relevance estimate: 72.1%.
