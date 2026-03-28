**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 33

------------------------------------------------------------------------

**Input Integrity & QC Checks**

- **Schema Presence Check:** No missing fields detected.

- **Entry Number Integrity:** All entry numbers are unique integers with
  no duplicates or gaps.

- **Taxonomy Validity Check:**

  - Invalid subtype detected in entries: 12, 33

  - Invalid values: ponzi_scheme, approval_misunderstanding

- **Classification Warning Audit:**

  - Records with classification_warning ≠ none: 4

  - Affected entry numbers: 12, 22, 30, 33

------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           21          63.6

  hack           6           18.2

  user_mistake   6           18.2
  ------------------------------------

------------------------------------------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      0                         0.0

  malware                      2           9,22          6.1

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           0                         0.0

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            1           25            3.0

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   0                         0.0

  exchange_vulnerability       0                         0.0

  insider_attack               1           32            3.0

  wallet_software_exploit      1           5             3.0
  ------------------------------------------------------------------------

**Insight (Hack Subcategories):**\
A single dominant subcategory exists: malware.\
Insights are affected by classification warnings.

------------------------------------------------------------------------

**Scam Subcategories**

  -----------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers** **% of Total
                                                        Incidents**
  ----------------------- ----------- ----------------- -----------------
  social_engineering      3           1,17,23           9.1

  phishing                3           10,18,24          9.1

  social_media_scam       0                             0.0

  crypto_wallet_scam      6           4,7,15,16,19,27   18.2

  smart_contract_scam     0                             0.0

  fake_app_or_extension   0                             0.0

  exchange_scam           2           29,31             6.1

  token_launch_scam       1           30                3.0

  pump_dump               0                             0.0

  rug_pull                0                             0.0

  airdrop_scam            0                             0.0

  nft_scam                0                             0.0

  sim_swap                0                             0.0

  job_scam                3           2,3,26            9.1

  blackmail_extortion     0                             0.0

  romance_scam            2           8,11              6.1
  -----------------------------------------------------------------------

**Insight (Scam Subcategories):**\
A single dominant subcategory exists: crypto_wallet_scam.\
Insights are affected by classification warnings.

------------------------------------------------------------------------

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  4           6,13,20,21    12.1

  seed_phrase_exposure           1           28            3.0

  approval_misunderstanding      0                         0.0

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             1           14            3.0

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
A single dominant subcategory exists: wrong_network.\
Insights are not affected by classification warnings.

------------------------------------------------------------------------

**Classification Warning Audit**

Records with classification_warning ≠ none: 4\
Affected entry numbers: 12, 22, 30, 33

------------------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (63.6% of incidents).\
2️⃣ Top three subcategories overall: crypto_wallet_scam; wrong_network;
job_scam.\
3️⃣ Upper-bound prevention relevance estimate: 63.6%.
