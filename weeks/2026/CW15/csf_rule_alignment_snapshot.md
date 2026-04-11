**CSF Rule Alignment Snapshot --- CW15 2026**

**Dataset Scope**

Total incidents analyzed: 41

------------------------------------------------------------------------

**Rule Alignment Summary**

Incidents aligned to at least one CSF rule: 32

Alignment is derived strictly from normalized prevention actions.\
Incidents with present but unmappable prevention text are treated as not
aligned under strict mapping constraints.

------------------------------------------------------------------------

**Rule Coverage Table**

  ----------------------------------------------------------------------
  **CSF Rule (Derived from Prevention Actions)**   **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            10          24.4

  Avoid unsolicited messages calls and DMs         5           12.2

  Do not pay fees to unlock withdrawals            7           17.1

  Enable strong authentication and account         2           4.9
  security                                                     

  Confirm network and address compatibility before 2           4.9
  transfers                                                    

  Test transactions with small amounts first       1           2.4

  Revoke token approvals and review permissions    2           4.9
  regularly                                                    

  Maintain complete transaction and tax records    5           12.2

  Never share recovery phrases or private keys     0           0.0

  Use hardware wallets for long term storage       0           0.0

  Limit browser extensions and keep browsers       0           0.0
  updated                                                      

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

------------------------------------------------------------------------

**Layer Coverage Table**

  ------------------------------------
  **Defensive    **Count**   **% of
  Layer**                    Total**
  -------------- ----------- ---------
  Behavioral     28          68.3

  Tooling        4           9.8

  Structural     0           0.0
  ------------------------------------

Notes:

- Behavioral layer dominates due to decision-point failures such as
  platform verification, communication handling, and fee/payment
  decisions.

- Tooling layer appears where authentication controls, approval
  management, and recordkeeping are explicitly mapped.

- Structural layer is not triggered under strict prevention-text mapping
  for this dataset.

- Multi-layer overlap exists, but primary alignment is used for
  determinism.

------------------------------------------------------------------------

**Residual / Uncertain Mappings**

Unmapped incidents: 9

Drivers of residuals:

- Prevention text present but not mappable to locked action set (9
  incidents)

- Classification warnings affecting mapping confidence (2 incidents)

Residual cases were not force-mapped to preserve rule integrity.

------------------------------------------------------------------------

**Method Note**

This snapshot reflects downstream research alignment of normalized
prevention actions to the CSF rule set.

It does not introduce new mappings, reinterpret incidents, or modify
prevention logic.
