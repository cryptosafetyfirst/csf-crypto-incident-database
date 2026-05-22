**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 35

**Schema Presence Check**

  ---------------------------------------
  **Check**                  **Result**
  -------------------------- ------------
  Required fields present    Yes

  Records missing required   0
  fields                     
  ---------------------------------------

**Entry Number Integrity**

  ---------------------------------
  **Check**            **Result**
  -------------------- ------------
  Unique integers      Yes

  Duplicate entry      None
  numbers              

  Gaps detected        None

  Non-integer values   None
  ---------------------------------

**Taxonomy Validity Check**

  ----------------------------------------
  **Entry      **Invalid Value**
  Number**     
  ------------ ---------------------------
  20           wrong_recipient_transfer

  21           wrong_recipient_transfer

  22           fake_exchange_or_platform

  23           fake_exchange_or_platform

  24           advance_fee_scam

  25           ponzi_scheme

  27           lost_access_credentials

  28           pig_butchering

  31           fake_investment_platform

  32           investment_scam

  33           lost_seed_phrase

  34           recovery_scam

  35           impersonation_scam
  ----------------------------------------

**Classification Warning Audit**

  -----------------------------------------------
  **Metric**                          **Value**
  ----------------------------------- -----------
  Records with classification_warning 3
  ≠ none                              

  Affected entry numbers              6, 10, 23
  -----------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           25          71.4

  user_mistake   8           22.9

  hack           2           5.7
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      2           9, 26         5.7

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

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      0                         0.0
  ------------------------------------------------------------------------

Insight (Hack Subcategories):

A single dominant subcategory exists: social_engineering_hack.

Insights are not materially affected by classification warnings.

**Scam Subcategories**

  ---------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry         **% of Total
                                      Numbers**       Incidents**
  ----------------------- ----------- --------------- -----------------
  social_engineering      1           7               2.9

  phishing                6           5, 8, 10, 17,   17.1
                                      29, 30          

  social_media_scam       3           12, 14, 15      8.6

  crypto_wallet_scam      0                           0.0

  smart_contract_scam     0                           0.0

  fake_app_or_extension   0                           0.0

  exchange_scam           4           1, 3, 18, 19    11.4

  token_launch_scam       0                           0.0

  pump_dump               1           4               2.9

  rug_pull                0                           0.0

  airdrop_scam            0                           0.0

  nft_scam                0                           0.0

  sim_swap                0                           0.0

  job_scam                1           13              2.9

  blackmail_extortion     0                           0.0

  romance_scam            0                           0.0
  ---------------------------------------------------------------------

Insight (Scam Subcategories):

A single dominant subcategory exists: phishing.

Insights are partially affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  1           16            2.9

  wrong_network                  2           2, 6          5.7

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      0                         0.0

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             1           11            2.9

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

Insight (User Mistake Subcategories):

A single dominant subcategory exists: wrong_network.

Insights are partially affected by classification warnings.

**Big-Picture Takeaways**

1️⃣ Dominant incident type: scam (71.4% of incidents).

2️⃣ Top three subcategories overall: phishing; exchange_scam;
social_media_scam.

3️⃣ Upper-bound prevention relevance estimate: 71.4%.
