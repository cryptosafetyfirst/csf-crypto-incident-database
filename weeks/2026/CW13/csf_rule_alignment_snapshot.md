**CSF Rule Alignment Snapshot --- CW13 2026**

------------------------------------------------------------------------

**Dataset Scope**

Total incidents analyzed: 33

------------------------------------------------------------------------

**Rule Alignment Summary**

Incidents aligned to at least one CSF rule: 33

All incidents in the dataset map to at least one prevention action,
which serves as the proxy for CSF rule alignment.

------------------------------------------------------------------------

**Rule Coverage Table**

  ----------------------------------------------------------------------
  **CSF Rule (Derived from Prevention Actions)**   **Count**   **% of
                                                               Total**
  ------------------------------------------------ ----------- ---------
  Verify platform legitimacy before use            6           18.2

  Do not pay fees to unlock withdrawals            6           18.2

  Confirm network and address compatibility before 4           12.1
  transfers                                                    

  Avoid unsolicited messages calls and DMs         3           9.1

  Never share recovery phrases or private keys     2           6.1

  Enable strong authentication and account         2           6.1
  security                                                     

  Revoke token approvals and review permissions    2           6.1
  regularly                                                    

  Use hardware wallets for long term storage       1           3.0

  Test transactions with small amounts first       1           3.0

  Limit browser extensions and keep browsers       1           3.0
  updated                                                      

  Maintain complete transaction and tax records    0           0.0

  Minimize public exposure of crypto holdings      0           0.0
  ----------------------------------------------------------------------

------------------------------------------------------------------------

**Layer Coverage Table**

  ------------------------------------
  **Defensive    **Count**   **% of
  Layer**                    Total**
  -------------- ----------- ---------
  Behavioral     27          81.8

  Tooling        6           18.2

  Structural     2           6.1
  ------------------------------------

Notes:

- Behavioral layer dominates due to decision-point failures
  (verification, communication handling, transaction validation).

- Tooling and structural layers appear where explicitly mapped (e.g.,
  approvals, hardware wallets).

- Multi-layer overlap exists; counts reflect primary alignment only for
  determinism.

------------------------------------------------------------------------

**Residual / Uncertain Mappings**

- Unmapped incidents: 0

- Residual ambiguity present in a subset of records due to:

  - classification warnings (4 incidents)

  - prevention text that is present but not fully aligned to the locked
    action set

These cases were conservatively mapped where possible without inference.

------------------------------------------------------------------------

**Method Note**

This snapshot reflects downstream alignment of normalized prevention
actions to the CSF rule set.\
It does not introduce new mappings, reinterpret incidents, or modify
prevention logic.
