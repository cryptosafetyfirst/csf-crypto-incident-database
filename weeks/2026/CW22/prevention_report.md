**CW22 2026 Prevention Action Normalization Report**

Stage: Prevention Action Normalization (Publication)

Scope: CW22 2026 Crypto & Web3 Incident Dataset

Total Incidents Analyzed: 40

**Purpose**

This report summarizes prevention coverage observed across the CW22 2026
incident dataset. Prevention guidance is normalized into a fixed
prevention action set to support consistent measurement, comparison, and
longitudinal tracking. All mappings are constrained to the locked
prevention action set and are derived only from prevention language
contained within incident records.

**Methodology Summary**

Prevention actions were mapped exclusively from the prevention field
contained in each incident record. Multiple prevention actions were
permitted when explicitly supported by the prevention text. Vague,
missing, narrative-only, or otherwise unmappable prevention text was not
forced into a prevention category. Classification warnings were handled
conservatively and reduce confidence in affected mappings.

**Data Integrity Notes**

- Total incidents analyzed: 40

- Records with classification warnings: 5

- Classification warning entry numbers: 2, 5, 10, 11, 15

- Records with missing prevention text: 0

- Records with present but unmappable prevention text: 20

- Entry number integrity issues detected: none

Because unmappable prevention text exists, prevention coverage should be
interpreted as a lower bound of explicitly stated prevention guidance
present within the dataset.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            2           5.0

  Avoid unsolicited messages calls and DMs         5           12.5

  Never share recovery phrases or private keys     2           5.0

  Do not pay fees to unlock withdrawals            1           2.5

  Use hardware wallets for long term storage       1           2.5

  Enable strong authentication and account         0           0.0
  security                                                     

  Confirm network and address compatibility before 9           22.5
  transfers                                                    

  Test transactions with small amounts first       6           15.0

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    2           5.0
  regularly                                                    

  Maintain complete transaction and tax records    0           0.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

- Confirm network and address compatibility before transfers was the
  most frequently observed prevention action.

- Test transactions with small amounts first was the second most
  frequently observed prevention action.

- Avoid unsolicited messages calls and DMs was the third most frequently
  observed prevention action.

- Four prevention actions recorded no coverage within the normalized
  dataset.

- Coverage distribution was concentrated within a small subset of the
  available prevention action set.

**Top Prevention Actions by Coverage**

  ---------------------------------------------------------------------------------
  **Rank**   **Prevention Action**                            **Count**   **% of
                                                                          Total**
  ---------- ------------------------------------------------ ----------- ---------
  1          Confirm network and address compatibility before 9           22.5
             transfers                                                    

  2          Test transactions with small amounts first       6           15.0

  3          Avoid unsolicited messages calls and DMs         5           12.5
  ---------------------------------------------------------------------------------

Combined percentage of total incidents: 50.0%

**Interpretation (Non-Speculative)**

The normalized coverage distribution is concentrated around transfer
validation, test transactions, and avoidance of unsolicited
communications. Several prevention actions recorded no explicit coverage
because no corresponding prevention language was present in the mapped
incident records. Classification warnings and unmappable prevention text
limit the completeness of measurable coverage.

**Role in the Weekly Series**

This report provides a weekly snapshot of prevention coverage observed
within the incident dataset. By applying a consistent normalization
process across weeks, it supports longitudinal comparison and
establishes stable prevention coverage metrics over time.

**Bottom Line**

CW22 2026 prevention coverage was concentrated in a small number of
explicitly stated prevention actions, led by transfer verification, test
transactions, and avoidance of unsolicited communications. Half of all
incidents mapped to one of these three actions. Coverage metrics reflect
only prevention language that could be normalized mechanically and
should be interpreted as measurable coverage rather than complete
prevention representation.
