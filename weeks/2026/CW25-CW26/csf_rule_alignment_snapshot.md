**CSF Rule Alignment Snapshot**

**Dataset Scope**

  ---------------------------------------------------
  **Metric**                         **Value**
  ---------------------------------- ----------------
  Week                               CW25+CW26 2026

  Total incidents analyzed           74

  Incidents aligned to at least one  74
  CSF Rule                           

  Residual / unmapped incidents      0
  ---------------------------------------------------

**Rule Alignment Summary**

The observed incident set aligns with the existing CSF Defensive Rule
Canon without requiring additions or modifications. Rule recurrence
remains concentrated within established defensive themes, particularly
platform legitimacy verification, avoidance of unsolicited contact,
advance-fee fraud prevention, wallet recovery protection, and
operational separation of assets. Alignment remains consistent with
existing normalization outputs and no governance escalation threshold
was identified. Residual mappings remain advisory only.

**Rule Coverage**

  --------------------------------------------------------------------------
  **Rule**                                                 **Occurrences**
  -------------------------------------------------------- -----------------
  SDR-007 --- Verify Platform Legitimacy                   44

  SDR-001 --- Ignore Unsolicited Contacts                  30

  SDR-006 --- Never Pay Advance Fees                       19

  SDR-005 --- Verify Websites Before Connecting Wallets    19

  SDR-004 --- Verify Wallet Requests Before Signing        11

  SDR-002 --- Verify Investment Opportunities              10
  Independently                                            

  SDR-003 --- Independently Verify Identities              9

  OR-001 --- Test Recovery Before It Is Needed             7

  OR-002 --- Maintain Multiple Secure Backups              7

  OR-004 --- Protect Recovery Phrases and Private Keys     4

  OR-008 --- Review Wallet Permissions Regularly           4

  HDR-001 --- Resist Social Engineering Attacks            3

  OR-005 --- Enable Strong Authentication                  3

  OR-006 --- Verify Addresses and Networks Before Sending  3

  OR-007 --- Maintain Recovery Documentation               3

  HDR-004 --- Protect Devices from Malware                 1

  HDR-010 --- Install Wallets and Extensions Only from     1
  Trusted Sources                                          

  GR-008 --- Separate Assets According to Risk             74
  --------------------------------------------------------------------------

**Defensive Layer Coverage**

  ---------------------------------
  **Defensive     **Occurrences**
  Layer**         
  --------------- -----------------
  Behavioral      133

  Operational     17

  Structural      74

  Tooling-based   8
  ---------------------------------

**Residual / Uncertain Mappings**

  ---------------------------------------------
  **Category**                **Occurrences**
  --------------------------- -----------------
  Unmapped incidents          0

  Uncertain rule mappings     0

  Normalization friction      6

  Classification ambiguity    41
  visibility                  
  ---------------------------------------------

Normalization friction originated from prevention statements that were
present but not sufficiently specific for deterministic rule assignment.
Classification ambiguity reflects records carrying classification
warnings while remaining successfully normalized within the existing
defensive canon. No incident required creation of a new defensive rule,
modification of an existing rule, or override of canonical prevention
mappings.

**Method Note**

This report is a downstream governance visibility artifact.

It does not modify canonical incident records, taxonomy classifications,
prevention mappings, or the CSF Rule Registry. Its purpose is solely to
provide visibility into alignment between observed incident prevention
mappings and the existing defensive rule canon.
