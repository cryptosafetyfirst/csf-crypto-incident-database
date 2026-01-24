**CW03 Prevention Action Normalization Report**

**Stage:** Prevention Action Normalization (Publication)\
**Scope:** CWXX Crypto & Web3 Incident Dataset\
**Total Incidents Analyzed:** **73**

------------------------------------------------------------------------

**Purpose**

This report presents a normalized view of prevention guidance extracted
from real crypto and Web3 incident records. Prevention normalization
measures how often specific, explicitly stated prevention actions appear
across incidents. All mappings are constrained to a locked prevention
action set, ensuring consistency, comparability, and auditability across
datasets and reporting periods.

------------------------------------------------------------------------

**Methodology Summary**

Prevention actions are mapped exclusively from the **prevention** field
of each incident record. Mapping is conservative: only explicitly stated
guidance is normalized, and no best practices are inferred. Incidents
may map to multiple prevention actions, but each incident is counted at
most once per action. Records with classification warnings are handled
with additional caution, and vague, narrative, or incompatible
prevention text is left unmapped.

------------------------------------------------------------------------

**Data Integrity Notes**

- **Total incidents analyzed:** 73

- **Incidents with classification warnings:** 4

- **Incidents with missing prevention text:** 0

- **Incidents with present but unmappable prevention text:** 33

- **Entry number integrity issues:** None detected (all entry numbers
  were unique integers)

Because a substantial portion of incidents contain prevention text that
is vague or incompatible with the locked action set, normalized coverage
should be interpreted as a **lower bound** on prevention guidance
explicitly stated in the dataset.

------------------------------------------------------------------------

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            18          24.7

  Avoid unsolicited messages calls and DMs         10          13.7

  Never share recovery phrases or private keys     2           2.7

  Do not pay fees to unlock withdrawals            5           6.8

  Use hardware wallets for long term storage       3           4.1

  Enable strong authentication and account         0           0.0
  security                                                     

  Confirm network and address compatibility before 2           2.7
  transfers                                                    

  Test transactions with small amounts first       0           0.0

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    0           0.0
  regularly                                                    

  Maintain complete transaction and tax records    8           11.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

------------------------------------------------------------------------

**Key Findings**

Explicit prevention guidance appears unevenly across incidents. A small
subset of actions accounts for most normalized coverage, while several
actions in the locked set do not appear at all. Nearly half of all
incidents include prevention language that could not be normalized due
to vagueness or incompatibility with the fixed action set.

------------------------------------------------------------------------

**Top Prevention Actions by Coverage**

1.  **Verify platform legitimacy before use** --- 24.7%

2.  **Avoid unsolicited messages calls and DMs** --- 13.7%

3.  **Maintain complete transaction and tax records** --- 11.0%

**Combined coverage:** **49.3%** of incidents (based on summed action
counts)

------------------------------------------------------------------------

**Interpretation (Non-Speculative)**

The distribution shows that explicit prevention guidance is concentrated
in a limited number of clearly articulated actions, while many incidents
lack directly mappable prevention statements. The absence of coverage
for several actions reflects the structure and specificity of the
recorded prevention text rather than the irrelevance of those actions.

------------------------------------------------------------------------

**Role in the Weekly Series**

This report serves as a weekly snapshot of normalized prevention
guidance derived from incident records. It supports longitudinal
comparison across weeks and anchors prevention coverage metrics in a
consistent, repeatable framework.

------------------------------------------------------------------------

**Bottom Line**

Only a subset of prevention actions is explicitly articulated across
incidents, and a significant share of prevention text remains unmappable
under conservative normalization rules. The value of this report lies in
its measurability and consistency, not in completeness or prescriptive
guidance.
