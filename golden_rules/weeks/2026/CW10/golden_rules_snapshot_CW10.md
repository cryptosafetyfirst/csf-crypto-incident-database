**CW10 Golden Rules --- Registry Snapshot (2026-CW10)**

Status: Derived\
week_scope_label: 2026-CW10\
week_scope_type: csf_report_window\
date_range_start: 2026-02-27\
date_range_end: 2026-03-06\
incident_count_in_scope: 44\
orchestrator_version: v1.4\
rule_registry_version: v1\
authority_boundary: Advisory only

------------------------------------------------------------------------

**GR-001 v1**

Rule Statement:\
Never share your seed phrase, private key, or recovery words under any
circumstance.

rule_status: Active

preventive_action_type: Behavioral

applies_to_incident_types: scam, hack

failure_pattern_blocked: secret disclosure inside impersonated or
malicious interface

first_observed_week: 2025-W38

last_observed_week: 2026-CW10

confidence_level: high

evidence_incident_count (CW10): 10

evidence_week_count: 15

------------------------------------------------------------------------

**GR-002 v1**

Rule Statement:\
Always verify the full URL and domain independently before connecting
your wallet or logging in.

rule_status: Active

preventive_action_type: Behavioral

applies_to_incident_types: scam, hack

failure_pattern_blocked: trust granted to attacker-controlled platform

first_observed_week: 2025-W41

last_observed_week: 2026-CW10

confidence_level: high

evidence_incident_count (CW10): 13

evidence_week_count: 13

------------------------------------------------------------------------

**GR-003 v1**

Rule Statement:\
Never pay fees, taxes, insurance, or verification deposits to unlock or
withdraw existing funds.

rule_status: Active

preventive_action_type: Behavioral

applies_to_incident_types: scam

failure_pattern_blocked: pay-to-withdraw extraction loop

first_observed_week: 2025-W44

last_observed_week: 2026-CW10

confidence_level: high

evidence_incident_count (CW10): 6

evidence_week_count: 11

------------------------------------------------------------------------

**GR-004 v1**

Rule Statement:\
Never follow real-time "support" or "security" instructions from
unsolicited messages, calls, or direct messages.

rule_status: Active

preventive_action_type: Behavioral

applies_to_incident_types: scam, hack

failure_pattern_blocked: engagement inside attacker-controlled
communication channel

first_observed_week: 2025-W46

last_observed_week: 2026-CW10

confidence_level: high

evidence_incident_count (CW10): 12

evidence_week_count: 12

------------------------------------------------------------------------

**GR-005 v1**

Rule Statement:\
Always review and revoke unused token approvals after interacting with
new smart contracts or dApps.

rule_status: Active

preventive_action_type: Operational

applies_to_incident_types: hack

failure_pattern_blocked: approval misuse and permission persistence

first_observed_week: 2025-W48

last_observed_week: 2026-CW10

confidence_level: Medium

evidence_incident_count (CW10): 2

evidence_week_count: 9

------------------------------------------------------------------------

**GR-006 v1**

Rule Statement:\
Always enable strong authentication and account security on exchanges,
wallets, and email accounts.

rule_status: Active

preventive_action_type: Technical

applies_to_incident_types: hack

failure_pattern_blocked: credential compromise and account takeover

first_observed_week: 2025-W40

last_observed_week: 2026-CW10

confidence_level: high

evidence_incident_count (CW10): 2

evidence_week_count: 14

------------------------------------------------------------------------

**GR-007 v1**

Rule Statement:\
Always confirm the full destination address and network before approving
or sending any transaction.

rule_status: Active

preventive_action_type: Operational

applies_to_incident_types: user_mistake, hack

failure_pattern_blocked: address substitution and network mismatch

first_observed_week: 2025-W39

last_observed_week: 2026-CW10

confidence_level: Medium

evidence_incident_count (CW10): 1

evidence_week_count: 16

------------------------------------------------------------------------

**GR-008 v1**

Rule Statement:\
Always maintain complete, recoverable wallet backups and transaction
records before you need them.

rule_status: Active

preventive_action_type: Operational

applies_to_incident_types: user_mistake

failure_pattern_blocked: irreversible loss due to recovery or
recordkeeping gaps

first_observed_week: 2025-W42

last_observed_week: 2026-CW10

confidence_level: Medium

evidence_incident_count (CW10): 1

evidence_week_count: 10

------------------------------------------------------------------------

**CW10 Structural Observations**

Dominant incident type: scam

Top prevention signal: verify platform legitimacy before use

No defensive coverage gap identified

No FAQ misalignment requiring structural update

Governance stability confirmed (no reclassification, no scope drift)

No new rule creation threshold triggered in CW10.\
No rule deprecation triggered.\
No rule logic modification required.

CW10 reinforces recurrence density inside:

- legitimacy verification

- pay-to-withdraw refusal

- secret protection

- authentication hygiene

- approval discipline

- operational custody readiness

These prevention behaviors remain the dominant early failure controls
across the CW10 incident corpus.

------------------------------------------------------------------------

**Mandatory Governance Footer**

Golden Rules are distilled preventive heuristics derived from observed
incidents.

They do not alter incident truth, classification, or attribution.

Intelligence informs rules.\
Rules never inform intelligence.
