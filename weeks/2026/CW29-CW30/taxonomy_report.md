# Taxonomy Report — Dataset Analytics

## Dataset Scope

Total incidents analyzed: **63**

## Input Integrity and Quality Control

### Schema Presence Check

Records with one or more missing required fields: **3**

Affected entry numbers: 60, 61, 62

### Entry Number Integrity

Entry numbers are unique integers with no gaps in the observed range.

### Taxonomy Validity Check

No invalid incident-type values detected.

| Entry Number | Invalid Incident Subtype |
|---:|---|
| 46 | exchange_transfer_issue |
| 52 | wallet_compromise |
| 56 | wallet_compromise |
| 58 | wallet_compromise |

## Incident Type Distribution

| Incident Type | Count | % of Total |
|---|---:|---:|
| scam | 44 | 69.8 |
| hack | 9 | 14.3 |
| user_mistake | 10 | 15.9 |

## Hack Subcategories

| Subcategory | Count | Entry Numbers | % of Total Incidents |
|---|---:|---|---:|
| social_engineering_hack | 0 |  | 0.0 |
| malware | 2 | 17, 61 | 3.2 |
| trojan | 0 |  | 0.0 |
| spyware | 1 | 13 | 1.6 |
| keylogger | 0 |  | 0.0 |
| clipboard_hijacker | 0 |  | 0.0 |
| ransomware | 0 |  | 0.0 |
| cryptojacking | 0 |  | 0.0 |
| network_mitm | 0 |  | 0.0 |
| wifi_sniffing | 0 |  | 0.0 |
| dns_spoofing | 0 |  | 0.0 |
| session_hijacking | 1 | 59 | 1.6 |
| ssl_stripping | 0 |  | 0.0 |
| fake_app_or_extension_hack | 2 | 11, 21 | 3.2 |
| exchange_vulnerability | 0 |  | 0.0 |
| insider_attack | 0 |  | 0.0 |
| wallet_software_exploit | 0 |  | 0.0 |

**Insight:** No single dominant subcategory exists. Tied top subcategories: fake_app_or_extension_hack, malware (2 incidents each; 3.2% of total incidents each).

Insights are affected by classification warnings: 7 hack records carry a warning.

## Scam Subcategories

| Subcategory | Count | Entry Numbers | % of Total Incidents |
|---|---:|---|---:|
| social_engineering | 12 | 7, 14, 20, 23, 27, 28, 31, 35, 38, 41, 54, 63 | 19.0 |
| phishing | 5 | 5, 6, 39, 45, 62 | 7.9 |
| social_media_scam | 2 | 2, 34 | 3.2 |
| crypto_wallet_scam | 3 | 1, 3, 44 | 4.8 |
| smart_contract_scam | 1 | 55 | 1.6 |
| fake_app_or_extension | 1 | 22 | 1.6 |
| exchange_scam | 12 | 4, 8, 9, 18, 19, 26, 29, 32, 36, 40, 48, 53 | 19.0 |
| token_launch_scam | 0 |  | 0.0 |
| pump_dump | 0 |  | 0.0 |
| rug_pull | 0 |  | 0.0 |
| airdrop_scam | 1 | 51 | 1.6 |
| nft_scam | 0 |  | 0.0 |
| sim_swap | 0 |  | 0.0 |
| job_scam | 4 | 24, 42, 43, 60 | 6.3 |
| blackmail_extortion | 0 |  | 0.0 |
| romance_scam | 3 | 12, 16, 25 | 4.8 |

**Insight:** No single dominant subcategory exists. Tied top subcategories: exchange_scam, social_engineering (12 incidents each; 19.0% of total incidents each).

Insights are affected by classification warnings: 26 scam records carry a warning.

## User Mistake Subcategories

| Subcategory | Count | Entry Numbers | % of Total Incidents |
|---|---:|---|---:|
| wrong_address | 2 | 33, 57 | 3.2 |
| wrong_network | 4 | 10, 15, 37, 50 | 6.3 |
| seed_phrase_exposure | 0 |  | 0.0 |
| approval_misunderstanding | 0 |  | 0.0 |
| backup_failure | 0 |  | 0.0 |
| address_poisoning_copy_paste | 0 |  | 0.0 |
| lost_wallet_access | 3 | 30, 47, 49 | 4.8 |
| poor_wallet_backup_practice | 0 |  | 0.0 |
| tax_recordkeeping | 0 |  | 0.0 |

**Insight:** A single dominant subcategory exists: wrong_network (4 incidents; 6.3% of total incidents).

Insights are affected by classification warnings: 1 user_mistake records carry a warning.

## Classification Warning Audit

Records with `classification_warning` other than `none`: **34**

Affected entry numbers: 4, 5, 7, 8, 9, 11, 13, 18, 19, 20, 23, 27, 28, 29, 31, 32, 34, 35, 36, 40, 41, 44, 48, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62

Records treated as `unknown_missing_warning_field`: **3**

Affected entry numbers: 60, 61, 62

## Big-Picture Takeaways

1️⃣ Dominant incident type: **scam** (44 incidents; 69.8% of incidents).

2️⃣ Top three subcategories overall: **exchange_scam** (12); **social_engineering** (12); **phishing** (5).

3️⃣ Upper-bound prevention relevance estimate: **69.8%**.
