**Governance Notes**

**1. Dataset Integrity Confirmation**

- Incident count (43) is consistent across:

  - manifest

  - taxonomy analytics

  - prevention normalization outputs

- Hash integrity is preserved and matches manifest declaration:

  - AEC6D03B29052D8863ADED7CF70FF73CEB85BA8669106C5212D1F7579E9E45C2

**2. Orchestrator Consistency**

- Orchestrator version is stable: v1.4

- No schema drift or version mismatch detected across artifacts.

**3. Taxonomy Governance Signals**

- Invalid subtype usage detected:

  - investment_scam appears in 6 records

- This constitutes a **taxonomy boundary violation** (locked taxonomy
  not respected).

- Presence of repeated invalid subtype indicates:

  - **taxonomy pressure signal (within-run)**

- No corrective action taken (immutability preserved).

**4. Classification Warning Governance**

- 4 incidents contain classification warnings:

  - entry numbers: 3, 4, 7, 14

- One explicit signal:

  - "taxonomy pressure resolved"

- Implication:

  - localized classification uncertainty exists

  - normalization and analytics were correctly executed under
    conservative rules

**5. Prevention Mapping Integrity**

- All incidents contained mappable prevention text:

  - no missing prevention fields

  - no fully unmappable records

- However:

  - partial vagueness present in some records

  - coverage must be interpreted as **lower-bound deterministic
    mapping**

**6. Cross-Stage Consistency**

- No contradictions detected between:

  - taxonomy distribution (Stage 2)

  - prevention normalization (Stage 3)

- Dominant incident type (scam \~74%) aligns with:

  - high concentration of platform verification and unsolicited contact
    avoidance actions

**7. Determinism & Reproducibility**

- All outputs satisfy:

  - zero-fill enforcement

  - fixed taxonomy usage

  - locked prevention action set

- Given identical inputs:

  - outputs are reproducible without variance

**8. Audit Readiness**

- Dataset is fully auditable due to:

  - manifest completeness (all incident IDs listed)

  - cryptographic hash linkage

  - explicit anomaly disclosure (taxonomy + warnings)

- No silent corrections or inferred adjustments detected

------------------------------------------------------------------------

**End of Report**
