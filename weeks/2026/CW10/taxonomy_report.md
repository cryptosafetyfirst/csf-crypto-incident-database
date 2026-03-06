**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 44

**Input Integrity & QC Checks**

Schema presence check: all 44 records contain all required fields.

Entry number integrity: all entry_number values are unique integers. No
duplicates, gaps, or non-integer values detected.

Taxonomy validity check: all incident_type and incident_subtype values
match the locked taxonomy.

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           29          65.9

  hack           9           20.5

  user_mistake   6           13.6
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry Numbers**   **% of Total
                                                               Incidents**
  ---------------------------- ----------- ------------------- -----------------
  social_engineering_hack      7           5, 20, 25, 32, 38,  15.9
                                           42, 44              

  malware                      0                               0.0

  trojan                       1           31                  2.3

  spyware                      0                               0.0

  keylogger                    0                               0.0

  clipboard_hijacker           0                               0.0

  ransomware                   0                               0.0

  cryptojacking                0                               0.0

  network_mitm                 0                               0.0

  wifi_sniffing                0                               0.0

  dns_spoofing                 0                               0.0

  session_hijacking            0                               0.0

  ssl_stripping                0                               0.0

  fake_app_or_extension_hack   1           2                   2.3

  exchange_vulnerability       0                               0.0

  insider_attack               0                               0.0

  wallet_software_exploit      0                               0.0
  ------------------------------------------------------------------------------

Insight: A single dominant subcategory exists: social_engineering_hack.
Insights are affected by classification warnings.

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**               **% of Total
                                                                      Incidents**
  ----------------------- ----------- ------------------------------- --------------
  social_engineering      16          1, 3, 4, 9, 10, 12, 15, 16, 18, 36.4
                                      23, 27, 30, 36, 39, 40, 43      

  phishing                2           11, 13                          4.5

  social_media_scam       1           7                               2.3

  crypto_wallet_scam      0                                           0.0

  smart_contract_scam     0                                           0.0

  fake_app_or_extension   0                                           0.0

  exchange_scam           5           14, 19, 24, 33, 37              11.4

  token_launch_scam       2           6, 26                           4.5

  pump_dump               1           21                              2.3

  rug_pull                0                                           0.0

  airdrop_scam            0                                           0.0

  nft_scam                0                                           0.0

  sim_swap                0                                           0.0

  job_scam                0                                           0.0

  blackmail_extortion     0                                           0.0

  romance_scam            2           22, 29                          4.5
  ----------------------------------------------------------------------------------

Insight: A single dominant subcategory exists: social_engineering.
Insights are affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  2           8, 17         4.5

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      1           28            2.3

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             1           34            2.3

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              2           35, 41        4.5
  --------------------------------------------------------------------------

Insight: No single dominant subcategory exists. Tied top subcategories:
tax_recordkeeping, wrong_network. Insights are affected by
classification warnings.

**Classification Warning Audit**

Records with classification_warning ≠ none: 8

Affected entry numbers: 6, 17, 19, 21, 29, 30, 33, 38

Observed warning values:

- taxonomy pressure resolved

- insufficient detail to classify confidently

A repeated warning pattern appears across multiple records: insufficient
detail to classify confidently. This is a taxonomy pressure signal.

**Big-Picture Takeaways**

1.  Dominant incident type: scam (65.9% of incidents).

2.  Top three subcategories overall: social_engineering (16),
    social_engineering_hack (7), exchange_scam (5).

3.  Upper-bound prevention relevance estimate: 65.9%.
