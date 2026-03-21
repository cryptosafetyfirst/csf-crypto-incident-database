**CSF Rule Alignment Snapshot --- CW12 2026**

**Dataset Scope**

Total incidents analyzed: 43

------------------------------------------------------------------------

**Rule Alignment Summary**

  ----------------------------------
  **Metric**             **Value**
  ---------------------- -----------
  Total incidents        43

  Incidents aligned to   43
  ≥1 CSF rule            

  Alignment coverage     100.0%
  ----------------------------------

All incidents map to at least one normalized prevention action, enabling
full downstream rule alignment coverage.

------------------------------------------------------------------------

**Rule Coverage Table**

  ---------------------------------------------------------------
  **CSF Rule (Derived from Prevention       **Count**   **% of
  Action)**                                             Total**
  ----------------------------------------- ----------- ---------
  Verify platform legitimacy before use     20          46.5

  Avoid unsolicited messages calls and DMs  11          25.6

  Never share recovery phrases or private   6           14.0
  keys                                                  

  Confirm network and address compatibility 4           9.3
  before transfers                                      

  Test transactions with small amounts      4           9.3
  first                                                 

  Revoke token approvals and review         4           9.3
  permissions regularly                                 

  Do not pay fees to unlock withdrawals     1           2.3

  Maintain complete transaction and tax     1           2.3
  records                                               

  Use hardware wallets for long term        0           0.0
  storage                                               

  Enable strong authentication and account  0           0.0
  security                                              

  Limit browser extensions and keep         0           0.0
  browsers updated                                      

  Minimize public exposure of crypto        0           0.0
  holdings                                              
  ---------------------------------------------------------------

Counts and percentages reflect normalized prevention mappings.

------------------------------------------------------------------------

**Layer Coverage Table**

  ------------------------------------
  **CSF Layer**  **Count**   **% of
                             Total**
  -------------- ----------- ---------
  Behavioral     36          83.7
  Controls                   

  Transaction    8           18.6
  Controls                   

  Tooling        4           9.3
  Controls                   

  Structural     0           0.0
  Controls                   
  ------------------------------------

Notes:

- Behavioral controls dominate due to high incidence of verification,
  communication, and credential exposure failures.

- Structural controls show no direct mappings in this dataset based on
  normalized prevention actions.

------------------------------------------------------------------------

**Residual / Uncertain Mappings**

  ---------------------------------
  **Category**          **Value**
  --------------------- -----------
  Unmapped incidents    0

  Residual / uncertain  0
  mappings              
  ---------------------------------

All incidents contain at least one mappable prevention action.\
No missing or fully unmappable prevention text cases were identified.

Classification warnings affect 4 records (entry numbers: 3, 4, 7, 14),
and mappings for these were performed conservatively.

------------------------------------------------------------------------

**Method Note**

This snapshot represents downstream research alignment only.\
It maps normalized prevention actions to CSF rules without altering
incident classifications, taxonomy structure, or prevention definitions.
