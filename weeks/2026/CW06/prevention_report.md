**CW06 Prevention Action Normalization Report**

**Stage:** Prevention Action Normalization (Publication)\
**Scope:** CWXX Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** **56**

**Purpose**

This report summarizes normalized prevention coverage across the weekly
incident dataset. Prevention guidance is derived only from the
prevention text recorded in incident records and mapped conservatively
into a locked prevention action set to support week-over-week
comparability.

**Methodology Summary**

Prevention actions are mapped only from the prevention field. Mapping is
conservative: incidents are mapped only when the prevention text
explicitly matches an allowed action. Multiple actions may be mapped per
incident. When classification warnings are present, mappings are handled
with additional caution. Vague, missing, or unmappable prevention text
is disclosed rather than forced into categories.

**Data Integrity Notes**

- Total incidents analyzed: **56**

- Incidents with classification warnings (including missing warning
  field treated as unknown): **3**

- Incidents with missing prevention text: **0**

- Incidents with present but unmappable prevention text: **25**

- Entry number integrity issues: **none detected**

Because unmappable prevention text exists, coverage should be
interpreted as a **lower bound** on prevention visibility in the
dataset.

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            15          26.8

  Avoid unsolicited messages calls and DMs         9           16.1

  Never share recovery phrases or private keys     2           3.6

  Do not pay fees to unlock withdrawals            4           7.1

  Use hardware wallets for long term storage       2           3.6

  Enable strong authentication and account         2           3.6
  security                                                     

  Confirm network and address compatibility before 3           5.4
  transfers                                                    

  Test transactions with small amounts first       0           0.0

  Limit browser extensions and keep browsers       1           1.8
  updated                                                      

  Revoke token approvals and review permissions    1           1.8
  regularly                                                    

  Maintain complete transaction and tax records    0           0.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

**Key Findings**

The most frequently surfaced prevention language relates to verifying
platform legitimacy and avoiding unsolicited outreach. A smaller share
of incidents explicitly reference withdrawal-fee dynamics. Several
actions show zero explicit coverage in prevention text this week,
indicating either absence of those guidance statements in records or
prevention text that did not map into the locked action set.

**Top Prevention Actions by Coverage**

Top three actions by coverage:

1.  **Verify platform legitimacy before use**

2.  **Avoid unsolicited messages calls and DMs**

3.  **Do not pay fees to unlock withdrawals**

**Combined coverage:** **50.0%** of total incidents.

**Interpretation (NON-SPECULATIVE)**

Coverage is concentrated in a small number of actions, while a
substantial portion of incidents contain prevention text that is present
but not mappable into the locked action set. This limits how much of the
dataset can be expressed in standardized action terms and means
normalized coverage metrics represent a lower bound.

**Role in the Weekly Series**

This report provides a weekly snapshot of prevention coverage normalized
into a fixed action set, supporting longitudinal comparison across weeks
while preserving deterministic, audit-friendly counts.

**Bottom Line**

This week's dataset shows that explicit prevention mapping is dominated
by a few actions, while **25 of 56 incidents** contain prevention text
that does not map into the locked action set. Zero-coverage actions
should be interpreted as "not explicitly present in mappable form"
rather than absence of relevance.
