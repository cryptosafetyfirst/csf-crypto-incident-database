**CW23 + CW24 2026 Prevention Action Normalization Report**

**Stage:** Prevention Action Normalization (Publication)\
**Scope:** CW23 + CW24 2026 Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** 86

**Purpose**

This report summarizes prevention guidance observed across the incident
dataset and normalizes that guidance into a fixed prevention action set.
The objective is to provide a consistent view of prevention coverage
across incidents while preserving comparability and avoiding
reinterpretation of the original prevention guidance.

**Methodology Summary**

- Prevention mappings were derived from the prevention field.

- Multiple prevention actions may be mapped to a single incident when
  explicitly supported.

- Vague, missing, narrative-only, or unmappable prevention text was not
  force-mapped.

- Classification warnings were treated conservatively during
  normalization.

- Coverage reflects only prevention actions present within the locked
  prevention action set.

**Data Integrity Notes**

  -----------------------------------------------
  **Metric**                        **Value**
  --------------------------------- -------------
  Total Incidents Analyzed          86

  Incidents with Classification     14
  Warnings                          

  Missing Prevention Text           0

  Present but Unmappable Prevention 25
  Text                              

  Entry Number Integrity Issues     None Observed
  -----------------------------------------------

Coverage should be interpreted as a lower bound because some prevention
text was present but could not be conservatively mapped to the locked
prevention action set.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            46          53.5

  Avoid unsolicited messages calls and DMs         18          20.9

  Never share recovery phrases or private keys     8           9.3

  Do not pay fees to unlock withdrawals            5           5.8

  Use hardware wallets for long term storage       1           1.2

  Enable strong authentication and account         7           8.1
  security                                                     

  Confirm network and address compatibility before 0           0.0
  transfers                                                    

  Test transactions with small amounts first       1           1.2

  Limit browser extensions and keep browsers       1           1.2
  updated                                                      

  Revoke token approvals and review permissions    0           0.0
  regularly                                                    

  Maintain complete transaction and tax records    1           1.2

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

- Platform legitimacy verification was the most frequently observed
  prevention action.

- Avoiding unsolicited messages, calls, and direct messages ranked
  second.

- Protection of recovery phrases and private keys ranked third.

- Several prevention actions appeared only once or were not explicitly
  represented in the dataset.

- Twenty-five incidents contained prevention text that could not be
  conservatively normalized into the locked action set.

**Top Prevention Actions by Coverage**

  ---------------------------------------------------------------------
  **Rank**   **Prevention Action**                **Count**   **% of
                                                              Total**
  ---------- ------------------------------------ ----------- ---------
  1          Verify platform legitimacy before    46          53.5
             use                                              

  2          Avoid unsolicited messages calls and 18          20.9
             DMs                                              

  3          Never share recovery phrases or      8           9.3
             private keys                                     
  ---------------------------------------------------------------------

**Combined Coverage of Top Three Actions:** 83.7%

**Interpretation**

The normalized distribution is concentrated in a small number of
prevention actions, particularly legitimacy verification and avoidance
of unsolicited contact. Several actions in the locked action set showed
minimal or no explicit coverage. Coverage is affected by the presence of
classification warnings and by prevention text that could not be mapped
conservatively into the predefined action set.

**Role in the Weekly Series**

This report provides a standardized weekly snapshot of prevention
coverage across observed incidents. By using a fixed prevention action
set and consistent normalization rules, it supports longitudinal
comparison of prevention patterns over time.

**Bottom Line**

The dataset\'s prevention coverage was dominated by platform legitimacy
verification, avoidance of unsolicited contact, and protection of
recovery phrases or private keys. A meaningful portion of incidents
contained prevention language that could not be normalized into the
locked action set, making the reported coverage measurable but not
exhaustive.
