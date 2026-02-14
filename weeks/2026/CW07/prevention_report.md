CW07 Prevention Action Normalization Report

Stage: Prevention Action Normalization (Publication)\
Scope: CW07 Crypto & Web3 Incident Dataset\
Total Incidents Analyzed: 79

------------------------------------------------------------------------

**Purpose**

This report presents a standardized normalization of prevention guidance
derived from real-world crypto and Web3 incidents. Prevention statements
are mapped strictly to a locked prevention action set to enable
comparability, auditability, and longitudinal measurement. All mappings
are constrained to predefined actions and are rendered mechanically from
canonical normalization output.

------------------------------------------------------------------------

**Methodology Summary**

Prevention actions are mapped exclusively from the prevention field of
each structured incident record. Summary and user mistake fields are
used only to clarify intent and never to invent or expand prevention
guidance.

Mapping is conservative:

- Only actions explicitly supported by prevention text are counted.

- Multiple actions may be mapped per incident.

- One incident is counted at most once per action.

- Vague, narrative, or incompatible prevention text is not forced into
  the locked action set.

- When classification warnings are present, normalization proceeds with
  elevated caution.

No reinterpretation or expansion of prevention guidance is permitted.

------------------------------------------------------------------------

**Data Integrity Notes**

- Total incidents analyzed: 79

- Incidents with classification warnings: 0

- Incidents with missing prevention text: 0

- Incidents with present but unmappable prevention text: 64

- Entry number integrity issues: None

Because 64 incidents contain prevention text that could not be
normalized within the locked action set, reported coverage represents a
lower bound of explicit, standardizable prevention language.

------------------------------------------------------------------------

**Normalized Prevention Actions --- Coverage Table**

  ----------------------------------------------------------------------
  **Prevention Action**                            **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            4           5.1

  Avoid unsolicited messages calls and DMs         2           2.5

  Never share recovery phrases or private keys     5           6.3

  Do not pay fees to unlock withdrawals            3           3.8

  Use hardware wallets for long term storage       1           1.3

  Enable strong authentication and account         1           1.3
  security                                                     

  Confirm network and address compatibility before 0           0.0
  transfers                                                    

  Test transactions with small amounts first       0           0.0

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    0           0.0
  regularly                                                    

  Maintain complete transaction and tax records    1           1.3

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

Percentages rounded to one decimal place.

------------------------------------------------------------------------

**Key Findings**

The most frequently occurring normalized prevention action is:

- Never share recovery phrases or private keys (6.3%)

This is followed by:

- Verify platform legitimacy before use (5.1%)

- Do not pay fees to unlock withdrawals (3.8%)

Several actions show zero coverage, including:

- Confirm network and address compatibility before transfers

- Test transactions with small amounts first

- Limit browser extensions and keep browsers updated

- Revoke token approvals and review permissions regularly

- Minimize public exposure of crypto holdings

Overall normalized coverage is concentrated in a small subset of the
locked action set.

------------------------------------------------------------------------

**Top Prevention Actions by Coverage**

1.  Never share recovery phrases or private keys --- 6.3%

2.  Verify platform legitimacy before use --- 5.1%

3.  Do not pay fees to unlock withdrawals --- 3.8%

Combined coverage of top three actions: 15.2%

------------------------------------------------------------------------

**Interpretation (NON-SPECULATIVE)**

Normalized coverage is limited to explicit prevention language
compatible with the locked action set. A substantial portion of
prevention text (64 out of 79 incidents) could not be mapped under
deterministic rules. As a result, measurable prevention coverage is
concentrated and mechanically constrained.

The absence of coverage for several actions reflects the lack of
explicit prevention references to those categories within this dataset.

------------------------------------------------------------------------

**Role in the Weekly Series**

This report serves as a weekly normalization snapshot of prevention
coverage across the CW07 incident dataset. It enables consistent
longitudinal comparison across reporting periods and anchors prevention
metrics to a fixed, deterministic action framework.

------------------------------------------------------------------------

**Bottom Line**

In CW07, normalized prevention coverage is limited and concentrated.
Only 15.2% of incidents map to the top three locked prevention actions,
and 64 incidents contain prevention text that cannot be standardized
within the current action taxonomy.

This report measures explicit, standardizable prevention language---not
total prevention intent---and provides a consistent baseline for
comparison across future weeks.
