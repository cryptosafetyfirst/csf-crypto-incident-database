# Prevention Action Normalization Report

## Dataset Scope

Total incidents analyzed: **63**

## Input Integrity and Quality Control

### Schema Presence Check

Records with one or more missing required fields: **3**

Affected entry numbers: 60, 61, 62

### Entry Number Integrity

Entry numbers are unique integers.

### Classification Warning Audit

Records with `classification_warning` other than `none`: **34**

Affected entry numbers: 4, 5, 7, 8, 9, 11, 13, 18, 19, 20, 23, 27, 28, 29, 31, 32, 34, 35, 36, 40, 41, 44, 48, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62

Records treated as `unknown_missing_warning_field`: **3**

Affected entry numbers: 60, 61, 62

Normalization was applied conservatively to records carrying classification warnings.

### Prevention Text Coverage

Records with missing prevention text: **0**

Affected entry numbers: None

Records with vague or non-actionable prevention text: **0**

Affected entry numbers: None

Records with present but unmappable prevention text: **7**

Affected entry numbers: 17, 30, 41, 46, 52, 60, 63

## Normalized Prevention Actions

| Prevention Action | Count | Entry Numbers | % of Total |
|---|---:|---|---:|
| Verify platform legitimacy before use | 31 | 2, 4, 5, 7, 8, 9, 11, 12, 16, 18, 22, 24, 25, 26, 27, 29, 31, 32, 34, 35, 36, 38, 39, 40, 42, 43, 48, 51, 53, 55, 62 | 49.2 |
| Avoid unsolicited messages calls and DMs | 7 | 14, 21, 28, 38, 45, 54, 62 | 11.1 |
| Never share recovery phrases or private keys | 5 | 6, 47, 49, 56, 61 | 7.9 |
| Do not pay fees to unlock withdrawals | 9 | 2, 19, 20, 23, 28, 31, 40, 53, 54 | 14.3 |
| Use hardware wallets for long term storage | 0 |  | 0.0 |
| Enable strong authentication and account security | 2 | 58, 59 | 3.2 |
| Confirm network and address compatibility before transfers | 10 | 1, 3, 10, 14, 15, 33, 37, 44, 50, 57 | 15.9 |
| Test transactions with small amounts first | 9 | 1, 4, 10, 15, 19, 26, 33, 37, 50 | 14.3 |
| Limit browser extensions and keep browsers updated | 2 | 11, 13 | 3.2 |
| Revoke token approvals and review permissions regularly | 1 | 55 | 1.6 |
| Maintain complete transaction and tax records | 0 |  | 0.0 |
| Minimize public exposure of crypto holdings | 0 |  | 0.0 |

## Prevention Insights

Top three prevention actions by coverage:

1. **Verify platform legitimacy before use** — 31 incidents (49.2%).
2. **Confirm network and address compatibility before transfers** — 10 incidents (15.9%).
3. **Do not pay fees to unlock withdrawals** — 9 incidents (14.3%).

Combined coverage of the top three actions: **50 incident-action mappings**, equivalent to **79.4% of total incidents**. Because one incident may map to multiple actions, this figure is not a unique-incident coverage rate.

Coverage is affected by classification warnings in **34** records.

Coverage is affected by missing or vague prevention text in **0** records.

Coverage is affected by present but unmappable prevention text in **7** records.

No conflict with previously published guidance was identified from the provided inputs. No separate previously published guidance dataset was supplied for comparison.
