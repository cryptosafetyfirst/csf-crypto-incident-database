**Taxonomy Report --- Dataset Analytics**

**Dataset Scope**

Total incidents analyzed: 43.

**Input Integrity and Quality Checks**

Schema presence check: all 43 records contain all required fields.

Entry number integrity: all entry_number values are unique integers. No
duplicates, gaps, or non-integer values were found in the observed run
scope.

Taxonomy validity check: all incident_type values are valid. Six records
contain an invalid incident_subtype value: investment_scam. Affected
entry numbers: 7, 12, 28, 30, 31, 34. These values were not corrected
and are reported as provided.

Classification warning audit: 4 records have classification_warning
values other than none. Affected entry numbers: 3, 4, 7, 14. No records
had missing, null, or empty classification_warning values. Cross-run
taxonomy pressure cannot be determined from a single dataset, but this
run contains a within-run taxonomy pressure indicator through repeated
invalid subtype usage (investment_scam) and one explicit warning value
of taxonomy pressure resolved.

**Incident Type Distribution**

  ------------------------------------
  **Incident     **Count**   **% of
  Type**                     Total**
  -------------- ----------- ---------
  scam           32          74.4

  hack           3           7.0

  user_mistake   8           18.6
  ------------------------------------

**Hack Subcategories**

  ------------------------------------------------------------------------
  **Subcategory**              **Count**   **Entry       **% of Total
                                           Numbers**     Incidents**
  ---------------------------- ----------- ------------- -----------------
  social_engineering_hack      0                         0.0

  malware                      1           14            2.3

  trojan                       0                         0.0

  spyware                      0                         0.0

  keylogger                    1           4             2.3

  clipboard_hijacker           1           29            2.3

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

Insight (Hack Subcategories): No single dominant subcategory exists. The
top subcategories are tied: clipboard_hijacker, keylogger, malware.
Insights are affected by classification warnings.

**Scam Subcategories**

  -----------------------------------------------------------------------
  **Subcategory**         **Count**   **Entry Numbers** **% of Total
                                                        Incidents**
  ----------------------- ----------- ----------------- -----------------
  social_engineering      4           2, 3, 24, 33      9.3

  phishing                6           10, 16, 19, 21,   14.0
                                      35, 40            

  social_media_scam       1           36                2.3

  crypto_wallet_scam      1           11                2.3

  smart_contract_scam     1           22                2.3

  fake_app_or_extension   0                             0.0

  exchange_scam           4           5, 9, 18, 32      9.3

  token_launch_scam       2           1, 23             4.7

  pump_dump               0                             0.0

  rug_pull                1           6                 2.3

  airdrop_scam            2           42, 43            4.7

  nft_scam                1           13                2.3

  sim_swap                0                             0.0

  job_scam                0                             0.0

  blackmail_extortion     0                             0.0

  romance_scam            2           17, 25            4.7
  -----------------------------------------------------------------------

Insight (Scam Subcategories): A single dominant subcategory exists:
phishing. Insights are affected by classification warnings.

**User Mistake Subcategories**

  --------------------------------------------------------------------------
  **Subcategory**                **Count**   **Entry       **% of Total
                                             Numbers**     Incidents**
  ------------------------------ ----------- ------------- -----------------
  wrong_address                  0                         0.0

  wrong_network                  1           41            2.3

  seed_phrase_exposure           0                         0.0

  approval_misunderstanding      1           37            2.3

  backup_failure                 0                         0.0

  address_poisoning_copy_paste   0                         0.0

  lost_wallet_access             4           8, 15, 20, 26 9.3

  poor_wallet_backup_practice    1           38            2.3

  tax_recordkeeping              1           27            2.3
  --------------------------------------------------------------------------

Insight (User Mistake Subcategories): A single dominant subcategory
exists: lost_wallet_access. Insights are not affected by classification
warnings.

**Classification Warning Audit**

  --------------------------------------------------------------------------
  **Metric**                                                     **Value**
  -------------------------------------------------------------- -----------
  Records with classification_warning ≠ none                     4

  Affected entry numbers                                         3, 4, 7, 14

  Missing/null/empty warning fields recoded as                   0
  unknown_missing_warning_field                                  
  --------------------------------------------------------------------------

**Big-Picture Takeaways**

1.  Dominant incident type by share: scam at 74.4% of all incidents.

2.  Top three most common subcategories across all locked taxonomy
    categories: phishing (6), exchange_scam (4), lost_wallet_access (4).
    The second and third positions are tied by count and ordered
    alphabetically for determinism.

3.  Upper-bound prevention relevance estimate: 74.4%.
