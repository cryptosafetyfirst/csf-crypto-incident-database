**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

**Total incidents analyzed:** 73

**Input Integrity & Quality Control**

**Schema Presence**

All 73 records contain the required fields: entry_number, incident_type,
incident_subtype, and classification_warning.

**Entry Number Integrity**

All entry_number values are unique integers. No duplicates or gaps are
present.

**Taxonomy Validity**

All incident_type values are valid.

Eight records contain incident_subtype values outside the locked
taxonomy. No values have been corrected or reclassified.

  ---------------------------------------------------
  **Entry      **Incident     **Invalid Incident
  Number**     Type**         Subtype**
  ------------ -------------- -----------------------
  12           scam           investment_scam

  15           scam           address_poisoning

  17           scam           fake_app_extension

  18           user_mistake   wrong_asset

  19           scam           investment_scam

  22           user_mistake   transaction_confusion

  25           scam           investment_scam

  31           scam           investment_scam
  ---------------------------------------------------

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           57          78.1

  hack           8           11.0

  user_mistake   8           11.0
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      1           42            1.4

  malware                      4           43, 53, 59,   5.5
                                           63            

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    0                         0.0

  clipboard_hijacker           0                         0.0

  ransomware                   0                         0.0

  cryptojacking                0                         0.0

  network_mitm                 0                         0.0

  wifi_sniffing                0                         0.0

  dns_spoofing                 0                         0.0

  session_hijacking            1           56            1.4

  ssl_stripping                0                         0.0

  fake_app_or_extension_hack   0                         0.0

  exchange_vulnerability       0                         0.0

  insider_attack               0                         0.0

  wallet_software_exploit      2           3, 8          2.7
  ------------------------------------------------------------------------

**Insight (Hack Subcategories):**

A single dominant subcategory exists: **malware**, with 4 incidents
representing **5.5%** of total incidents.

Insights are affected by classification warnings. Hack records 3, 8, and
42 contain classification warnings.

**Scam Subcategories**

  ----------------------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers**                **% of Total
                                                                       Incidents**
  ----------------------- ----------- -------------------------------- -------------
  social_engineering      11          28, 32, 36, 40, 55, 57, 58, 61,  15.1
                                      62, 67, 70                       

  phishing                17          2, 5, 13, 14, 16, 26, 33, 35,    23.3
                                      41, 47, 48, 64, 65, 66, 71, 72,  
                                      73                               

  social_media_scam       0                                            0.0

  crypto_wallet_scam      1           50                               1.4

  smart_contract_scam     0                                            0.0

  fake_app_or_extension   1           52                               1.4

  exchange_scam           10          1, 7, 24, 37, 38, 39, 44, 46,    13.7
                                      49, 60                           

  token_launch_scam       2           54, 68                           2.7

  pump_dump               0                                            0.0

  rug_pull                2           9, 30                            2.7

  airdrop_scam            2           21, 29                           2.7

  nft_scam                0                                            0.0

  sim_swap                0                                            0.0

  job_scam                2           6, 20                            2.7

  blackmail_extortion     0                                            0.0

  romance_scam            3           10, 34, 69                       4.1
  ----------------------------------------------------------------------------------

**Insight (Scam Subcategories):**

A single dominant subcategory exists: **phishing**, with 17 incidents
representing **23.3%** of total incidents.

Insights are affected by classification warnings.

Six scam records have subtype values outside the locked taxonomy and
therefore are not represented in the subcategory table: entries **12,
15, 17, 19, 25, and 31**.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  1           23            1.4

  wrong_network                  2           27, 51        2.7

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      0                         0.0

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             3           4, 11, 45     4.1

  poor_wallet_backup_practice    0                         0.0

  tax_recordkeeping              0                         0.0
  --------------------------------------------------------------------------

**Insight (User Mistake Subcategories):**

A single dominant subcategory exists: **lost_wallet_access**, with 3
incidents representing **4.1%** of total incidents.

Insights are affected by classification warnings.

Two user-mistake records have subtype values outside the locked taxonomy
and therefore are not represented in the subcategory table: entries **18
and 22**.

**Classification Warning Audit**

**Records with classification_warning ≠ none:** 30

**Affected entry numbers:** 3, 8, 10, 12, 13, 14, 17, 20, 21, 22, 23,
24, 26, 27, 28, 29, 31, 32, 33, 36, 42, 49, 50, 58, 60, 61, 67, 70, 71,
72

  ------------------------------------------------------------------------------
  **Classification Warning**                            **Count**   **Entry
                                                                    Numbers**
  ----------------------------------------------------- ----------- ------------
  insufficient detail to classify confidently           3           3, 28, 32

  insufficient detail to confirm intentional scam       3           24, 49, 50

  insufficient detail to identify compromise vector     2           42, 67

  insufficient detail to identify exact compromise      2           71, 72
  mechanism                                                         

  physical mail QR code phishing campaign               1           14

  likely pig-butchering investment scam                 1           10

  physical courier variant of pig-butchering investment 1           12
  scam                                                              

  expired-domain phishing attack                        1           13

  includes secondary recovery scam after initial        1           21
  airdrop scam                                                      

  suspected job scam with no confirmed loss or          1           20
  subsequent payment demand                                         

  insufficient detail to confirm how the fake token     1           17
  substitution occurred                                             

  no confirmed loss or completed user error reported    1           22

  funds reportedly remain on-chain at an address        1           27
  controlled by Coinbase                                            

  possible address poisoning but insufficient evidence  1           23
  to confirm attacker involvement                                   

  reported fake merchant with additional payment demand 1           26

  multi-channel phishing using phone impersonation and  1           33
  fake email                                                        

  advance-fee scam pattern with no confirmed individual 1           31
  loss stated                                                       

  suspected malicious token distribution with no        1           29
  confirmed loss or harmful interaction                             

  attempted social engineering with no confirmed        1           28
  financial loss                                                    

  insufficient detail to determine exact scam mechanism 1           36

  taxonomy pressure resolved                            1           40

  attempted phishing with no confirmed interaction or   1           41
  financial loss                                                    

  insufficient detail to confirm user loss              1           58

  mixed scam patterns with separate rug pull losses     1           70
  ------------------------------------------------------------------------------

Repeated warning patterns are present in the dataset.

**Big-Picture Takeaways**

1️⃣ **Dominant incident type:** **scam**, with 57 of 73 incidents
(**78.1%**).

2️⃣ **Top three valid subcategories overall:** **phishing** (17),
**social_engineering** (11), and **exchange_scam** (10).

3️⃣ **Upper-bound prevention relevance estimate:** **78.1%**.
