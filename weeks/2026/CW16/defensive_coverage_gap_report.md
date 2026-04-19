**Defensive Coverage Gap Report --- CW16 2026**

**Inputs Declared (CW16)**

- incidents.csv (CW16)

- taxonomy_report.md (CW16)

- prevention_report.md (CW16)

- governance_notes.md (CW16)

- manifest.md (CW16)

**Defensive Canon Availability**

All required defensive materials were identified and available at
generation time:

- Practical Crypto & Web3 Safety Tools (canonical snapshot)

- Three-Wallet Model (canonical description)

- CSF Hacks Guidebook

- CSF Scams Guidebook

- CSF User Mistakes Guidebook

------------------------------------------------------------------------

**Dataset Scope**

Total incidents analyzed: 55

Dominant prevention failure points are derived from normalized
prevention coverage.

------------------------------------------------------------------------

**Defensive Coverage Assessment**

  -----------------------------------------------------------------------------
  **Prevention Failure **Coverage   **Coverage   **Canonical Basis**
  Point**              Status**     Type**       
  -------------------- ------------ ------------ ------------------------------
  Failure to verify    covered      tooling /    Safety Tools (domain
  platform legitimacy               behavioral   verification, archive tools);
                                                 Scams Guide (platform
                                                 validation patterns)

  Engagement with      covered      behavioral   Scams Guide (social
  unsolicited messages                           engineering, impersonation
  and impersonation                              mechanisms); Hacks Guide
                                                 (social engineering vectors)

  Failure to maintain  covered      tooling /    Safety Tools (portfolio & tax
  transaction and tax               behavioral   trackers); User Mistakes Guide
  records                                        (recordkeeping and
                                                 auditability)

  Incorrect network or covered      behavioral   User Mistakes Guide
  address usage                                  (transaction errors, wrong
                                                 network/address handling)

  Sharing sensitive    covered      behavioral   Scams Guide (seed phrase theft
  credentials or keys                            patterns); Hacks Guide
                                                 (credential compromise)

  Paying fees to       covered      behavioral   Scams Guide (exchange scams,
  unlock withdrawals                             pay-to-withdraw mechanisms)

  Failure to test      covered      behavioral   User Mistakes Guide
  transactions before                            (transaction verification
  full transfer                                  practices)

  Lack of              covered      tooling /    Safety Tools (hardware
  hardware-based key                structural   wallets); Three-Wallet Model
  isolation                                      (custody segmentation)

  Weak authentication  covered      tooling      Safety Tools (2FA, security
  and account                                    keys); Hacks Guide (account
  protection                                     takeover prevention)

  Unreviewed or        covered      tooling      Safety Tools (approval
  persistent token                               management tools); Scams Guide
  approvals                                      (smart contract abuse)
  -----------------------------------------------------------------------------

------------------------------------------------------------------------

**Residual / Uncovered Areas**

No dominant prevention failure points were identified as fully uncovered
within the current defensive canon.

A subset of incidents contains prevention language that is present but
not expressible within the normalized action set. These cases do not
constitute uncovered defensive gaps, as corresponding defensive
mechanisms exist within the canon but are not directly represented in
the mapped action set.

**Method Note**

This report evaluates alignment between observed prevention failure
points and existing defensive materials.

It does not introduce new defensive measures, reinterpret incidents, or
assess effectiveness.
