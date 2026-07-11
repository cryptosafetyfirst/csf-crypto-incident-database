**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

**Total incidents analyzed:** 63

**Input Integrity & Quality Checks**

  -------------------------------------------------------------------------
  **Check**        **Result**
  ---------------- --------------------------------------------------------
  Schema presence  PASS --- all required fields present

  Entry number     PASS --- unique integer entry numbers (1--63)
  integrity        

  Taxonomy         PASS --- all incident types and subtypes match the
  validity         locked taxonomy

  Classification   28 records contain a classification warning other than
  warning audit    none: 2, 4, 6, 7, 8, 9, 11, 16, 17, 18, 19, 20, 22, 23,
                   35, 37, 40, 43, 47, 48, 50, 53, 54, 55, 56, 61, 62, 63.
                   Repeated warning patterns indicate taxonomy pressure
                   signals.
  -------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           51          81.0

  hack           5           7.9

  user_mistake   7           11.1
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      1           56            1.6

  malware                      0                         0.0

  trojan                       2           15, 51        3.2

  spyware                      1           37            1.6

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

  wallet_software_exploit      1           16            1.6
  ------------------------------------------------------------------------

**Insight (Hack Subcategories)**

A single dominant subcategory exists: **trojan**.\
Insights are partially affected by classification warnings.

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**               **% of Total
                                                                      Incidents**
  ----------------------- ----------- ------------------------------- --------------
  social_engineering      8           12, 24, 25, 31, 32, 40, 44, 61  12.7

  phishing                7           3, 29, 36, 45, 52, 57, 58       11.1

  social_media_scam       4           4, 11, 19, 50                   6.3

  crypto_wallet_scam      1           39                              1.6

  smart_contract_scam     5           14, 18, 46, 54, 63              7.9

  fake_app_or_extension   1           27                              1.6

  exchange_scam           17          2, 6, 7, 8, 9, 17, 20, 22, 23,  27.0
                                      28, 30, 33, 34, 35, 43, 53, 62  

  token_launch_scam       0                                           0.0

  pump_dump               0                                           0.0

  rug_pull                0                                           0.0

  airdrop_scam            0                                           0.0

  nft_scam                0                                           0.0

  sim_swap                0                                           0.0

  job_scam                3           1, 5, 38                        4.8

  blackmail_extortion     0                                           0.0

  romance_scam            5           13, 26, 42, 59, 60              7.9
  ----------------------------------------------------------------------------------

**Insight (Scam Subcategories)**

A single dominant subcategory exists: **exchange_scam**.\
Insights are partially affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  0                         0.0

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      2           47, 48        3.2

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   1           41            1.6

  lost_wallet_access             2           10, 55        3.2

  poor_wallet_backup_practice    1           21            1.6

  tax_recordkeeping              1           49            1.6
  --------------------------------------------------------------------------

**Insight (User Mistake Subcategories)**

No single dominant subcategory exists. The top subcategories are
**approval_misunderstanding** and **lost_wallet_access** (tie).\
Insights are partially affected by classification warnings.

**Classification Warning Audit**

  -----------------------------------------------------------------------
  **Metric**                  **Value**
  --------------------------- -------------------------------------------
  Records with                28
  classification_warning ≠    
  none                        

  Affected entry numbers      2, 4, 6, 7, 8, 9, 11, 16, 17, 18, 19, 20,
                              22, 23, 35, 37, 40, 43, 47, 48, 50, 53, 54,
                              55, 56, 61, 62, 63
  -----------------------------------------------------------------------

**Big-Picture Takeaways**

1.  **Dominant incident type:** **scam**, representing **81.0%** of all
    incidents.

2.  **Top three subcategories overall:** **exchange_scam** (17),
    **social_engineering** (8), **phishing** (7).

3.  **Upper-bound prevention relevance estimate:** **81.0%**.
