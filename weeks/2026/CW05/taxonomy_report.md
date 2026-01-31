**Taxonomy Report --- Dataset Analytics**

------------------------------------------------------------------------

**Dataset Scope**

**Total incidents analyzed:** **80**

------------------------------------------------------------------------

**Input Integrity & QC Checks**

**Schema Presence Check**

All 80 records contain the required fields:

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

⚠️ **Gaps exist** (expected and allowed).\
Entry numbers are run-scoped and not required to be contiguous.

------------------------------------------------------------------------

**Taxonomy Validity Check**

**Invalid incident_type values detected (outside locked taxonomy):**

  -------------------------------------
  **entry_number**   **invalid
                     incident_type**
  ------------------ ------------------
  58                 data_breach

  59                 defi_exploit

  60                 defi_exploit

  61                 defi_exploit

  62                 crypto_scam
  -------------------------------------

These records are **reported but not corrected** and remain included in
totals.

------------------------------------------------------------------------

**Classification Warning Audit**

- **Records with classification_warning ≠ none:** **11**

- **Affected entry numbers:**\
  18, 19, 32, 34, 41, 58, 59, 60, 61, 62, 75

⚠️ Recurrent patterns observed:

- *taxonomy pressure resolved*

- *insufficient detail to classify confidently*

These constitute an **early taxonomy pressure signal**.

------------------------------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           61          76.3

  user_mistake   8           10.0

  hack           6           7.5
  ------------------------------------

Percentages are based on total incidents (80).\
Invalid incident types are excluded from this table but disclosed above.

------------------------------------------------------------------------

**Hack Subcategories**

  ----------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of
                                           Numbers**     Total**
  ---------------------------- ----------- ------------- ---------
  social_engineering_hack      0                         0.0

  malware                      4           5, 15, 32, 75 5.0

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

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      2           13, 34        2.5
  ----------------------------------------------------------------

**Insight (Hack Subcategories):**\
A single dominant subcategory exists: **malware**.\
Insights are **partially affected** by classification warnings.

------------------------------------------------------------------------

**Scam Subcategories**

  ------------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**                      **% of
                                                                             Total**
  ----------------------- ----------- -------------------------------------- ---------
  social_engineering      12          2, 12, 20, 23, 33, 37, 38, 42, 46, 52, 15.0
                                      70, 79                                 

  phishing                7           30, 31, 39, 53, 68, 69, 78             8.8

  social_media_scam       7           3, 7, 11, 24, 26, 27, 63               8.8

  crypto_wallet_scam      2           65, 67                                 2.5

  smart_contract_scam     1           35                                     1.2

  fake_app_or_extension   0                                                  0.0

  exchange_scam           17          4, 9, 16, 17, 21, 25, 29, 40, 43, 44,  21.3
                                      50, 55, 71, 72, 76, 77, 80             

  token_launch_scam       1           66                                     1.2

  pump_dump               0                                                  0.0

  rug_pull                1           64                                     1.2

  airdrop_scam            4           8, 10, 28, 36                          5.0

  nft_scam                0                                                  0.0

  sim_swap                0                                                  0.0

  job_scam                1           6                                      1.2

  blackmail_extortion     0                                                  0.0

  romance_scam            4           14, 22, 45, 73                         5.0
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

  wrong_network                  2           1, 54         2.5

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      1           19            1.2

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             1           74            1.2

  poor_wallet_backup_practice    1           18            1.2

  tax_recordkeeping              3           48, 49, 51    3.8
  ------------------------------------------------------------------

**Insight (User Mistake Subcategories):**\
A single dominant subcategory exists: **tax_recordkeeping**.\
Insights are **affected by classification warnings**.

------------------------------------------------------------------------

**Big-Picture Takeaways**

1️⃣ **Dominant incident type:** **scam** (76.3% of incidents).

2️⃣ **Top three subcategories overall:**

- exchange_scam

- social_engineering

- phishing

3️⃣ **Upper-bound prevention relevance estimate:** **76.3%**.
