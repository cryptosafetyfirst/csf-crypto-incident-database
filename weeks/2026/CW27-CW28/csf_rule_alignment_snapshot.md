**CSF Rule Alignment Snapshot --- CW27 + CW28 2026**

**Dataset Scope**

  --------------------------------------------------
  **Metric**                        **Value**
  --------------------------------- ----------------
  Week                              CW27 + CW28 2026

  Total incidents analyzed          63

  Incidents aligned to at least one 52
  CSF rule                          

  Residual / unmapped incidents     11
  --------------------------------------------------

------------------------------------------------------------------------

**Rule Alignment Summary**

Rule alignment remains concentrated within a small number of recurring
defensive behaviors. Platform verification continues to account for most
mapped incidents, followed by avoidance of unsolicited contacts and
refusal to make withdrawal-related payments. Residual mappings remain
limited to prevention statements that could not be conservatively
normalized into the locked rule set. Recurrence remains concentrated
within existing governance expectations, and no governance escalation
threshold was identified.

------------------------------------------------------------------------

**Rule Coverage Table**

  ------------------------------------------------------------------
  **Rule**                                         **Occurrences**
  ------------------------------------------------ -----------------
  Verify platform legitimacy before use            36

  Avoid unsolicited messages, calls and DMs        13

  Do not pay fees to unlock withdrawals            8

  Never share recovery phrases or private keys     5

  Confirm network and address compatibility before 4
  transfers                                        

  Revoke token approvals and review permissions    4
  regularly                                        

  Use hardware wallets for long-term storage       2

  Test transactions with small amounts first       2

  Maintain complete transaction and tax records    2
  ------------------------------------------------------------------

------------------------------------------------------------------------

**Layer Coverage Table**

  ---------------------------------
  **Defensive     **Occurrences**
  Layer**         
  --------------- -----------------
  Behavioral      62

  Operational     6

  Structural      4

  Tooling-based   4
  ---------------------------------

------------------------------------------------------------------------

**Residual / Uncertain Mappings**

Residual mappings remain advisory only.

  -----------------------------------------------------------------------
  **Observation**            **Value**
  -------------------------- --------------------------------------------
  Incidents with unmappable  11
  prevention guidance        

  Incidents with             28
  classification warnings    

  Missing prevention         0
  guidance                   

  Normalization status       Conservative mapping applied

  Ambiguity visibility       Present through declared classification
                             warnings and unmappable prevention
                             statements
  -----------------------------------------------------------------------

Classification warnings and unmappable prevention guidance reduce
normalization confidence but do not alter canonical prevention mappings
or reported coverage.

------------------------------------------------------------------------

**Method Note**

This report is a downstream governance visibility artifact only.

It does not modify canonical incident records, taxonomy classifications,
prevention mappings, or the CSF Defensive Rule Canon. It provides
observational visibility into current-week defensive rule alignment
based exclusively on declared weekly inputs.
