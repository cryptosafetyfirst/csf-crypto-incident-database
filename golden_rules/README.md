**Golden Rules --- Preventive Intelligence Layer**

This directory contains the **CSF Golden Rules system**, a governed
preventive layer derived from structured crypto and Web3 incident
intelligence.

Golden Rules are:

- Immutable, versioned, single-sentence preventive heuristics

- Derived after incident ingestion and classification are complete

- Grounded in recurrence density (not severity)

- Tested weekly against canonical incident datasets

- Advisory only

They do not:

- Modify incident records

- Alter taxonomy or verdicts

- Influence classification decisions

- Act as detection logic

Intelligence informs rules.\
Rules never inform intelligence.

------------------------------------------------------------------------

**System Structure**

**/schema/**

Contains the formal Golden Rule Schema definition (current version).

Defines:

- Required rule fields

- Governance constraints

- Versioning requirements

- Weekly testing contract

------------------------------------------------------------------------

**/registry/**

Contains the active Golden Rule registry.

Each rule includes:

- rule_id

- rule_version

- rule_status

- rule_statement

- applicable incident types

- preventive action type

- recurrence-derived confidence

- historical observation window

Registry files are version-controlled.\
Rules evolve only via explicit governance action.

------------------------------------------------------------------------

**/weeks/**

Contains deterministic weekly rule testing outputs.

Structure:

weeks/{year}/{week_scope_label}/

Each week may include:

- GoldenRule_CoverageMatrix.csv

- GoldenRule_CoverageSummary.csv

- Governance_flag_report.csv

- Candidate_pattern_sheet.csv

- Snapshot render (optional)

Weekly artifacts:

- Declare scope type and date range

- Record orchestrator version

- Use the active registry version

- Do not reinterpret incident truth

------------------------------------------------------------------------

**Weekly Testing Model**

For each incident in scope, each active rule is evaluated with one of
three outcomes:

- prevented

- not_prevented (if deterministically supported)

- not_applicable

No partial credit.\
No narrative reinterpretation.\
No probabilistic scoring.

Coverage summaries and governance flags are derived mechanically from
this matrix.

------------------------------------------------------------------------

**Governance Boundary**

Golden Rules are a preventive distillation layer.

They exist to answer one question:

What single behavior would have prevented this loss?

They do not replace incident analysis.\
They do not override classification.\
They do not modify canonical records.

All incident truth resides in the canonical dataset.

------------------------------------------------------------------------

**Reproducibility**

Each weekly Golden Rules artifact is reproducible using:

- The canonical incident dataset for that week

- The active Golden Rule registry

- The applicable schema version

- The declared orchestrator version

All artifacts are version-controlled for longitudinal integrity.

------------------------------------------------------------------------

**Status**

This layer operates under active governance and strict separation from
ingestion and classification stages.

Golden Rules compress intelligence into measurable preventive behaviors
--- without contaminating the underlying intelligence system.
