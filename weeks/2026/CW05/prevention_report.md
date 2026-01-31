**CW05 Prevention Action Normalization Report**

Stage: Prevention Action Normalization (Publication)\
Scope: CW05 Crypto & Web3 Incident Dataset\
Total Incidents Analyzed: **80**

------------------------------------------------------------------------

**Purpose**

This report renders normalized prevention coverage derived from real
incident records. Prevention guidance is mapped conservatively from the
incident **prevention** field into a fixed, locked prevention action set
to support week-over-week comparability.

------------------------------------------------------------------------

**Methodology Summary**

- Prevention actions are mapped **only** from the prevention field.

- summary and user_mistake are used only to **clarify intent**, never to
  invent actions.

- Incidents may map to **multiple** actions.

- If classification_warning ≠ none, mappings are applied with **extra
  caution**.

- If prevention text is missing, vague, or incompatible with the locked
  action set, **no forced mapping** is performed.

------------------------------------------------------------------------

**Data Integrity Notes**

- Total incidents analyzed: **80**

- Incidents with classification warnings: **11** (entry numbers: 18, 19,
  32, 34, 41, 58, 59, 60, 61, 62, 75)

- Missing prevention text: **0**

- Present but unmappable prevention text: **36**

- Vague / non-actionable prevention text: **0**

Because unmappable prevention text exists, coverage figures should be
treated as a **lower bound** relative to the locked action set.

------------------------------------------------------------------------

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            7           8.8

  Avoid unsolicited messages calls and DMs         27          33.8

  Never share recovery phrases or private keys     1           1.2

  Do not pay fees to unlock withdrawals            4           5.0

  Use hardware wallets for long term storage       1           1.2

  Enable strong authentication and account         2           2.5
  security                                                     

  Confirm network and address compatibility before 1           1.2
  transfers                                                    

  Test transactions with small amounts first       0           0.0

  Limit browser extensions and keep browsers       1           1.2
  updated                                                      

  Revoke token approvals and review permissions    6           7.5
  regularly                                                    

  Maintain complete transaction and tax records    3           3.8

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

------------------------------------------------------------------------

**Key Findings**

- The most frequently mapped prevention action is **Avoid unsolicited
  messages calls and DMs** (33.8% of incidents).

- Secondary coverage appears in **Verify platform legitimacy before
  use** (8.8%) and **Revoke token approvals and review permissions
  regularly** (7.5%).

- Multiple actions have low or zero coverage within the locked set for
  this dataset (e.g., "Test transactions with small amounts first",
  "Minimize public exposure of crypto holdings").

------------------------------------------------------------------------

**Top Prevention Actions by Coverage**

Top 3 actions (ranked by count; ties would be broken alphabetically):

1.  Avoid unsolicited messages calls and DMs

2.  Verify platform legitimacy before use

3.  Revoke token approvals and review permissions regularly

Combined coverage: **50.0%**

------------------------------------------------------------------------

**Interpretation (NON-SPECULATIVE)**

The distribution shows that explicit prevention language most often maps
to avoiding unsolicited outreach, followed by basic legitimacy
verification and permission/approval hygiene. A substantial portion of
incidents contain prevention guidance that does not map cleanly into the
locked action set, meaning measured coverage is constrained by the fixed
taxonomy of actions.

------------------------------------------------------------------------

**Role in the Weekly Series**

This report provides a weekly prevention-coverage snapshot that supports
longitudinal comparison across weeks using a consistent, locked action
set and stable rendering structure.

------------------------------------------------------------------------

**Bottom Line**

Measured prevention coverage is concentrated in a small subset of locked
actions, while a meaningful share of incidents contain prevention text
that is not mappable to the fixed set. This report emphasizes
measurability and comparability over completeness.
