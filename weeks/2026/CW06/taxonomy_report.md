**Taxonomy Report --- Dataset Analytics**

------------------------------------------------------------------------

**Dataset Scope**

**Total incidents analyzed:** **56**

------------------------------------------------------------------------

**Input Integrity & QC Checks**

**Schema Presence Check**

All 56 records contain the required fields:

- entry_number

- incident_type

- incident_subtype

- classification_warning

✅ No missing fields detected.

------------------------------------------------------------------------

**Entry Number Integrity**

- Entry numbers are integers.

- Entry numbers are unique.

- No duplicates detected.

⚠️ Gaps may exist and are allowed.\
Entry numbers are run-scoped and not required to be contiguous.

------------------------------------------------------------------------

**Taxonomy Validity Check**

**Invalid taxonomy values detected (outside locked taxonomy):**

  -----------------------------------------------------
  **entry_number**   **invalid field**  **invalid
                                        value**
  ------------------ ------------------ ---------------
  37                 incident_type      exchange_scam

  37                 incident_subtype   Reddit
  -----------------------------------------------------

These records are **reported but not corrected** and remain included in
totals.

------------------------------------------------------------------------

**Classification Warning Audit**

- **Records with classification_warning ≠ none:** **3**

- **Affected entry numbers:** 9, 20, 37

⚠️ One record contained a missing / null warning field and was treated
as\
unknown_missing_warning_field.

⚠️ Recurrent ambiguity patterns constitute an **early taxonomy pressure
signal**.

------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           43          76.8

  user_mistake   7           12.5

  hack           5           8.9
  ------------------------------------

Percentages are based on total incidents (56).\
Invalid incident types are excluded from this table but disclosed above.

------------------------------------------------------------------------

**Hack Subcategories**

  ----------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of
                                           Numbers**     Total**
  ---------------------------- ----------- ------------- ---------
  social_engineering_hack      0                         0.0

  malware                      2           45, 52        3.6

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

  fake_app_or_extension_hack   1           15            1.8

  exchange_vulnerability       1           21            1.8

  insider_attack               0                         0.0

  wallet_software_exploit      1           55            1.8
  ----------------------------------------------------------------

**Insight (Hack Subcategories):**\
No single dominant subcategory exists.\
Top subcategories (tied): **exchange_vulnerability,
fake_app_or_extension_hack, malware, wallet_software_exploit** (listed
alphabetically).\
Insights are **affected by classification warnings**.

------------------------------------------------------------------------

**Scam Subcategories**

  ------------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**                      **% of
                                                                             Total**
  ----------------------- ----------- -------------------------------------- ---------
  social_engineering      9           1, 5, 9, 10, 14, 20, 23, 32, 41        16.1

  phishing                6           2, 6, 29, 30, 38                       10.7

  social_media_scam       1           50                                     1.8

  crypto_wallet_scam      0                                                  0.0

  smart_contract_scam     0                                                  0.0

  fake_app_or_extension   0                                                  0.0

  exchange_scam           19          12, 13, 17, 18, 19, 24, 25, 26, 28,    33.9
                                      31, 33, 34, 35, 36, 40, 42, 44, 47,    
                                      51, 53, 54                             

  token_launch_scam       2           4, 46                                  3.6

  pump_dump               0                                                  0.0

  rug_pull                0                                                  0.0

  airdrop_scam            4           3, 8, 27                               7.1

  nft_scam                0                                                  0.0

  sim_swap                0                                                  0.0

  job_scam                1           11                                     1.8

  blackmail_extortion     0                                                  0.0

  romance_scam            0                                                  0.0
  ------------------------------------------------------------------------------------

**Insight (Scam Subcategories):**\
A single dominant subcategory exists: **exchange_scam**.\
Insights are **affected by classification warnings**.

------------------------------------------------------------------------

**User Mistake Subcategories**

  ------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of
                                             Numbers**     Total**
  ------------------------------ ----------- ------------- ---------
  wrong_address                  0                         0.0

  wrong_network                  0                         0.0

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      0                         0.0

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   3           7, 22, 56     5.4

  lost_wallet_access             2           16, 43        3.6

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              2           39, 48        3.6
  ------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
A single dominant subcategory exists: **address_poisoning_copy_paste**.\
Insights are **not affected by classification warnings**.

------------------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ **Dominant incident type:** **scam** (76.8% of incidents).\
2️⃣ **Top three subcategories overall:** exchange_scam;
social_engineering; phishing.\
3️⃣ **Upper-bound prevention relevance estimate:** **76.8%**.
