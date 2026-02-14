Taxonomy Report --- Dataset Analytics

------------------------------------------------------------------------

Dataset Scope\
Total incidents analyzed: 79

------------------------------------------------------------------------

Input Integrity & QC Checks

Schema Presence Check\
All 79 records contain the required fields:\
• entry_number\
• incident_type\
• incident_subtype\
• classification_warning\
✅ No missing fields detected.

------------------------------------------------------------------------

Entry Number Integrity\
• Entry numbers are integers.\
• Entry numbers are unique.\
• No duplicates detected.\
⚠️ Gaps may exist and are allowed.\
Entry numbers are run-scoped and not required to be contiguous.

------------------------------------------------------------------------

Taxonomy Validity Check\
No invalid taxonomy values detected.\
All incident_type and incident_subtype values conform to the locked
taxonomy.

------------------------------------------------------------------------

Classification Warning Audit\
• Records with classification_warning ≠ none: 7\
• Affected entry numbers: 33, 39, 40, 48, 62, 66, 73\
⚠️ Recurrent ambiguity patterns constitute an early taxonomy pressure
signal.

------------------------------------------------------------------------

Incident Type Distribution

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           57          72.2

  user_mistake   14          17.7

  hack           8           10.1
  ------------------------------------

Percentages are based on total incidents (79).

------------------------------------------------------------------------

Hack Subcategories

  ----------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of
                                           Numbers**     Total**
  ---------------------------- ----------- ------------- ---------
  social_engineering_hack      2           33, 39        2.5

  malware                      0                         0.0

  trojan                       1           69            1.3

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           1           14            1.3

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            0                         0.0

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   3           30, 40, 72    3.8

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      1           66            1.3
  ----------------------------------------------------------------

Insight (Hack Subcategories):\
A single dominant subcategory exists: fake_app_or_extension_hack.\
Insights are partially affected by classification warnings.

------------------------------------------------------------------------

Scam Subcategories

  ------------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**                      **% of
                                                                             Total**
  ----------------------- ----------- -------------------------------------- ---------
  social_engineering      15          3, 6, 9, 15, 20, 43, 68, 75, 78, 79,   19.0
                                      1, 12, 24, 35, 65                      

  phishing                6           23, 26, 73, 10, 5, 92                  7.6

  social_media_scam       15          13, 18, 25, 28, 35, 37, 42, 50, 64,    19.0
                                      70, 76, 77, 2, 8, 27                   

  crypto_wallet_scam      1           1                                      1.3

  smart_contract_scam     2           65, 71                                 2.5

  fake_app_or_extension   0                                                  0.0

  exchange_scam           18          2, 5, 8, 12, 17, 19, 22, 29, 34, 36,   22.8
                                      44, 45, 53, 57, 60, 63, 67, 74         

  token_launch_scam       1           27                                     1.3

  pump_dump               0                                                  0.0

  rug_pull                0                                                  0.0

  airdrop_scam            4           7, 10, 21, 60                          5.1

  nft_scam                0                                                  0.0

  sim_swap                0                                                  0.0

  job_scam                1           32                                     1.3

  blackmail_extortion     0                                                  0.0

  romance_scam            1           58                                     1.3
  ------------------------------------------------------------------------------------

Insight (Scam Subcategories):\
A single dominant subcategory exists: exchange_scam.\
Insights are partially affected by classification warnings.

------------------------------------------------------------------------

User Mistake Subcategories

  ------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of
                                             Numbers**     Total**
  ------------------------------ ----------- ------------- ---------
  wrong_address                  1           31            1.3

  wrong_network                  4           16, 46, 51,   5.1
                                             56            

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      0                         0.0

  backup_failure                 3           11, 47, 55    3.8

  address_poisoning_copy_paste   1           62            1.3

  lost_wallet_access             3           4, 52, 54     3.8

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              2           38, 41        2.5
  ------------------------------------------------------------------

Insight (User Mistake Subcategories):\
A single dominant subcategory exists: wrong_network.\
Insights are affected by classification warnings.

------------------------------------------------------------------------

Big-Picture Takeaways

1️⃣ Dominant incident type: scam (72.2% of incidents).\
2️⃣ Top three subcategories overall: exchange_scam; social_engineering;
social_media_scam.\
3️⃣ Upper-bound prevention relevance estimate: 72.2%.
