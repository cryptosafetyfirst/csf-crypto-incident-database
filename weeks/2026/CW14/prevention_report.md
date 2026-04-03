**CW14 Prevention Action Normalization Report**

**Stage:** Prevention Action Normalization (Publication)\
**Scope:** CW14 Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** 37

**Purpose**

This report measures how often explicit prevention guidance in the
weekly incident dataset can be normalized into a fixed prevention action
set. The guidance is derived from real incidents, and all mappings are
constrained to a locked action list to preserve comparability across
weeks.

**Methodology Summary**

Normalization was performed from the prevention field only. Mapping was
conservative, multiple actions were allowed for a single incident when
explicitly supported by the prevention text, and vague or unmappable
language was left unmapped rather than forced into a category. Records
with classification warnings were handled with reduced confidence.

**Data Integrity Notes**

All 37 records were analyzed. No required-field gaps were detected in
the provided dataset, and no entry number integrity issues were
identified.\
Classification warnings were present in 7 records: 6, 10, 20, 21, 23,
34, 37.\
Missing prevention text was present in 0 records.\
Present but unmappable prevention text was present in 11 records: 3, 4,
6, 8, 11, 12, 13, 18, 20, 30, 32.\
Because unmappable prevention text exists, the coverage figures below
represent a lower bound.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            14          37.8

  Avoid unsolicited messages calls and DMs         8           21.6

  Never share recovery phrases or private keys     0           0.0

  Do not pay fees to unlock withdrawals            5           13.5

  Use hardware wallets for long term storage       0           0.0

  Enable strong authentication and account         1           2.7
  security                                                     

  Confirm network and address compatibility before 4           10.8
  transfers                                                    

  Test transactions with small amounts first       1           2.7

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    0           0.0
  regularly                                                    

  Maintain complete transaction and tax records    0           0.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

Coverage is concentrated in a small number of actions. The most frequent
normalized action is **Verify platform legitimacy before use**, followed
by **Avoid unsolicited messages calls and DMs**, then **Do not pay fees
to unlock withdrawals**. **Confirm network and address compatibility
before transfers** appears at a lower level, while the remaining mapped
actions occur rarely or not at all. No conflicts with previously
published guidance are observable from the provided inputs.

**Top Prevention Actions by Coverage**

1.  Verify platform legitimacy before use --- 14 incidents --- 37.8%

2.  Avoid unsolicited messages calls and DMs --- 8 incidents --- 21.6%

3.  Do not pay fees to unlock withdrawals --- 5 incidents --- 13.5%

Combined coverage of the top three prevention actions: **73.0% of total
incidents**.

**Interpretation**

The normalized distribution is concentrated around platform vetting,
unsolicited-contact avoidance, and withdrawal-unlock payment resistance.
Several action categories remain unused in this week's dataset, and
measured coverage is constrained by both classification warnings and
prevention text that was present but could not be mapped conservatively.

**Role in the Weekly Series**

This report serves as a weekly snapshot of explicit prevention coverage
in the incident dataset. It supports longitudinal comparison by keeping
the action set fixed and the normalization rules stable across weeks.

**Bottom Line**

This week's measurable prevention coverage is concentrated in a narrow
subset of the action set, especially platform verification and
unsolicited-contact avoidance. The results reflect only prevention
language that could be normalized directly from the dataset, so they
measure explicit coverage rather than complete preventive potential.
