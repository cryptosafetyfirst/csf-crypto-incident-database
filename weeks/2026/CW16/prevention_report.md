**CW16 Prevention Action Normalization Report**

Stage: Prevention Action Normalization (Publication)

Scope: CW16 Crypto & Web3 Incident Dataset

Total Incidents Analyzed: 55

**Purpose**

This report measures how often explicit prevention guidance appears
across the incident dataset after normalizing free-text prevention
language into a fixed prevention action set. The guidance reflected here
is derived from recorded incident-level prevention text and is
constrained to a locked action set for consistency and comparability.

**Methodology Summary**

Prevention guidance was mapped from the prevention field only. Summary
and user mistake fields were used only to clarify intent where needed
and were not used to invent actions. Multiple actions were allowed for a
single incident when the prevention text explicitly supported them.
Present but vague, narrative, or incompatible prevention text was left
unmapped. Records carrying classification warnings were handled more
conservatively.

**Data Integrity Notes**

A total of 55 incidents were analyzed.

All required fields were present across all records. No schema-presence
failures were identified.

Entry numbers were unique integers throughout the dataset. No entry
number integrity issues were identified.

Classification warnings were present in 4 incidents: 4, 17, 37, and 41.

Missing prevention text was identified in 0 incidents.

Present but unmappable prevention text was identified in 9 incidents.

Because present but unmappable prevention text exists, the coverage
figures in this report represent a lower bound.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            28          50.9

  Avoid unsolicited messages calls and DMs         16          29.1

  Never share recovery phrases or private keys     4           7.3

  Do not pay fees to unlock withdrawals            4           7.3

  Use hardware wallets for long term storage       1           1.8

  Enable strong authentication and account         1           1.8
  security                                                     

  Confirm network and address compatibility before 4           7.3
  transfers                                                    

  Test transactions with small amounts first       2           3.6

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    1           1.8
  regularly                                                    

  Maintain complete transaction and tax records    5           9.1

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

The most frequently normalized prevention action was Verify platform
legitimacy before use, appearing in 28 incidents. Avoid unsolicited
messages calls and DMs ranked second with 16 incidents. Maintain
complete transaction and tax records ranked third with 5 incidents.

A secondary cluster of actions appeared at lower but consistent levels:
Never share recovery phrases or private keys, Do not pay fees to unlock
withdrawals, and Confirm network and address compatibility before
transfers each appeared in 4 incidents.

Several locked actions had little or no explicit coverage in the
recorded prevention text. Limit browser extensions and keep browsers
updated and Minimize public exposure of crypto holdings did not appear
in any incident mappings.

**Top Prevention Actions by Coverage**

  -----------------------------------------------------------------------
  **Rank**   **Prevention Action**                  **Count**   **% of
                                                                Total**
  ---------- -------------------------------------- ----------- ---------
  1          Verify platform legitimacy before use  28          50.9

  2          Avoid unsolicited messages calls and   16          29.1
             DMs                                                

  3          Maintain complete transaction and tax  5           9.1
             records                                            
  -----------------------------------------------------------------------

Combined percentage of total incidents: 89.1

**Interpretation**

The distribution shows a strong concentration in explicit
platform-verification guidance, followed by avoidance of unsolicited
contact paths. After those two actions, coverage declines sharply across
the remainder of the locked action set.

The dataset also contains a measurable amount of present but unmappable
prevention language. This limits total normalized coverage and indicates
that some recorded prevention guidance is more specific, operational, or
category-bound than the locked action set can represent.

Coverage is affected by classification warnings and by present but
unmappable prevention text. Missing prevention text did not affect
coverage in this dataset.

No conflicts were identified between the mapped actions and the
previously published safety guidance included in the attached materials,
which consistently reinforce themes such as platform verification, seed
phrase protection, approval review, transaction checking, recordkeeping,
and hardware-wallet use.

**Role in the Weekly Series**

This report serves as a weekly snapshot of normalized prevention
coverage across the incident dataset. It supports longitudinal
comparison and anchors prevention coverage metrics across weeks.

**Bottom Line**

The dataset is dominated by prevention language tied to platform
legitimacy checks and avoidance of unsolicited contact. Explicit tax
recordkeeping guidance appears meaningfully but at much lower frequency,
while several locked actions show minimal or zero direct coverage. The
result is measurable and comparable, but not complete, because some
incident prevention text is present yet cannot be mapped conservatively
into the locked action set.
