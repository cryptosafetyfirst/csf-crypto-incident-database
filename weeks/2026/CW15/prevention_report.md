**CW15 Prevention Action Normalization Report**

**Stage:** Prevention Action Normalization (Publication)\
**Scope:** CW15 Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** 41

**Purpose**

This report measures how often prevention guidance from real incident
records can be normalized into a fixed prevention action set. The
guidance is derived from the incident dataset itself, and all mappings
are constrained to the locked action list used for consistent
week-over-week comparison.

**Methodology Summary**

Normalization was performed from the prevention field only. The summary
and user_mistake fields were used only to clarify intent where needed,
not to invent new actions. An incident could map to more than one
prevention action, but it could be counted only once per action.
Prevention text that was missing, vague, purely narrative,
contradictory, or incompatible with the locked action set was left
unmapped. Extra caution was applied where classification warnings were
present.

**Data Integrity Notes**

Total incidents analyzed: 41.

All records contained the required fields used for normalization. All
entry_number values were unique integers, and no entry number integrity
issues were found.

Incidents with classification warnings: 2. Affected entry numbers: 14,
20.

Incidents with missing prevention text: 0.

Incidents with present but unmappable prevention text: 9. Affected entry
numbers: 4, 6, 8, 14, 17, 37, 38, 39, 40.

Incidents with vague or non-actionable prevention text: 0.

Because present but unmappable prevention text exists, the measured
coverage in this report represents a lower bound rather than complete
prevention coverage.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            10          24.4

  Avoid unsolicited messages calls and DMs         5           12.2

  Never share recovery phrases or private keys     0           0.0

  Do not pay fees to unlock withdrawals            7           17.1

  Use hardware wallets for long term storage       0           0.0

  Enable strong authentication and account         2           4.9
  security                                                     

  Confirm network and address compatibility before 2           4.9
  transfers                                                    

  Test transactions with small amounts first       1           2.4

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    2           4.9
  regularly                                                    

  Maintain complete transaction and tax records    5           12.2

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

Coverage is led by **Verify platform legitimacy before use** at 24.4% of
incidents, followed by **Do not pay fees to unlock withdrawals** at
17.1%. Two actions are tied for the next-highest coverage level: **Avoid
unsolicited messages calls and DMs** and **Maintain complete transaction
and tax records**, each at 12.2%.

Several locked actions received no explicit mappings in this dataset:
**Never share recovery phrases or private keys**, **Use hardware wallets
for long term storage**, **Limit browser extensions and keep browsers
updated**, and **Minimize public exposure of crypto holdings**.

Coverage is affected by classification warnings and by present but
unmappable prevention text. No missing prevention text was found. No
conflicts with previously published guidance are identifiable from the
provided normalization results.

**Top Prevention Actions by Coverage**

1.  **Verify platform legitimacy before use** --- 10 incidents (24.4%)

2.  **Do not pay fees to unlock withdrawals** --- 7 incidents (17.1%)

3.  **Avoid unsolicited messages calls and DMs** --- 5 incidents (12.2%)

Combined coverage of the top three actions: **53.7%** of total
incidents.

**Interpretation**

The normalized coverage is concentrated in a small number of prevention
actions rather than distributed evenly across the full action set. The
strongest concentration appears around platform verification and
withdrawal-fee refusal language, while a smaller but still visible
portion of the dataset maps to unsolicited-contact avoidance and
transaction-record maintenance.

At the same time, nine incidents contain prevention language that is
present but cannot be normalized into the locked action set without
forcing a mapping. This limits measured coverage and leaves several
prevention themes visible in the source dataset but not countable within
the standardized action table.

**Role in the Weekly Series**

This report serves as a weekly snapshot of prevention coverage across
the incident dataset. It supports longitudinal comparison by keeping the
action set, mapping discipline, and output structure stable from week to
week, allowing prevention coverage metrics to be tracked consistently
over time.

**Bottom Line**

For CW15, normalized prevention coverage is concentrated in **platform
verification**, **withdrawal-fee refusal**, and **unsolicited-contact
avoidance**. At the same time, measured coverage remains partial because
a meaningful share of incidents contains prevention text that is
explicit but not mappable to the standardized action set. This report
therefore reflects what is measurable from the dataset, not the full
universe of prevention language present in the records.
