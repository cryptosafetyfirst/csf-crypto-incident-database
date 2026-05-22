**CW21 Prevention Action Normalization Report**

**Stage: Prevention Action Normalization (Publication)**

**Scope: CW21 Crypto & Web3 Incident Dataset**

Total Incidents Analyzed: 35

**Purpose**

This report measures how frequently normalized prevention actions appear
across the weekly incident dataset. Prevention guidance is derived
directly from real incident records and normalized into a fixed
prevention action set to support consistency, comparability, and
longitudinal analysis. All mappings are constrained to the locked
prevention action set and are based solely on prevention guidance
explicitly present in the dataset.

**Methodology Summary**

Prevention actions were mapped conservatively using only the prevention
field contained in each incident record. Summary and user mistake fields
were used only to clarify intent when necessary and never to invent new
prevention actions. Multiple prevention actions could be mapped to a
single incident where explicitly supported by the prevention text.
Vague, narrative-only, contradictory, or unmappable prevention text was
not forced into a prevention category. Incidents containing
classification warnings were handled with additional caution during
normalization.

**Data Integrity Notes**

  ---------------------------------------------
  **Metric**                        **Value**
  --------------------------------- -----------
  Total incidents analyzed          35

  Incidents with classification     3
  warnings                          

  Missing prevention text           0

  Present but unmappable prevention 13
  text                              

  Entry number integrity issues     None
  ---------------------------------------------

Coverage represents a lower bound because some prevention text was
present but could not be conservatively mapped to the locked prevention
action set.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            9           25.7

  Avoid unsolicited messages calls and DMs         3           8.6

  Never share recovery phrases or private keys     1           2.9

  Do not pay fees to unlock withdrawals            3           8.6

  Use hardware wallets for long term storage       1           2.9

  Enable strong authentication and account         5           14.3
  security                                                     

  Confirm network and address compatibility before 5           14.3
  transfers                                                    

  Test transactions with small amounts first       1           2.9

  Limit browser extensions and keep browsers       1           2.9
  updated                                                      

  Revoke token approvals and review permissions    1           2.9
  regularly                                                    

  Maintain complete transaction and tax records    1           2.9

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

  ---------------------------------------------------------------------------------
  **Rank**   **Prevention Action**                            **Count**   **% of
                                                                          Total**
  ---------- ------------------------------------------------ ----------- ---------
  1          Verify platform legitimacy before use            9           25.7

  2          Confirm network and address compatibility before 5           14.3
             transfers                                                    

  3          Enable strong authentication and account         5           14.3
             security                                                     
  ---------------------------------------------------------------------------------

The dataset shows the highest concentration of prevention coverage
around platform verification practices. Address and network verification
actions and account security actions appeared at equal frequency.
Several prevention actions appeared only once, while one prevention
action category received no coverage in the analyzed dataset.

**Top Prevention Actions by Coverage**

  ---------------------------------------------------------------------------------
  **Rank**   **Prevention Action**                            **Count**   **% of
                                                                          Total**
  ---------- ------------------------------------------------ ----------- ---------
  1          Verify platform legitimacy before use            9           25.7

  2          Confirm network and address compatibility before 5           14.3
             transfers                                                    

  3          Enable strong authentication and account         5           14.3
             security                                                     
  ---------------------------------------------------------------------------------

Combined percentage of total incidents covered by the top three
prevention actions: 54.3%

**Interpretation**

The distribution shows that prevention language in the dataset
concentrated primarily around legitimacy verification, transfer
validation, and account security practices. Coverage across the
remaining prevention actions was comparatively sparse, with several
actions appearing only once or not at all. The dataset also contains
prevention text that could not be conservatively normalized into the
locked prevention action set, limiting total measurable coverage.

**Role in the Weekly Series**

This report serves as a weekly snapshot of normalized prevention
coverage across the incident dataset. By maintaining a fixed prevention
action structure and stable reporting format, it supports longitudinal
comparison of prevention patterns and measurable prevention coverage
across weekly reporting cycles.

**Bottom Line**

The dataset's measurable prevention coverage was concentrated in a
relatively small number of prevention actions, particularly platform
legitimacy verification and transaction validation practices. A
meaningful portion of prevention text remained unmappable under
conservative normalization rules, reinforcing that reported coverage
represents measurable normalized guidance rather than complete
prevention representation.
