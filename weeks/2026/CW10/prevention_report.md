**CW10 Prevention Action Normalization Report**

**Stage:** Prevention Action Normalization (Publication)\
**Scope:** CW10 Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** 44

------------------------------------------------------------------------

**Purpose**

This report presents normalized prevention actions derived from a
dataset of crypto and Web3 security incidents. Prevention normalization
measures how often actionable safety guidance appears across incidents
when mapped to a standardized prevention action set. The guidance
reflected in this report originates from real incident records and is
constrained to a fixed set of prevention actions to ensure comparability
across datasets.

------------------------------------------------------------------------

**Methodology Summary**

Prevention guidance is mapped conservatively using only the
**prevention** field of each incident record. When prevention text
clearly corresponds to one or more allowed actions, the incident is
mapped accordingly. Multiple actions may be mapped to a single incident
when explicitly supported by the prevention text.

If prevention text is vague, narrative, or incompatible with the
standardized prevention action set, no mapping is forced. In such cases,
the prevention text is treated as present but unmappable.

Incidents with classification warnings are interpreted conservatively
during normalization, which may reduce mapping confidence.

------------------------------------------------------------------------

**Data Integrity Notes**

Total incidents analyzed: **44**

Incidents with classification warnings: **8**

Incidents with missing prevention text: **0**

Incidents with present but unmappable prevention text: **0**

Entry number integrity issues: **none detected**

------------------------------------------------------------------------

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            13          29.5

  Avoid unsolicited messages calls and DMs         10          22.7

  Never share recovery phrases or private keys     6           13.6

  Do not pay fees to unlock withdrawals            5           11.4

  Use hardware wallets for long term storage       0           0.0

  Enable strong authentication and account         0           0.0
  security                                                     

  Confirm network and address compatibility before 2           4.5
  transfers                                                    

  Test transactions with small amounts first       0           0.0

  Limit browser extensions and keep browsers       1           2.3
  updated                                                      

  Revoke token approvals and review permissions    1           2.3
  regularly                                                    

  Maintain complete transaction and tax records    2           4.5

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

------------------------------------------------------------------------

**Key Findings**

The most frequently occurring normalized prevention action is **Verify
platform legitimacy before use**, appearing in 13 incidents (29.5% of
the dataset).

The next most common actions are **Avoid unsolicited messages calls and
DMs** (22.7%) and **Never share recovery phrases or private keys**
(13.6%).

Several actions appear only rarely, including **Limit browser extensions
and keep browsers updated** and **Revoke token approvals and review
permissions regularly**, each appearing in a single incident.

Four actions do not appear in the dataset: **Use hardware wallets for
long term storage**, **Enable strong authentication and account
security**, **Test transactions with small amounts first**, and
**Minimize public exposure of crypto holdings**.

------------------------------------------------------------------------

**Top Prevention Actions by Coverage**

1.  Verify platform legitimacy before use --- 29.5%

2.  Avoid unsolicited messages calls and DMs --- 22.7%

3.  Never share recovery phrases or private keys --- 13.6%

Combined coverage of the top three actions: **65.9% of incidents**

------------------------------------------------------------------------

**Interpretation**

The normalized distribution shows that prevention guidance most
frequently focuses on verifying the legitimacy of platforms and avoiding
unsolicited communication. A smaller portion of incidents reference seed
phrase protection and withdrawal fee scams.

Several prevention actions defined in the standardized action set do not
appear in the dataset, indicating that explicit guidance corresponding
to those categories is not present in the incident prevention fields for
this week.

------------------------------------------------------------------------

**Role in the Weekly Series**

This report provides a weekly snapshot of normalized prevention coverage
derived from the incident dataset. Using a fixed prevention action set
and deterministic mapping rules allows prevention coverage metrics to
remain comparable across weeks and supports longitudinal analysis of
prevention guidance trends.

------------------------------------------------------------------------

**Bottom Line**

In CW10, normalized prevention coverage is concentrated in three areas:
platform legitimacy verification, avoiding unsolicited contact, and
protecting recovery phrases. Together these actions account for **65.9%
of incidents** with mappable prevention guidance.

Other prevention categories appear rarely or not at all in the dataset,
highlighting areas where explicit prevention language is absent from
incident records.
