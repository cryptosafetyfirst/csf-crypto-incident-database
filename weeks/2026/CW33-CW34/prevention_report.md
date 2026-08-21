**CW33 + CW34 Prevention Action Normalization Report**

**Scope:** CW33 + CW34 Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** 56

**Purpose**

Prevention action normalization measures how frequently standardized
prevention actions are explicitly supported by incident-level prevention
guidance. Guidance is derived from the incident dataset and mapped
conservatively to a fixed prevention action set without introducing
additional advice or inferred actions.

**Methodology Summary**

Prevention mappings are derived from the prevention field only. Summary
and user-mistake information may clarify intent but do not create
additional mappings. Prevention text that is missing, vague,
non-actionable, or incompatible with the available action set remains
unmapped. A single incident may map to multiple prevention actions, but
may be counted only once for each action. Classification warnings
require more conservative treatment.

**Data Integrity Notes**

A total of **56 incidents** were analyzed.

All records contained the required incident fields, and no duplicate or
non-integer entry-number issues were identified.

**27 incidents** contained a classification warning other than none: 18
were marked taxonomy pressure resolved, 8 were marked insufficient
detail to classify confidently, and 1 was marked mixed scam and
technical vectors.

There were **0 incidents with missing prevention text**. There were **18
incidents with prevention text present but unmappable to the available
prevention actions**. These incidents contained prevention guidance, but
that guidance did not correspond sufficiently to an available action to
justify a mapping.

Because present but unmappable prevention text exists, normalized
coverage represents a **lower bound** of the prevention guidance
contained in the dataset.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            21          37.5%

  Avoid unsolicited messages calls and DMs         6           10.7%

  Never share recovery phrases or private keys     4           7.1%

  Do not pay fees to unlock withdrawals            8           14.3%

  Use hardware wallets for long term storage       0           0.0%

  Enable strong authentication and account         0           0.0%
  security                                                     

  Confirm network and address compatibility before 9           16.1%
  transfers                                                    

  Test transactions with small amounts first       4           7.1%

  Limit browser extensions and keep browsers       1           1.8%
  updated                                                      

  Revoke token approvals and review permissions    0           0.0%
  regularly                                                    

  Maintain complete transaction and tax records    0           0.0%

  Minimize public exposure of crypto holdings      2           3.6%
  ----------------------------------------------------------------------

**Key Findings**

**Verify platform legitimacy before use** has the highest normalized
coverage, appearing in **21 incidents (37.5%)**.

**Confirm network and address compatibility before transfers** ranks
second with **9 incidents (16.1%)**, followed by **Do not pay fees to
unlock withdrawals** with **8 incidents (14.3%)**.

**Avoid unsolicited messages calls and DMs** appears in 6 incidents
(10.7%). **Never share recovery phrases or private keys** and **Test
transactions with small amounts first** each appear in 4 incidents
(7.1%).

Four actions have zero mapped incidents: **Use hardware wallets for long
term storage**, **Enable strong authentication and account security**,
**Revoke token approvals and review permissions regularly**, and
**Maintain complete transaction and tax records**.

**Top Prevention Actions by Coverage**

  --------------------------------------------------------------------------------------
  **Rank**       **Prevention Action**                           **Count**   **% of
                                                                             Total**
  -------------- ----------------------------------------------- ----------- -----------
  1              Verify platform legitimacy before use           21          37.5%

  2              Confirm network and address compatibility       9           16.1%
                 before transfers                                            

  3              Do not pay fees to unlock withdrawals           8           14.3%

  **Combined**                                                   **38**      **67.9%**
  --------------------------------------------------------------------------------------

**Interpretation**

Normalized prevention coverage is concentrated around platform
verification, transfer compatibility, and withdrawal-fee avoidance. The
highest-ranked action alone accounts for 37.5% of incidents, while the
three highest-ranked action counts together equal 67.9% of the dataset
size.

Coverage is affected by classification warnings in 27 incidents and by
18 incidents containing prevention guidance that could not be mapped
conservatively to the available actions. No prevention text was missing.

Zero coverage for an action means that no supplied prevention text
mapped to that action in this dataset. It does not establish the absence
or relevance of that issue beyond the normalized prevention guidance
analyzed here.

No conflicts with previously published guidance are established by the
supplied inputs.

**Role in the Weekly Series**

This report provides a standardized snapshot of prevention-action
coverage across the CW33 + CW34 incident dataset. Its fixed action
structure supports longitudinal comparison and provides consistent
prevention coverage metrics across reporting periods.

**Bottom Line**

The most prevalent normalized prevention gaps in the 56 incidents are
**platform legitimacy verification (37.5%)**, **network and address
compatibility confirmation (16.1%)**, and **avoidance of fees required
to unlock withdrawals (14.3%)**.

The distribution measures only prevention guidance that can be mapped
consistently. With 18 incidents containing present but unmappable
prevention text, the reported coverage should be interpreted as a
measurable lower bound rather than a complete representation of all
prevention guidance in the dataset.
