**Taxonomy Report --- Dataset Analytics**

**Input Integrity & QC Checks**

**Schema Presence Check**

- Records missing one or more required fields (entry_number,
  incident_type, incident_subtype, classification_warning): **0**

- Affected entry_number values: *(none)*

**Entry Number Integrity**

- Non-integer entry_number values: **0**

- Duplicate entry_number values: **0**

- Gaps detected in entry_number sequence (within min..max of provided
  set): **0**

- Affected values: *(none)*

**Taxonomy Validity Check (Locked Taxonomy)**

- Records with invalid taxonomy values: **13**

- Affected entry_number values: **7, 8, 11, 25, 30, 32, 33, 40, 44, 45,
  46, 47, 48**

- Invalid values observed (incident_subtype): **advance_fee_scam;
  fake_crypto_platform; investment_scam; pig_butchering;
  smart_contract_drain; telegram_bot_scam**

- No reclassification performed.

**Classification Warning Audit**

- Records where classification_warning ≠ none: **4**

- Affected entry_number values: **7, 37, 49, 54**

- Records with missing/null/empty classification_warning: **0**

- Observed recurring warning string within dataset: **taxonomy pressure
  resolved** (3 occurrences)

------------------------------------------------------------------------

**Dataset Scope**

Total incidents analyzed: **76**

------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           50          65.8

  user_mistake   15          19.7

  hack           11          14.5
  ------------------------------------

------------------------------------------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      1           76            1.3

  malware                      3           13, 27, 58    3.9

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           1           5             1.3

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            0                         0.0

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   0                         0.0

  exchange_vulnerability       1           26            1.3

  insider_attack               0                         0.0

  wallet_software_exploit      5           9, 49, 54,    6.6
                                           61, 70        
  ------------------------------------------------------------------------

Insight (Hack Subcategories):\
A single dominant subcategory exists: **wallet_software_exploit**.\
Insights are affected by classification warnings (entries 49 and 54).

------------------------------------------------------------------------

**Scam Subcategories**

  -------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**   **% of Total
                                                          Incidents**
  ----------------------- ----------- ------------------- -----------------
  social_engineering      5           20, 21, 22, 23, 29  6.6

  phishing                5           12, 14, 18, 36, 56  6.6

  social_media_scam       3           4, 59, 60           3.9

  crypto_wallet_scam      5           6, 16, 34, 35, 52   6.6

  smart_contract_scam     2           10, 31              2.6

  fake_app_or_extension   0                               0.0

  exchange_scam           7           3, 15, 17, 19, 24,  9.2
                                      28, 41              

  token_launch_scam       0                               0.0

  pump_dump               0                               0.0

  rug_pull                0                               0.0

  airdrop_scam            0                               0.0

  nft_scam                0                               0.0

  sim_swap                0                               0.0

  job_scam                0                               0.0

  blackmail_extortion     3           37, 38, 39          3.9

  romance_scam            5           42, 50, 51, 53, 55  6.6
  -------------------------------------------------------------------------

Insight (Scam Subcategories):\
A single dominant subcategory exists: **exchange_scam**.\
Insights are affected by classification warnings (entry 37; entry 7 is
taxonomy-invalid and therefore not represented in locked rows).

------------------------------------------------------------------------

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  0                         0.0

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      3           69, 72, 75    3.9

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             4           1, 64, 66, 74 5.3

  poor_wallet_backup_practice    3           62, 65, 67    3.9

  tax_recordkeeping              5           2, 63, 68,    6.6
                                             71, 73        
  --------------------------------------------------------------------------

Insight (User Mistake Subcategories):\
A single dominant subcategory exists: **tax_recordkeeping**.\
Insights are not affected by classification warnings.

------------------------------------------------------------------------

**Classification Warning Summary**

- Records with classification_warning ≠ none: **4**

- Affected entry numbers: **7, 37, 49, 54**

- Warning values observed:

  - taxonomy pressure resolved (7, 37, 49)

  - insufficient technical detail provided (54)

------------------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ Dominant incident type: **scam (65.8%)**.\
2️⃣ Top three subcategories overall (ranked by count; ties
alphabetically): **investment_scam; exchange_scam;
crypto_wallet_scam**.\
3️⃣ Upper-bound prevention relevance estimate: **65.8%**.
