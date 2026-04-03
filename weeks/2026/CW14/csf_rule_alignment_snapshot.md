**CSF Rule Alignment Snapshot --- CW14 2026**

------------------------------------------------------------------------

**Dataset Scope**

Total incidents analyzed: 37

------------------------------------------------------------------------

**Rule Alignment Summary**

Incidents aligned to at least one CSF rule: 26

Alignment is derived from normalized prevention actions.\
Incidents without mappable prevention actions are treated as not aligned
under strict mapping constraints.

------------------------------------------------------------------------

**Rule Coverage Table**

  ----------------------------------------------------------------------
  **CSF Rule (Derived from Prevention Actions)**   **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            14          37.8

  Avoid unsolicited messages calls and DMs         8           21.6

  Do not pay fees to unlock withdrawals            5           13.5

  Confirm network and address compatibility before 4           10.8
  transfers                                                    

  Enable strong authentication and account         1           2.7
  security                                                     

  Test transactions with small amounts first       1           2.7

  Never share recovery phrases or private keys     0           0.0

  Use hardware wallets for long term storage       0           0.0

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Revoke token approvals and review permissions    0           0.0
  regularly                                                    

  Maintain complete transaction and tax records    0           0.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

------------------------------------------------------------------------

**Layer Coverage Table**

  ------------------------------------
  **Defensive    **Count**   **% of
  Layer**                    Total**
  -------------- ----------- ---------
  Behavioral     25          67.6

  Tooling        1           2.7

  Structural     0           0.0
  ------------------------------------

Notes:

- Behavioral layer dominates due to decision-point failures such as
  platform verification, communication handling, and transaction
  validation.

- Tooling appears minimally where explicitly mapped (authentication
  controls).

- Structural layer is not triggered under strict prevention-text mapping
  for this week.

- Multi-layer overlap exists but primary alignment is used for
  determinism.

------------------------------------------------------------------------

**Residual / Uncertain Mappings**

Unmapped incidents: 11

Drivers of residuals:

- Prevention text present but not mappable to locked action set (11
  incidents)

- Classification warnings affecting mapping confidence (7 incidents)

Residual cases were not force-mapped to preserve rule integrity.

------------------------------------------------------------------------

**Method Note**

This snapshot reflects downstream alignment of normalized prevention
actions to the CSF rule set.

It does not introduce new mappings, reinterpret incidents, or modify
prevention logic.
