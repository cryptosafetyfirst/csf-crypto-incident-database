Taxonomy Report --- Dataset Analytics

------------------------------------------------------------------------

**Dataset Scope**

Total incidents analyzed: **63**

------------------------------------------------------------------------

**Input Integrity & QC Checks**

**Schema Presence Check**

- All required fields present in all records.

- Records with missing fields: **0**

**Entry Number Integrity**

- All entry_number values are unique integers.

- No duplicates, gaps, or non-integer values detected.

**Taxonomy Validity Check**

- All incident_type and incident_subtype values match the locked
  taxonomy.

- No invalid values detected.

**Classification Warning Audit**

- Records with classification_warning ≠ none: **2**

- Affected entry numbers: **16, 18**

------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           53          84.1

  hack           1           1.6

  user_mistake   9           14.3
  ------------------------------------

------------------------------------------------------------------------

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

  fake_app_or_extension_hack   1           56            1.6

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      0                         0.0
  ------------------------------------------------------------------------

**Insight (Hack Subcategories):**\
A single dominant subcategory exists: **fake_app_or_extension_hack**.\
Insights are not materially affected by classification warnings.

------------------------------------------------------------------------

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**              **% of Total
                                                                     Incidents**
  ----------------------- ----------- ------------------------------ ---------------
  social_engineering      8           25, 27, 31, 49, 52, 53, 55, 58 12.7

  phishing                5           2, 34, 42, 44, 63              7.9

  social_media_scam       5           1, 26, 30, 54, 61              7.9

  crypto_wallet_scam      2           23, 36                         3.2

  smart_contract_scam     0                                          0.0

  fake_app_or_extension   1           29                             1.6

  exchange_scam           13          7, 10, 17, 19, 21, 22, 32, 33, 20.6
                                      39, 45, 46, 48, 50             

  token_launch_scam       6           12, 16, 18, 20, 24, 62         9.5

  pump_dump               0                                          0.0

  rug_pull                2           9, 38                          3.2

  airdrop_scam            1           8                              1.6

  nft_scam                1           11                             1.6

  sim_swap                1           35                             1.6

  job_scam                1           13                             1.6

  blackmail_extortion     0                                          0.0

  romance_scam            3           6, 43, 60                      4.8
  ----------------------------------------------------------------------------------

**Insight (Scam Subcategories):**\
A single dominant subcategory exists: **exchange_scam**.\
Insights are partially affected by classification warnings (entries
**16, 18**).

------------------------------------------------------------------------

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  1           4             1.6

  wrong_network                  1           15            1.6

  seed_phrase_exposure           1           3             1.6

  approval_misunderstanding      0                         0.0

  backup_failure                 2           14, 28        3.2

  address_poisoning_copy_paste   3           37, 40, 41    4.8

  lost_wallet_access             1           47            1.6

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              3           5, 57, 59     4.8
  --------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
No single dominant subcategory exists.\
The following subcategories are tied for highest share (alphabetical):\
**address_poisoning_copy_paste; tax_recordkeeping**.\
Insights are not materially affected by classification warnings.

------------------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ Dominant incident type: **scam (84.1% of incidents).**\
2️⃣ Top three subcategories overall: **exchange_scam (13);
social_engineering (8); token_launch_scam (6).**\
3️⃣ Upper-bound prevention relevance estimate: **84.1%**
