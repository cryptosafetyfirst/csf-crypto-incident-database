**Taxonomy Report --- Dataset Analytics**

**Input Integrity and QC Checks**

Schema presence check: all 41 records contain all required fields
(entry_number, incident_type, incident_subtype, classification_warning).

Entry number integrity: all entry_number values are unique integers. No
duplicates, gaps, or non-integer values were found.

Taxonomy validity check: all incident_type and incident_subtype values
match the locked taxonomy. No invalid values were found.

Classification warning audit: 2 records have classification_warning
values other than none. Affected entry numbers: 14, 20. Warning values
observed: insufficient detail on exploit mechanism; classification
inferred from behavior.

**Dataset Scope**

Total incidents analyzed: 41

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           25          61.0

  hack           4           9.8

  user_mistake   12          29.3
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

  exchange_vulnerability       1           16            2.4

  insider_attack               0                         0.0

  wallet_software_exploit      3           3, 14, 20     7.3
  ------------------------------------------------------------------------

Insight (Hack Subcategories): A single dominant subcategory exists:
wallet_software_exploit. Insights are affected by classification
warnings.

**Scam Subcategories**

  ---------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**     **% of Total
                                                            Incidents**
  ----------------------- ----------- --------------------- -----------------
  social_engineering      8           5, 9, 10, 18, 21, 24, 19.5
                                      34, 40                

  phishing                1           7                     2.4

  social_media_scam       4           15, 23, 27, 31        9.8

  crypto_wallet_scam      2           32, 35                4.9

  smart_contract_scam     1           37                    2.4

  fake_app_or_extension   0                                 0.0

  exchange_scam           6           1, 11, 12, 25, 33, 39 14.6

  token_launch_scam       0                                 0.0

  pump_dump               0                                 0.0

  rug_pull                0                                 0.0

  airdrop_scam            0                                 0.0

  nft_scam                0                                 0.0

  sim_swap                0                                 0.0

  job_scam                0                                 0.0

  blackmail_extortion     0                                 0.0

  romance_scam            2           2, 19                 4.9
  ---------------------------------------------------------------------------

Insight (Scam Subcategories): A single dominant subcategory exists:
social_engineering. Insights are not affected by classification
warnings.

**User Mistake Subcategories**

  ---------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry        **% of Total
                                             Numbers**      Incidents**
  ------------------------------ ----------- -------------- -----------------
  wrong_address                  0                          0.0

  wrong_network                  1           28             2.4

  seed_phrase_exposure           0                          0.0

  approval_misunderstanding      0                          0.0

  backup_failure                 1           36             2.4

  address_poisoning_copy_paste   1           41             2.4

  lost_wallet_access             6           4, 6, 8, 17,   14.6
                                             22, 38         

  poor_wallet_backup_practice    0                          0.0

  tax_recordkeeping              4           13, 26, 29, 30 9.8
  ---------------------------------------------------------------------------

Insight (User Mistake Subcategories): A single dominant subcategory
exists: lost_wallet_access. Insights are not affected by classification
warnings.

**Classification Warning Audit**

Records with classification_warning not equal to none: 2

  ----------------------------------------------
  **Entry      **Classification Warning**
  Number**     
  ------------ ---------------------------------
  14           insufficient detail on exploit
               mechanism

  20           classification inferred from
               behavior
  ----------------------------------------------

These warnings indicate taxonomy pressure signals within the hack
segment, concentrated in wallet_software_exploit.

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (61.0% of incidents).

2️⃣ Top three subcategories overall: social_engineering (8),
exchange_scam (6), lost_wallet_access (6).

3️⃣ Upper-bound prevention relevance estimate: 61.0%.
