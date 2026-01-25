# CSF Crypto Incident Intelligence Pipeline

**Orchestrator Specification --- v1.1**

**PUBLIC**

**Legal & IP Notice**

© 2026 Juan Pablo Renedo, operating as CryptoSafetyFirst (CSF). All
rights reserved.

This document ("CSF Crypto Incident Intelligence Pipeline ---
Orchestrator Specification") and its normative appendices are
intellectual property of CSF unless otherwise stated.

**License:** This specification is made available under the **Creative
Commons Attribution--NoDerivatives 4.0 International (CC BY-ND 4.0)**
license. You may copy and redistribute this document under the terms of
that license. You may not distribute modified versions of this document.
You must preserve this notice and provide appropriate attribution.

**No advice; no warranties:** This document is provided for
informational and educational purposes only. It is not legal, financial,
investment, incident response, or recovery advice. The document is
provided "AS IS" without warranties of any kind.

**No affiliation:** CSF is not affiliated with, endorsed by, or
sponsored by any third-party platforms, projects, or organizations
referenced in incident sources.

**Controlled execution artifacts:** Normative execution artifacts
(including prompt texts, tooling, and automation) may be
access-controlled and are not necessarily published in full, even when
referenced by this specification.

## Executive Overview

### Purpose

The **CSF Intelligence Pipeline** is a deterministic system for
collecting, structuring, and analyzing publicly reported crypto and Web3
security incidents.

Its purpose is to transform messy, unstructured incident reports (social
media posts, forums, news articles, and user accounts) into:

- **immutable, atomic incident records**, and

- **reproducible weekly intelligence artifacts** suitable for analysis,
  publication, and long-term archival.

The pipeline prioritizes **integrity, traceability, and
reproducibility** over speed, completeness, or narrative polish.

### Scope and Intended Use

This specification defines:

- how incidents are identified and uniquely indexed

- how raw incident text is converted into structured records

- how weekly analytical outputs are generated

- how governance and auditability are preserved over time

It is designed for use by:

- analysts and researchers

- safety educators and publishers

- downstream automation (dashboards, chatbots, APIs)

- auditors reviewing historical outputs

This system is **not** designed for real-time threat detection,
law-enforcement investigation, or blockchain forensics.

### Design Philosophy

The pipeline is built around five non-negotiable principles:

1.  **Atomic truth**\
    Each incident is captured once as an immutable record. Incidents are
    never silently edited or overwritten.

2.  **Stage isolation**\
    Every stage of the pipeline can be executed independently using only
    the data explicitly passed to it. No hidden state or cross-stage
    memory is allowed.

3.  **Determinism**\
    Given the same inputs, the pipeline must always produce the same
    outputs. Human judgment is confined to clearly defined pre-ingest
    steps.

4.  **Auditability over convenience**\
    The system favors explicit artifacts, hashes, manifests, and logs
    over convenience or automation shortcuts.

5.  **Governance visibility**\
    Ambiguity, uncertainty, and taxonomy pressure are surfaced
    explicitly rather than smoothed over.

### Mental Model

The pipeline operates across **three planes**:

- **Collection Plane**\
  Human-driven sourcing, deduplication, and identity assignment.

- **Intelligence Plane**\
  Deterministic, stage-based structuring and analysis of incidents.

- **Governance Plane**\
  Weekly integrity anchoring, traceability, and long-term trust
  management.

Each plane has clearly defined responsibilities and produces explicit
artifacts.

### What This Pipeline Does *Not* Do

To avoid misinterpretation, the following are **explicit non-goals**:

- It does not attempt to merge multiple sources into a single "canonical
  real-world incident."

- It does not infer attacker identity, attribution, or intent beyond
  what is explicitly stated.

- It does not retroactively reclassify incidents without explicit
  governance action.

- It does not guarantee completeness of coverage or real-time awareness.

- It does not provide investment, legal, or recovery advice.

These constraints are intentional and foundational to the system's
credibility.

### Stability and Versioning

This document defines **version v1.1** of the orchestrator.

- v1.x versions may introduce clarifications, documentation hardening,
  or non-breaking quality controls.

- v2.0 and beyond will be required for any breaking change to:

  - stage ordering

  - required inputs or outputs

  - taxonomy structure

  - prevention action sets

  - immutability guarantees

Weekly outputs MUST record the orchestrator version used to generate
them.

## How to Read This Specification

This document describes a **deterministic crypto incident intelligence
pipeline**.\
It is not a tutorial, a blog post, or a narrative report.

If you are new to this system, this page explains **how to approach the
spec**, **what matters**, and **what does not**.

### What This Spec Is (and Is Not)

**What this spec *is***

- A **formal execution contract** for how crypto and web3 incidents are
  collected, structured, and analyzed.

- A description of **inputs, stages, outputs, and invariants**.

- A reference for **reproducible weekly intelligence production**.

- A governance document designed to survive audits, automation, and
  time.

**What this spec *is not***

- Not a real-time monitoring system.

- Not a blockchain forensics framework.

- Not an investigation or attribution methodology.

- Not a guarantee of completeness or accuracy of public reports.

- Not investment, legal, or recovery advice.

If you are looking for *alerts*, *live feeds*, or *case narratives*,
this spec intentionally sits **one level below** that.

### How the Document Is Structured

The spec is organized around **planes, stages, and artifacts**.

**Planes (big picture)**

- **Collection Plane**\
  Human-driven sourcing, deduplication, and identity assignment.

- **Intelligence Plane**\
  Deterministic structuring and analysis using isolated stages.

- **Governance Plane**\
  Integrity, traceability, and long-term trust.

If you only want the *why*, read the **Executive Overview**.\
If you want the *how*, read the stage sections.

### How to Read the Pipeline Stages

Each stage is designed to be:

- **Isolated** --- it can run without knowing anything about other
  stages

- **Deterministic** --- same inputs → same outputs

- **Immutable** --- outputs are never silently modified later

When reading a stage, focus on:

1.  **Inputs** --- exactly what data is allowed in

2.  **Execution rules** --- what is explicitly forbidden

3.  **Outputs** --- what artifacts are produced

4.  **Boundary rules** --- what downstream stages may *not* do

If a rule seems "overly strict," that is intentional.

### How to Interpret the Prompts

Prompts in this spec are **not suggestions**.\
They are **locked execution contracts**.

Important implications:

- Prompts must be executable in isolation.

- Prompts may not rely on memory of previous runs.

- Prompts may not infer missing data.

- Prompts may surface ambiguity, but never resolve it silently.

If you are used to flexible LLM workflows, this will feel rigid by
design.

### How to Read the Outputs

**Canonical outputs**

Files under /incidents/ are **atomic and immutable**.\
They represent the system's source of truth.

**Weekly outputs**

Files under /weeks/YYYY/CWxx/ are:

- editorial snapshots

- fully regenerable

- traceable back to canonical incidents

If a weekly file conflicts with a canonical incident file,\
**the canonical incident always wins**.

### What "Immutability" Means Here

Immutability does **not** mean "never wrong."

It means:

- Errors are corrected by **creating new records**, not rewriting
  history.

- Taxonomy changes are **explicit and versioned**.

- Ambiguity is **surfaced**, not hidden.

This mirrors practices used in:

- vulnerability disclosure systems

- incident response timelines

- regulated reporting environments

### Known Trade-offs (Read This Before Critiquing)

Some things you might expect are **intentionally excluded**:

- Cross-source incident merging

- Lifecycle states ("resolved", "ongoing")

- Automatic reclassification

- Semantic duplicate detection

- Retrospective cleanup

These are design choices, not omissions.

They preserve:

- auditability

- reproducibility

- trust over time

### How to Use This Spec Practically

Depending on your role:

- **Analyst / Researcher**\
  Follow the stages strictly; treat outputs as immutable evidence.

- **Engineer / Automator**\
  Treat this as an API contract expressed in documents.

- **Reviewer / Auditor**\
  Validate that artifacts match declared inputs and versions.

- **Educator / Publisher**\
  Use weekly outputs, not canonical incident files, for narratives.

### Final Reading Advice

Do **not** read this spec linearly.

Recommended order:

1.  Executive Overview

2.  This page

3.  System Overview

4.  Stage 1 (Incident Ingest)

5.  Weekly Outputs & Governance

6.  Appendices (as needed)

If something feels constrained, ask:

"What failure mode is this preventing?"

The answer is usually: **silent drift**.

## 1. Introduction

### 1.1 Purpose and Scope

The **CSF Crypto Incident Intelligence Pipeline** defines a structured,
deterministic workflow for collecting, classifying, and analyzing
publicly reported crypto and Web3 security incidents.

The purpose of this specification is to establish a **clear, auditable
contract** for how raw incident signals---such as forum posts, social
media threads, and news articles---are transformed into:

- immutable, atomic incident records, and

- reproducible weekly intelligence artifacts.

This document specifies:

- the stages of the pipeline,

- the required inputs and outputs at each stage,

- the invariants that must be preserved, and

- the governance rules that prevent silent drift or retrospective
  alteration.

The scope of this pipeline is limited to **publicly observable incident
reporting** and **post-incident intelligence structuring**. It does not
attempt to detect incidents in real time, investigate on-chain activity,
or verify claims beyond the information explicitly present in source
materials.

This specification is intended to be stable, versioned, and suitable for
long-term reuse across research, publishing, and automation contexts.

### 1.2 Intended Audience

This specification is written for readers who need to **understand,
execute, review, or rely on** a crypto incident intelligence pipeline
with strong integrity guarantees.

Primary audiences include:

- **Analysts and researchers**\
  who collect, classify, and study crypto/Web3 security incidents.

- **Security educators and publishers**\
  who require reproducible datasets and weekly intelligence summaries
  without silent reinterpretation.

- **Engineers and automation designers**\
  who may build tooling, dashboards, APIs, or chatbots on top of
  structured incident data.

- **Reviewers, auditors, and collaborators**\
  who need to verify how incidents were processed and whether outputs
  can be trusted over time.

This document assumes:

- familiarity with basic crypto and Web3 concepts,

- comfort reading structured technical documentation,

- no prior knowledge of internal CSF tooling or workflows.

It is **not** written as an introductory guide for beginners or as a
narrative explanation of individual scams.

### 1.3 Non-Goals and Explicit Limitations

To avoid misinterpretation, the following are **explicit non-goals** of
this pipeline.

The CSF Crypto Incident Intelligence Pipeline does **not**:

- provide real-time monitoring, alerting, or threat detection,

- perform blockchain forensics or on-chain attribution,

- investigate or verify the truthfulness of incident claims beyond
  source text,

- merge multiple sources into a single "canonical real-world incident,"

- track incident lifecycles (e.g., resolved, ongoing, recovered),

- retroactively reclassify incidents without explicit governance action,

- offer legal, financial, recovery, or investment advice.

Additionally, the pipeline intentionally accepts the following
limitations:

- Duplicate detection is limited to URL equivalence, not semantic
  similarity.

- Incident records are immutable once ingested; corrections require new
  records.

- Prevention analysis reflects **recorded prevention text**, not
  theoretical preventability.

- Weekly outputs are snapshots and may be regenerated; canonical
  incident files are not.

These constraints are **intentional design choices**, made to preserve
auditability, reproducibility, and long-term trust at the expense of
convenience or apparent completeness.

**Public Reporting Reliability Notice**

Incident records reflect claims present in publicly available sources at
time of capture. CSF does not verify all claims, and records may contain
incomplete or disputed information. Where uncertainty exists, it is
surfaced via classification_warning. CSF does not assert criminal
attribution unless explicitly stated in the cited source.

### 1.4 Intellectual Property, Licensing, and Third-Party Content

This specification covers a workflow for processing **publicly
reported** crypto/Web3 incident information. The specification text and
its normative prompt contracts are published under the license stated in
the front matter.

Incident sources referenced by the pipeline (e.g., social media posts,
forum threads, articles) remain the intellectual property of their
respective authors and publishers. CSF does not claim ownership over
third-party source material.

CSF's incident records are **transformative, safety-oriented summaries**
derived from publicly available reporting and are intended for research,
education, and risk awareness. Where possible, records include a source
URL to support attribution and traceability.

If you believe a record improperly includes or misrepresents content,
contact CSF to request review and correction via the governance process
described in this specification.

## 2. System Overview

### 2.1 High-Level Pipeline Architecture

The CSF Crypto Incident Intelligence Pipeline is a **multi-stage,
artifact-driven system** that converts raw, publicly reported incident
signals into structured intelligence outputs.

At a high level, the pipeline operates as a **one-way flow**:

1.  Raw signals are collected and prepared by humans.

2.  Structured incident records are generated through deterministic
    stages.

3.  Weekly intelligence artifacts are produced and anchored by
    governance metadata.

4.  Canonical incident records are stored immutably for long-term
    reference.

The pipeline explicitly separates:

- **human judgment** (limited to sourcing and preparation), from

- **deterministic processing** (classification, analytics,
  normalization).

Once an incident enters the deterministic portion of the pipeline, all
downstream outputs are governed by strict invariants and immutability
rules.

The architecture is designed to support:

- incremental ingestion during the week,

- reproducible weekly aggregation,

- regeneration of weekly outputs without altering historical truth.

### 2.2 Planes, Phases, and Responsibilities

To clarify responsibilities and reduce ambiguity, the pipeline is
organized into **three planes**, each with distinct roles and
constraints.

**Collection Plane (Pre-Orchestrator)**

**Responsibility:**\
Human-driven sourcing, preparation, and identity assignment.

**Key characteristics:**

- Involves manual review and judgment.

- Determines *what enters* the pipeline, not *how it is classified*.

- Produces stable, globally unique incident identifiers.

**Outputs:**

- De-duplicated source links.

- Assigned unique incident IDs.

- Raw incident text ready for ingest.

This plane exists explicitly to prevent subjective interpretation from
leaking into structured intelligence stages.

**Intelligence Plane (Deterministic Processing)**

**Responsibility:**\
Convert prepared inputs into structured, analyzable incident
intelligence.

**Key characteristics:**

- Fully deterministic and stage-based.

- Each stage is executable in isolation.

- No stage may rely on implicit memory or downstream context.

- Incident classification becomes immutable at ingest.

**Core functions:**

- Atomic incident ingest (Stage 1)

- Dataset-level taxonomy analytics (Stage 2)

- Prevention action normalization (Stage 3)

All analytical insight is derived from structured records produced in
this plane.

**Governance Plane (Integrity and Trust)**

**Responsibility:**\
Ensure long-term trust, traceability, and auditability of outputs.

**Key characteristics:**

- Anchors weekly outputs with explicit metadata.

- Surfaces ambiguity and taxonomy pressure explicitly.

- Prevents silent changes to historical records.

**Outputs:**

- manifest.md

- governance notes

- integrity hashes

- canonical single-incident files

This plane ensures that the system remains credible as it scales across
time, contributors, and downstream uses.

A phase-by-phase orchestration index is provided in Appendix N for
navigational reference.

### 2.3 Artifact-First Design

The pipeline follows an **artifact-first design philosophy**.

Every meaningful action in the system produces a named, inspectable
artifact.\
No stage relies on transient state, hidden transformations, or implicit
context.

**Core principles of artifact-first design**

- **Explicit outputs:** Every stage produces clearly labeled files or
  datasets.

- **Immutability:** Once an artifact is published, it is never silently
  modified.

- **Reproducibility:** Weekly artifacts can be regenerated from
  canonical records.

- **Traceability:** Every weekly output can be traced back to specific
  incident IDs.

- **Audit readiness:** External reviewers can validate process integrity
  without access to internal tooling.

**Canonical vs. derived artifacts**

The system distinguishes between:

- **Canonical artifacts**\
  Atomic incident records stored under /incidents/.\
  These represent the system's source of truth.

- **Derived artifacts**\
  Weekly files under /weeks/YYYY/CWxx/.\
  These are snapshots, not authorities, and may be regenerated.

If a conflict exists between a canonical artifact and a derived
artifact, **the canonical artifact always takes precedence**.

This distinction is fundamental to the system's ability to evolve
without rewriting history.

**Why this matters**

An artifact-first architecture:

- prevents silent drift,

- enables external verification,

- supports automation without sacrificing trust,

- and aligns the pipeline with established practices in security
  reporting and incident response.

This design choice prioritizes **credibility and longevity** over
convenience.

## 3. Human Collection Plane (Pre-Orchestrator)

The Human Collection Plane defines all activities that occur **before**
an incident enters the deterministic intelligence pipeline.

This plane exists to handle tasks that inherently require human
judgment---such as sourcing, relevance filtering, and identity
assignment---while **explicitly constraining** that judgment to prevent
downstream ambiguity or silent bias.

Once an incident leaves this plane, **human interpretation is no longer
permitted**.

### 3.1 Rolling Link Collection

**Purpose**

Rolling link collection captures **potential incident signals** from
public sources on an ongoing basis.

This step is intentionally permissive: it favors inclusion over
precision and does not assume that every collected link will ultimately
become an incident record.

**Sources**

Typical sources include, but are not limited to:

- social media posts and threads

- forums and community discussions

- news articles and blog posts

- public disclosures and advisories

**Rules**

- Collected items MUST be stored as source URLs with a collection date.

- No incident interpretation, classification, or summarization occurs at
  this stage.

- Links MAY represent duplicates, follow-ups, or partial information.

- Collection cadence is flexible (daily or near-daily).

**Output Artifact**

A rolling link table containing, at minimum:

- collection date

- source URL

This artifact represents **uncommitted signals**, not incidents.

### 3.2 Duplicate Detection (Prompt 0)

**Purpose**

Duplicate detection identifies **URL-level duplicates** within a link
table prior to incident creation.

This step exists to reduce accidental double-processing while preserving
analyst discretion.

**Mechanism**

- Duplicate detection is performed using **PROMPT 0**.

- Only normalized source URLs are used for comparison.

- Incident text, titles, dates, or inferred similarity are explicitly
  excluded.

**Constraints**

- PROMPT 0 MUST be executed in isolation.

- PROMPT 0 MUST NOT recommend deletions or select a "primary" record.

- Duplicate detection is **informational only**.

**Human Responsibility**

- Humans decide how to handle reported duplicates.

- No automated deletion or consolidation is permitted at this stage.

**Output Artifact**

- DUPLICATE_REPORT\
  Stored verbatim and not interpreted by the orchestrator.

### [3.3 Unique Incident ID Generation]{.mark}

[**Purpose**\
This step assigns a globally stable, immutable identifier to each
incident that enters the intelligence pipeline.\
The incident ID is the system's primary identity anchor and persists
across:]{.mark}

- [weeks]{.mark}

- [reprocessing]{.mark}

- [reordering]{.mark}

- [downstream artifacts]{.mark}

[Once assigned, an incident ID permanently defines the identity of that
incident within the CSF system.]{.mark}

[**Method**\
Incident IDs are generated deterministically using a controlled identity
system defined in Appendix A.\
The system derives a stable identifier from invariant properties of the
source material, ensuring that:]{.mark}

- [the same incident always receives the same ID, and]{.mark}

- [different incidents never share an ID.]{.mark}

[The exact derivation method is a normative execution artifact and may
be access-controlled.\
This specification defines the **behavioral guarantees** of incident
identity, not the implementation details.]{.mark}

**[Rules]{.mark}**

- [IDs MUST be generated before any structured ingest occurs.]{.mark}

- [IDs MUST be frozen (copied as values) once assigned.]{.mark}

- [IDs MUST NOT be regenerated after publication.]{.mark}

- [IDs MUST be reused consistently across all artifacts and
  weeks.]{.mark}

[If an ID cannot be generated due to invalid or incomplete inputs, the
incident MAY still proceed through the pipeline, but the anomaly MUST be
surfaced explicitly downstream.]{.mark}

[**Output Artifact**\
A registry of incident IDs mapped to their corresponding source
references and first-observed context.]{.mark}

[This registry represents the **point of no return** for incident
identity: once an incident ID is assigned, the incident's identity is
fixed permanently.]{.mark}

### 3.4 Handoff into the Intelligence Plane

**Purpose**

This step marks the transition from **human judgment** to
**deterministic processing**.

From this point forward:

- interpretation is constrained by prompt rules,

- classification becomes immutable,

- and all outputs are governed by stage invariants.

**Required Inputs for Handoff**

Each incident handed into the Intelligence Plane MUST include:

- incident ID

- source URL

- raw incident text

No additional metadata is permitted unless explicitly required by a
downstream stage.

**Boundary Rule (Critical)**

Once an incident enters the Intelligence Plane:

- humans MUST NOT reinterpret or reclassify the incident,

- corrections MUST be handled via governance mechanisms,

- historical artifacts MUST NOT be silently altered.

This boundary is foundational to the credibility of the pipeline.

**Summary**

The Human Collection Plane:

- allows judgment where it is unavoidable,

- constrains that judgment to explicit steps,

- and produces stable artifacts that enable deterministic intelligence
  processing.

Its sole purpose is to prepare incidents for **trustworthy, repeatable
analysis**---not to interpret them.

## 4. Intelligence Plane --- Atomic Incident Ingest

The Atomic Incident Ingest is the **first deterministic stage** of the
Intelligence Plane and the point at which an incident becomes a
**canonical record** within the CSF system.

From this stage onward:

- incident identity is fixed,

- classification is immutable,

- and all downstream analysis is constrained to the structured output
  produced here.

This stage is intentionally strict. Its purpose is not to be flexible or
expressive, but to be **correct, reproducible, and audit-safe**.

### 4.2 Stage 1: Atomic Incident Ingest (Prompt 1)

**Purpose**

Stage 1 converts raw incident text into **one immutable, structured
incident record**.

This stage is the **single source of truth** for:

- incident classification,

- subtype assignment,

- summary framing,

- recorded user mistake,

- and prevention text.

No other stage may reinterpret or modify these fields.

**Mechanism**

- Stage 1 is executed using **PROMPT 1 --- INCIDENT TEXT → PSV ROW
  (PRIMARY INGEST)**.

- PROMPT 1 is a locked execution contract and MUST be run exactly as
  specified.

- Each execution produces **exactly one PSV row** per incident.

**Determinism and Isolation**

- PROMPT 1 MUST be executable in isolation.

- PROMPT 1 MUST rely only on the explicitly provided inputs.

- PROMPT 1 MUST NOT use memory of prior incidents or runs.

- Given identical inputs, PROMPT 1 MUST always produce identical output.

**Error and Ambiguity Handling**

- Missing, ambiguous, or malformed inputs do not halt ingest.

- Instead, uncertainty MUST be surfaced explicitly via
  classification_warning.

- Even in error conditions, exactly one PSV row MUST be produced.

This ensures that ingest never fails silently and that ambiguity is
preserved, not hidden.

**Output Artifact**

The output of Stage 1 is a **canonical incident record**, stored as a
PSV row and aggregated into INCIDENT_RECORDS.

This record becomes immutable once produced.

### 4.1 Raw Incident Text Capture

**Purpose**

Raw incident text capture preserves the **original, unstructured
description** of an incident exactly as reported by the source.

This step ensures that:

- no interpretation is introduced before ingest,

- downstream classification is grounded in observable claims,

- future reviewers can trace structured outputs back to original
  wording.

**Rules**

- Incident text MUST be captured verbatim from the source.

- No summarization, paraphrasing, or cleanup is permitted.

- Formatting artifacts (line breaks, emphasis, quoted replies) MAY be
  preserved.

- Non-textual content (images, videos) may be referenced descriptively
  but not interpreted.

Raw incident text is treated as **evidence**, not analysis.

**Output Artifact**

For each incident:

- incident ID

- source URL

- raw incident text

This artifact is a transient input into Stage 1 and is not itself a
structured record.

### 4.3 Canonical Incident Record Invariants

Canonical incident records produced by Stage 1 are governed by strict
invariants.

**Immutability**

- Canonical records MUST NOT be edited, rewritten, or reclassified after
  ingest.

- Corrections or reinterpretations require:

  - explicit governance action, or

  - creation of a new incident record.

Historical records are preserved even if later understanding evolves.

**Field Stability**

- Field order, meaning, and allowed values are locked by PROMPT 1.

- Taxonomy values are authoritative for the run in which they were
  generated.

- Downstream stages may analyze but never alter these fields.

**Identity Integrity**

- The incident ID is the primary identifier.

- Entry numbers used in later stages are run-scoped and
  non-authoritative.

- All weekly and governance artifacts must reference the canonical ID.

**Transparency of Uncertainty**

- Ambiguity is explicitly recorded, not resolved downstream.

- classification_warning is a first-class signal, not an error
  condition.

- Records with warnings remain valid and analyzable.

**Canonical vs. Derived Use**

Canonical incident records:

- serve as the system's source of truth,

- may be reused across weeks,

- may outlive any single weekly publication.

Derived artifacts must always defer to canonical records in the event of
conflict.

**Why this stage matters**

Stage 1 establishes the **epistemic boundary** of the entire system.

Once an incident is ingested:

- analysis may continue,

- patterns may be identified,

- prevention may be normalized,

but the original structured interpretation remains fixed.

This design choice prioritizes **credibility, auditability, and
long-term trust** over convenience or revisionism.

## 5. Intelligence Plane --- Weekly Aggregation

Weekly aggregation converts a set of immutable, canonical incident
records into **time-bounded editorial snapshots** suitable for analysis,
publication, and review.

This process is intentionally **mechanical and non-interpretive**.\
No new meaning is introduced, and no existing meaning is altered.

Weekly aggregation exists to answer one question only:

*"What incidents were curated during this week?"*

### 5.1 incidents.psv Generation

**Purpose**

incidents.psv is the **mechanical aggregation artifact** that combines
all canonical incident records selected for a given week.

It is the sole bridge between:

- atomic incident ingest (Stage 1), and

- weekly analytical outputs (Stages 2 and 3).

**Construction Rules**

- incidents.psv MUST be created by **concatenating Stage 1 PSV rows
  verbatim**.

- Records MUST appear in a deliberate, documented order.

- No headers are permitted.

- The pipe character (\|) MUST be used as the delimiter.

- UTF-8 encoding is required.

**Prohibited Actions**

During incidents.psv generation, the following are explicitly forbidden:

- editing or rewording any field

- reordering fields within a record

- normalizing dates, casing, or whitespace

- correcting perceived classification issues

- exporting via spreadsheet "Save As" workflows

incidents.psv is not a dataset to be "prepared"; it is a **verbatim
assembly**.

**Status**

incidents.psv is:

- not a source of truth,

- not intended for publication,

- a transient but critical aggregation artifact.

### 5.2 Safe Ingest into Excel (Power Query)

**Purpose**

Excel may be used for review and downstream file generation, but it
introduces risks---particularly **silent type coercion**, most notably
for dates.

This step defines the **only approved method** for ingesting
incidents.psv into Excel without mutating data.

**Approved Method**

- Ingest MUST be performed using **Power Query**.

- All columns MUST be explicitly forced to text.

- Headers MUST be applied manually, not inferred.

- No automatic type detection or transformation is permitted.

A single defensive operation is allowed:

- prefixing a leading space to date fields *inside Power Query only* to
  prevent Excel date coercion.

**Constraints**

- The prefixed space is a **display-layer safeguard**, not a data
  transformation.

- Prefixed dates MUST NOT be exported back into canonical or aggregated
  artifacts.

- Any Power Query step beyond the approved sequence invalidates the
  ingest.

The authoritative procedure is defined in **Appendix B**.

### 5.3 incidents.csv as a Weekly Snapshot

**Purpose**

incidents.csv is the **editorial snapshot** of all incidents curated
during a specific calendar week.

It is designed for:

- human review,

- downstream analytics,

- publication workflows,

- integrity anchoring.

**Nature of the File**

incidents.csv is a **derived artifact**.

It:

- may be regenerated at any time,

- does not define incident truth,

- must always defer to canonical incident records.

**Generation Rules**

- incidents.csv MUST be generated mechanically from incidents.psv.

- Allowed transformations are limited to:

  - delimiter replacement (\| → ,)

  - header insertion

- No semantic transformation is permitted.

**Authority Boundary**

If a discrepancy exists between:

- incidents.csv, and

- a canonical incident file under /incidents/

**the canonical incident file always takes precedence**.

**Role in the Pipeline**

incidents.csv answers:

*"What incidents are included in this week's bundle?"*

It does **not** answer:

- whether classifications are correct,

- whether prevention guidance is sufficient,

- whether incidents are related across weeks.

Those questions are handled by later analytical and governance stages.

Why this separation matters

By strictly separating:

- **immutable incident truth**, from

- **regenerable weekly snapshots**,

the pipeline enables:

- consistent weekly reporting,

- safe regeneration of historical outputs,

- long-term trust without silent revision.

Weekly aggregation is therefore a **publishing convenience**, not an
epistemic authority.

## 6. Intelligence Plane --- Dataset Analytics

Dataset analytics operate on **collections of immutable incident
records** to provide visibility into patterns, distributions, and
prevention relevance across a defined time window.

Crucially, these stages are **analytical only**.\
They do not create new facts, reinterpret incidents, or modify canonical
records.

Their role is to answer higher-order questions such as:

- *What kinds of failures are most common?*

- *Where is classification uncertain or under pressure?*

- *Which prevention actions appear most frequently across incidents?*

### 6.1 Stage 2: Taxonomy Analytics (Prompt 2)

**Purpose**

Stage 2 performs **taxonomy-level analysis and quality control** across
a dataset of incident records.

It is designed to:

- surface distribution patterns across incident types and subtypes,

- validate taxonomy integrity,

- expose ambiguity or classification pressure without resolving it.

**Inputs**

Stage 2 operates on a **restricted extract** of incident data,
including:

- entry number (run-scoped)

- incident type

- incident subtype

- classification warning

Raw incident text, summaries, and prevention guidance are explicitly
excluded.

**Mechanism**

- Stage 2 is executed using **PROMPT 2 --- INCIDENT DATASET → TAXONOMY
  ANALYTICS**.

- The taxonomy used is locked for the duration of the run.

- All categories are zero-filled to ensure full visibility.

**Guarantees**

- No incident is reclassified.

- Invalid or ambiguous values are reported, not corrected.

- Classification warnings are treated as first-class analytical signals.

- Entry numbers preserve traceability to the underlying dataset order.

**Output Artifact**

- taxonomy_report.md

This report provides:

- dataset scope,

- incident type distribution,

- full subtype tables,

- explicit disclosure of classification warnings,

- exactly three data-backed takeaways.

The report answers:

*"What kinds of incidents dominated this dataset, and where is
classification under strain?"*

### 6.2 Stage 3: Prevention Action Normalization (Prompt 3)

**Purpose**

Stage 3 analyzes **recorded prevention guidance** to understand how
frequently specific prevention actions appear across incidents.

It does **not** infer ideal prevention, best practices, or hypothetical
mitigations.

**Inputs**

Stage 3 operates on a structured subset of incident records, including:

- entry number

- incident type and subtype

- summary

- user mistake

- prevention text

- classification warning

The free-text prevention field remains the primary signal.

**Mechanism**

- Stage 3 is executed using **PROMPT 3 --- PREVENTION ACTION
  NORMALIZATION**.

- Mapping is restricted to a **locked prevention action set**.

- Identical prevention text must produce identical mappings.

**Constraints**

- Actions are mapped conservatively.

- Vague, missing, or narrative prevention text may result in no mapping.

- No new prevention actions may be invented or generalized.

**Output Artifact**

- prevention_report.md

This report includes:

- a zero-filled prevention action table,

- entry-number traceability,

- coverage percentages,

- explicit disclosure of unmappable or ambiguous prevention text.

The report answers:

*"Which prevention actions appear most often in recorded incident
guidance?"*

### 6.3 Interpretation Boundaries

Dataset analytics are subject to strict interpretation boundaries.

**What analytics may do**

- Count and distribute existing classifications.

- Surface ambiguity and taxonomy pressure.

- Quantify recorded prevention coverage.

- Support trend visibility across a defined dataset.

**What analytics must not do**

- Reclassify incidents.

- Correct or override Stage 1 outputs.

- Infer attacker behavior beyond recorded fields.

- Translate low coverage into low preventability.

- Generate new advice, guidance, or recommendations.

**Analytical humility (by design)**

Low prevalence of a category or prevention action may reflect:

- reporting bias,

- vague source material,

- conservative mapping rules,

- or intentional refusal to infer.

The system treats these outcomes as **signals**, not failures.

**Authority boundary**

If an analytical conclusion conflicts with:

- a canonical incident record, or

- an explicit classification warning,

the canonical record and warning take precedence.

Analytics explain the dataset; they do not redefine it.

### Why this separation matters

By separating:

- **incident truth creation** (Stage 1), from

- **dataset-level analysis** (Stages 2 and 3),

the pipeline ensures that insight can evolve **without rewriting
history**.

This preserves:

- reproducibility,

- auditability,

- and long-term trust in published intelligence.

## 7. Governance Plane --- Weekly Closure

The Governance Plane formalizes the **end-of-week closure** of a dataset
and establishes long-term trust in published outputs.

Its role is not analytical.\
Its role is to ensure that what was produced during the week can be:

- identified unambiguously,

- verified later,

- regenerated if needed,

- and audited without relying on institutional memory.

Weekly closure is therefore an **integrity operation**, not a content
operation.

### 7.1 manifest.md (Integrity Anchor)

**Purpose**

manifest.md is the **primary integrity anchor** for a weekly
intelligence bundle.

It defines *exactly* what constitutes the week's output and serves as
the entry point for:

- humans,

- automation,

- and future audits.

**Required Content**

The manifest MUST include:

- the calendar week identifier (e.g., CW02 2026),

- the total incident count,

- an ordered list of incident IDs included that week,

- a generation timestamp.

Optional but strongly recommended fields include:

- orchestrator version,

- integrity hash of incidents.csv.

**Authority**

The manifest:

- does not summarize incidents,

- does not restate analytics,

- does not interpret data.

It answers one question only:

*"What exact inputs and outputs define this week?"*

If a discrepancy exists between weekly artifacts, the manifest is the
**authoritative reference** for scope and inclusion.

### 7.2 taxonomy_report.md and prevention_report.md

**Purpose**

These reports represent the **analytical outputs** of the Intelligence
Plane, preserved as part of the weekly bundle.

They are governed artifacts, not working documents.

**Role in Governance**

Within the Governance Plane, these reports:

- freeze analytical results for the week,

- prevent silent regeneration with different inputs,

- enable comparison across weeks.

**Constraints**

Once published as part of a weekly bundle:

- reports MUST NOT be edited or regenerated silently,

- any correction requires an explicit new weekly bundle or governance
  note,

- historical reports remain immutable.

These reports provide analytical context but **do not override**
canonical incident records.

Documentation Integrity Note

Weekly governed Markdown files (including taxonomy_report.md and
prevention_report.md)

are generated from authoritative source documents using the procedure
described

in Appendix J.

To preserve reproducibility and auditability, these files are not
manually rewritten

during production. If discrepancies are identified after publication,
the Markdown

files are regenerated from the original source documents following the
same procedure.

### 7.3 governance_notes.md

Governance notes are generated solely from explicit, human-provided
inputs and MUST NOT depend on incident text, analytical outputs, or
prior weeks.

**Purpose**

governance_notes.md is a **lightweight governance signal**, not a
report.

It exists to capture:

- taxonomy pressure signals,

- recurring classification warnings,

- anomalies observed during the week,

- notes that may influence future taxonomy or guidance updates.

**Characteristics**

- Short and focused (typically a few lines).

- Optional in content but **required in presence** from its effective
  date onward.

- May reference governance documents, but does not introduce changes
  itself.

**Authority Boundary**

Governance notes:

- do not modify incidents,

- do not change taxonomy,

- do not retroactively affect analytics.

They function as a **forward-looking marker**, not a corrective
mechanism.

The input contract and determinism guarantees for governance_notes.md
are defined in Appendix M.

### 7.4 Single-Incident Canonical Storage

**Purpose**

Single-incident canonical storage preserves each incident as an
**independent, immutable artifact**.

This supports:

- atomic truth at the incident level,

- precise version control,

- long-term archival and reuse.

**Mechanism**

- Each incident included in the weekly bundle is written to its own
  file.

- Filenames are derived directly from the incident ID.

- File contents reflect the canonical structured record exactly.

**Rules**

- Canonical incident files MUST NOT be overwritten.

- One incident equals one file, forever.

- Weekly artifacts may be regenerated; canonical incident files may not.

**Relationship to Weekly Outputs**

Weekly bundles are snapshots.\
Canonical incident files are **the record**.

If a conflict arises:

- canonical incident files take precedence,

- weekly artifacts may be regenerated,

- history is not rewritten.

### Why weekly closure matters

Without formal weekly closure:

- outputs drift,

- trust erodes,

- audits become narrative-dependent.

The Governance Plane ensures that each week:

- has a clear boundary,

- leaves a verifiable footprint,

- and can be revisited years later without ambiguity.

This discipline is foundational to the system's credibility.

## 8. Output Contracts

Output contracts define **what artifacts are produced**, **in which
combinations**, and **in what order**, depending on how the pipeline is
executed.

They exist to ensure that:

- downstream users know exactly what to expect,

- automation can rely on stable interfaces,

- and partial executions do not create ambiguity.

The pipeline supports three execution modes:

- Rolling Ingest

- Weekly Close

- Full Pipeline

Each mode has a **strict, explicit output contract**.

### 8.1 Rolling Ingest Outputs

**Purpose**

Rolling ingest supports **incremental processing during the week**,
allowing incidents to be ingested and stored without triggering full
weekly analytics or governance closure.

This mode prioritizes **timeliness and atomic truth**, not completeness.

**When Used**

- During the week as new incidents are observed

- When only a subset of incidents is ready for ingest

- When analytics and weekly bundling are intentionally deferred

**Required Outputs**

Rolling ingest produces the following outputs, in this exact order:

1.  **DUPLICATE_REPORT**

    - Produced only if duplicate detection (Stage 0) is executed

    - Stored verbatim

    - Informational only

2.  **INCIDENT_RECORDS**

    - One PSV row per incident processed in the run

    - Canonical, immutable records

    - May represent a partial week

**Constraints**

- No aggregation across days is implied.

- No analytics or prevention normalization is performed.

- Outputs may be appended to future weekly bundles.

Rolling ingest answers:

*"What new canonical incidents were ingested?"*

### 8.2 Weekly Close Outputs

**Purpose**

Weekly close produces a **complete, governed intelligence bundle** for a
defined calendar week.

This mode freezes:

- scope,

- analytics,

- and governance metadata.

**When Used**

- At the end of the weekly curation period

- When all incidents for the week have been ingested

- When outputs are intended for publication or archival

**Required Outputs**

Weekly close produces the following outputs, in this exact order:

1.  **INCIDENT_RECORDS**

    - Ordered list of all canonical incident records included that week

2.  **TAXONOMY_REPORT**

    - Dataset-level taxonomy analytics

    - Generated via Stage 2

3.  **PREVENTION_REPORT**

    - Normalized prevention action analysis

    - Generated via Stage 3

4.  **manifest.md**

    - Integrity anchor defining the weekly bundle

5.  **governance_notes.md**

    - Lightweight governance signals and observations

Generated from a fixed qualitative input block; non-analytical and
non-authoritative.

**Constraints**

- Outputs are immutable once published.

- Corrections require a new weekly bundle or explicit governance action.

- Weekly close does not modify canonical incident records.

Weekly close answers:

*"What happened this week, how did it classify, and what governance
context applies?"*

### 8.3 Full Pipeline Outputs

**Purpose**

Full pipeline execution produces **all possible artifacts** in a single,
end-to-end run.

This mode is primarily used for:

- backfills,

- reprocessing historical data,

- validation of tooling,

- onboarding or demonstration environments.

**When Used**

- When both rolling ingest and weekly close are performed together

- When no prior artifacts are assumed to exist

**Required Outputs**

Full pipeline execution produces the following outputs, in this exact
order:

1.  **DUPLICATE_REPORT**

    - Result of duplicate detection on the provided link table

2.  **INCIDENT_RECORDS**

    - Canonical incident records generated during the run

3.  **TAXONOMY_REPORT**

    - Dataset-level taxonomy analytics

4.  **PREVENTION_REPORT**

    - Normalized prevention action analysis

5.  **manifest.md**

6.  **governance_notes.md**

7.  **Single-incident canonical files**

    - One file per incident, stored under /incidents/

**Constraints**

- All stage ordering rules apply.

- No stage may infer or reuse outputs from outside the run.

- Full pipeline execution does not override existing canonical incident
  files.

Full pipeline answers:

*"Given these inputs, what would the system have produced end-to-end?"*

### Output Ordering and Labeling Rules (Global)

Across all execution modes:

- Outputs MUST be clearly labeled.

- Output order MUST be preserved.

- Sections MUST NOT be merged.

- No summarization or editorialization is permitted within outputs.

- Stage outputs MUST be stored verbatim.

If an expected output is missing, the run is considered **incomplete**.

### Why explicit output contracts matter

Explicit output contracts:

- prevent ambiguity in partial runs,

- enable reliable automation,

- allow third parties to verify completeness,

- and eliminate "implicit behavior" assumptions.

They ensure that **what the pipeline does is always visible at the
boundary**, not hidden inside implementation details.

## 9. Integrity Guarantees

Integrity guarantees define the **core trust properties** of the CSF
Crypto Incident Intelligence Pipeline.

They ensure that:

- outputs cannot drift silently,

- results can be reproduced,

- and published intelligence remains auditable years after creation.

These guarantees are not aspirational.\
They are enforced through explicit rules, artifacts, and boundaries
defined throughout this specification.

### 9.1 Immutability Rules

**Canonical Immutability**

Canonical incident records produced during **Atomic Incident Ingest
(Stage 1)** are immutable.

This means:

- fields MUST NOT be edited after ingest,

- classifications MUST NOT be reinterpreted,

- summaries and prevention text MUST NOT be rewritten.

If new information emerges or an error is discovered:

- the original record remains unchanged,

- remediation occurs via governance action or creation of a new record.

Immutability preserves historical truth, even when understanding
evolves.

**Derived Artifact Immutability**

Once a weekly bundle is published:

- incidents.csv

- taxonomy_report.md

- prevention_report.md

- manifest.md

- governance_notes.md

must be treated as immutable for that week.

Corrections or changes require:

- a new weekly bundle, or

- explicit governance documentation explaining the deviation.

Silent regeneration or retroactive modification is prohibited.

**Scope Immutability**

The scope of a weekly bundle---defined by the incident IDs listed in
manifest.md---MUST NOT change after publication.

If an incident was omitted or mis-scoped:

- the correction applies to a future week,

- not by altering the historical manifest.

### 9.2 Determinism and Reproducibility

**Deterministic Execution**

All deterministic stages in the pipeline operate under the following
rule:

**Identical inputs MUST produce identical outputs.**

This applies to:

- Stage 0 (Duplicate Detection)

- Stage 1 (Atomic Incident Ingest)

- Stage 2 (Taxonomy Analytics)

- Stage 3 (Prevention Action Normalization)

No stage may rely on:

- hidden state,

- implicit memory,

- external context,

- or prior runs.

**Reproducibility Across Time**

Given:

- the same inputs,

- the same orchestrator version,

- the same prompt versions,

the pipeline MUST be able to reproduce:

- identical canonical incident records,

- identical analytical reports,

- identical weekly bundles.

Reproducibility is enforced by:

- locked prompts,

- explicit inputs,

- artifact-first design,

- versioned governance.

**Version Sensitivity**

Outputs are reproducible **within a version context**.

If:

- the orchestrator version changes, or

- taxonomy or prevention sets change,

then outputs may differ legitimately.

Such changes:

- MUST be versioned,

- MUST be documented,

- MUST NOT affect historical artifacts.

### 9.3 Hashing and Audit Anchors

**Purpose of Hashing**

Hashing provides **tamper-evidence**, not semantic meaning.

Hashes allow future reviewers to answer:

*"Is this file exactly the same as the one originally published?"*

They do not:

- validate correctness,

- imply authenticity of source claims,

- or replace incident IDs.

**incidents.csv Integrity Hash**

For each weekly bundle, an integrity hash MAY be generated for
incidents.csv.

Rules:

- The hash algorithm is SHA-256.

- The hash is computed on the final, published file.

- No normalization of line endings, encoding, or delimiters is
  permitted.

The hash, if generated:

- MUST be recorded verbatim in manifest.md,

- MUST NOT be recalculated after publication.

The authoritative procedure is defined in **Appendix C**.

**Audit Anchors**

The following artifacts collectively form the audit surface of the
system:

- incident IDs

- canonical incident files

- weekly manifest.md

- optional integrity hashes

- governance notes

- orchestrator version declarations

An external reviewer with access to these artifacts can:

- reconstruct what was known at the time,

- verify scope and integrity,

- identify where ambiguity was explicitly surfaced.

No internal tooling or institutional memory is required.

**Why integrity guarantees matter**

Without explicit integrity guarantees:

- datasets drift,

- trust erodes,

- and historical claims become unverifiable.

By enforcing immutability, determinism, and audit anchoring, the
pipeline ensures that its intelligence outputs can be **trusted, reused,
and scrutinized** over the long term.

This is foundational to the system's purpose.

## 10. Known Trade-offs and Design Constraints

The CSF Crypto Incident Intelligence Pipeline makes **deliberate
trade-offs** to preserve integrity, reproducibility, and long-term
trust.

This section documents constraints that may appear limiting to some
users, but which are **intentional and non-accidental**.\
They define the boundaries within which the system remains reliable.

### 10.1 Duplicate Semantics

**Constraint**

Duplicate detection is limited to **URL-level equivalence** after
normalization.

The system does **not** attempt to detect duplicates based on:

- semantic similarity,

- shared narratives,

- matching attacker behavior,

- or overlapping victim descriptions.

**Implication**

The same real-world incident may appear as multiple canonical records if
it is reported across:

- different platforms,

- different URLs,

- or follow-up posts.

**Rationale**

Semantic duplicate detection introduces:

- subjective interpretation,

- hidden heuristics,

- non-deterministic behavior.

By restricting duplicate semantics to normalized URLs, the pipeline
ensures:

- deterministic results,

- reproducible decisions,

- transparent boundaries.

Duplicate handling beyond URL equivalence is deferred to **human
judgment or downstream analysis**, not embedded into the core pipeline.

### 10.2 Cross-Week Identity Resolution

**Constraint**

The pipeline does not assign a shared identity to incidents reported
across different weeks.

Each canonical incident record is:

- scoped to its original ingest,

- immutable once created,

- independent of later reports or follow-ups.

**Implication**

Ongoing scams, long-running campaigns, or repeated reports may be
represented as:

- multiple incident records across weeks,

- without an explicit linkage mechanism.

This may inflate apparent incident counts when viewed longitudinally.

**Rationale**

Cross-week identity resolution requires:

- retrospective judgment,

- reinterpretation of historical records,

- or mutable incident state.

The pipeline prioritizes **atomic truth at the time of observation**
over retrospective consolidation.

Longitudinal linkage is considered an **external analytical concern**,
not a core pipeline responsibility.

### 10.3 Incident Lifecycle Limitations

**Constraint**

Canonical incident records do not include lifecycle states such as:

- resolved,

- ongoing,

- recovered,

- mitigated,

- or attributed.

Once ingested, an incident remains in its original state indefinitely.

**Implication**

The system does not track:

- follow-up developments,

- law enforcement action,

- asset recovery,

- or post-incident remediation.

Such updates must be represented as **new incident records or external
commentary**, not as modifications to existing records.

**Rationale**

Lifecycle tracking conflicts with immutability and introduces:

- ambiguous state transitions,

- retroactive reinterpretation,

- silent record drift.

The pipeline treats incident records as **snapshots of reported
reality**, not evolving case files.

### 10.4 Prevention Coverage Interpretation

**Constraint**

Prevention analysis reflects **only what is explicitly recorded** in
incident prevention fields.

The system does not:

- infer ideal prevention,

- generalize best practices,

- or translate narrative warnings into actions.

**Implication**

Prevention coverage may appear low due to:

- missing prevention text,

- vague or narrative guidance,

- conservative refusal to map ambiguous actions.

Low coverage does **not** imply low preventability.

**Rationale**

Inferring prevention beyond recorded text introduces:

- speculative guidance,

- inconsistent mappings,

- hindsight bias.

By constraining prevention analysis to explicit, mappable actions, the
pipeline preserves analytical honesty and comparability across weeks.

### Design Philosophy Summary

These constraints reflect a consistent philosophy:

- prefer **explicit signals** over inferred meaning,

- preserve **historical truth** over convenience,

- surface **ambiguity** rather than resolve it silently,

- separate **collection, analysis, and interpretation** concerns.

The result is a system that may feel conservative, but which remains
**trustworthy under scrutiny**.

## 11. Versioning and Change Control

Versioning and change control define how the CSF Crypto Incident
Intelligence Pipeline evolves over time without compromising
reproducibility, auditability, or historical integrity.

This section establishes:

- how versions are assigned,

- what constitutes a breaking change,

- how compatibility is preserved,

- and how changes become effective.

No change to this system is considered valid unless it complies with the
rules defined here.

### 11.1 Semantic Versioning Rules

The orchestrator specification follows **semantic versioning** in the
form:

**MAJOR.MINOR**

Examples:

- v1.0

- v1.1

- v2.0

**MAJOR version changes (breaking)**

A MAJOR version increment indicates a **breaking change** to the
pipeline contract.

Breaking changes include, but are not limited to:

- reordering or redefining pipeline stages,

- changing required inputs or outputs of any stage,

- modifying canonical field definitions or order,

- altering incident ID semantics,

- changing taxonomy structure or allowed values,

- changing the locked prevention action set,

- relaxing or tightening immutability guarantees.

MAJOR version changes invalidate direct comparability with artifacts
produced under earlier major versions.

### **MINOR version changes (non-breaking)**

A MINOR version increment indicates a **non-breaking clarification or
hardening**.

Non-breaking changes may include:

- stronger wording of existing invariants,

- additional validation or QC checks that do not alter outputs,

- documentation clarifications,

- added examples or appendices,

- tooling guidance that preserves existing behavior.

MINOR changes MUST NOT:

- alter canonical incident records,

- change analytical results for identical inputs,

- invalidate previously published artifacts.

### 11.2 Compatibility Contract

Each MAJOR version defines a **stable execution contract**.

Within a MAJOR version:

- stage boundaries are fixed,

- prompt behavior is fixed,

- artifact semantics are fixed,

- immutability guarantees are fixed.

Artifacts produced under a given MAJOR version:

- remain valid indefinitely,

- MUST NOT be retroactively modified to match newer versions,

- MUST retain their original meaning within their version context.

**Cross-version comparison**

Comparisons across different MAJOR versions:

- may be informative,

- but MUST be explicitly labeled as cross-version,

- MUST NOT assume direct equivalence.

Automation, dashboards, or publications that consume pipeline outputs
are expected to:

- detect orchestrator versions,

- handle version differences explicitly.

### 11.3 Change Log Requirements

No change to this specification may be introduced silently.

**Required documentation**

All changes MUST be recorded in an explicit change log entry that
includes:

- version number,

- change classification (MAJOR or MINOR),

- description of what changed,

- rationale for the change,

- impact on existing workflows or outputs.

**Location**

Recommended locations:

- taxonomy-related changes → governance/taxonomy_change_log.md

- orchestrator or pipeline changes →
  governance/orchestrator_change_log.md

Historical entries MUST NOT be altered.

**Approval rules (lightweight governance)**

- MINOR changes require at least one maintainer approval.

- MAJOR changes require:

  - a written rationale,

  - an explicit migration note,

  - clear identification of incompatible outputs.

Governance exists to prevent **quiet drift**, not to slow iteration.

------------------------------------------------------------------------

### 11.4 Effective Dates

Every version change MUST declare an **effective date** in ISO 8601
format (YYYY-MM-DD).

**Rules**

- Changes apply only to pipeline runs generated on or after the
  effective date.

- Historical artifacts retain the rules and semantics of the version
  under which they were created.

- Effective dates MUST be documented alongside version entries in the
  change log.

**Manifest linkage (recommended)**

Weekly manifests SHOULD record:

- the orchestrator version used for that run.

This allows future reviewers to:

- understand which rules applied,

- reproduce results accurately,

- and interpret outputs correctly.

### Why versioning discipline matters

Without strict versioning and change control:

- outputs lose comparability,

- trust erodes,

- and historical intelligence becomes ambiguous.

By enforcing explicit version boundaries, documented changes, and
effective dates, the pipeline ensures that evolution is **transparent,
controlled, and auditable**.

This is essential for long-term credibility.

## 12. Appendices

**Appendix Authority and Precedence**

Appendices in this specification serve distinct roles.

Appendices **A--E** define supporting systems, tooling procedures, and
operational workflows that implement the pipeline described in the main
body.

Appendices **F--I** contain **authoritative, executable prompt
contracts** used to operate the Intelligence Pipeline.

**Authority Rules**

1.  **Prompts in Appendices F--I are normative.**\
    They define the exact execution behavior of pipeline stages.

2.  **In the event of a conflict**, the following precedence applies:

    1.  Appendix prompt text (F--I)

    2.  Main specification body

    3.  Supporting appendices and examples

3.  Narrative descriptions in the main body **explain intent** but do
    not override prompt behavior.

4.  Prompt text MUST be executed exactly as specified.\
    No interpretation, enrichment, or deviation is permitted unless
    explicitly versioned and documented.

**Versioning and Stability**

- Prompt text is version-bound to the orchestrator version under which
  it is published.

- Changes to prompt behavior are governed by the same **semantic
  versioning rules** defined in Section 11.

- Historical prompt text MUST remain accessible and immutable for runs
  generated under earlier versions.

**Design Intent**

This separation ensures that:

- the main specification remains readable and stable,

- execution behavior remains explicit and auditable,

- and implementation details can evolve without silently changing
  historical outcomes.

This structure mirrors established practices in:

- technical standards,

- security frameworks,

- and regulated reporting systems.

## Appendix A --- Unique Incident ID System

**Status:** FINAL / PRODUCTION\
**Scope:** Crypto Incident Intelligence Pipeline\
**Audience:** Analyst, Researcher, Incident Ingest\
**Applies To:** All runs under Orchestrator Spec v1.0+

### A.1 Purpose

This appendix defines the **authoritative method** for generating
**globally stable, collision-resistant Unique Incident IDs** for crypto
scam and security incidents.

The Unique Incident ID is the **primary identity anchor** of the entire
pipeline.

The system guarantees:

- The same incident always produces the same ID

- Different incidents never share an ID

- IDs remain stable across weeks, batches, re-ingests, and reordering

- IDs can be generated reliably inside Excel without external
  dependencies

Once generated and published, an incident ID is **immutable**.

### A.2 Design Rationale

**A.2.1 What This System Explicitly Does *Not* Use**

The following approaches are **intentionally forbidden**:

- Row numbers

- Entry numbers

- Sequential counters (e.g., YYYYMMDD-001)

- Excel row order

- Ingest or processing order

These methods fail under common operational conditions, including:

- Row insertion or deletion

- Sorting or filtering

- Historical backfills

- Reprocessing of previously seen sources

Any identity system dependent on ordering is inherently unstable.

**A.2.2 What This System Uses Instead**

The Unique Incident ID is derived from **three invariant properties**:

1.  **First Observed Date**\
    Provides temporal context without implying lifecycle state.

2.  **Normalized Source URL**\
    Serves as the stable identity anchor for the observed report.

3.  **Cryptographic Hash**\
    Ensures collision resistance and immutability.

This combination yields a deterministic, reproducible identifier that
survives all normal editorial and operational workflows.

### A.3 ID Format (LOCKED)

The canonical format is:

INC-YYYYMMDD-hhhhhhhhhh

Where:

- YYYYMMDD = first observed date (ISO 8601, compact form)

- hhhhhhhhhh = first 10 hexadecimal characters of\
  SHA-256(normalized_source_url)

**Example:**

INC-20260104-c469c7d486

This format is **version-stable** and MUST NOT be altered within a major
orchestrator version.

### A.4 Required Input Columns (Excel)

At minimum, the source table MUST contain:

  -----------------------------------------------
  **Column Name**  **Description**
  ---------------- ------------------------------
  First Observed   Excel date or ISO text
  Date             (YYYY-MM-DD)

  Source Link      Canonical source URL
  -----------------------------------------------

Optional but recommended:

- Entry Number (for human reference only; never used for identity)

### A.5 URL Normalization Rules (MANDATORY)

[Before incident ID generation, the source URL is normalized using a
**locked, deterministic normalization procedure**.]{.mark}

**[Purpose]{.mark}**

[URL normalization ensures that:]{.mark}

- [semantically identical source links produce the same incident
  ID,]{.mark}

- [incidental formatting differences do not affect identity,]{.mark}

- [IDs remain stable across tools, reprocessing, and time.]{.mark}

**[Public Contract]{.mark}**

[The normalization procedure:]{.mark}

- [is **order-sensitive** and **deterministic**,]{.mark}

- [operates only on the source URL,]{.mark}

- [produces a single canonical string used for hashing,]{.mark}

- [is identical for all runs within a major orchestrator
  version.]{.mark}

[Normalization explicitly **does not**:]{.mark}

- [infer semantic equivalence across different URLs,]{.mark}

- [merge related but distinct reports,]{.mark}

- [rely on content, titles, or metadata.]{.mark}

**[Authority and Control]{.mark}**

[The **authoritative normalization rules** are defined in the controlled
execution implementation referenced by this specification.]{.mark}

[Implementations:]{.mark}

- [MUST NOT invent, extend, reorder, or partially apply normalization
  rules,]{.mark}

- [MUST treat normalization as a **black-box contract** unless
  explicitly authorized.]{.mark}

[Any change to normalization logic:]{.mark}

- [REQUIRES a MAJOR orchestrator version change,]{.mark}

- [MUST NOT be applied retroactively to existing incident IDs.]{.mark}

### [A.6 Incident ID Generation --- Implementation Authority]{.mark}

**[Public Guarantee]{.mark}**

[Incident IDs are generated by applying a cryptographic hash to the
normalized source URL and combining it with the first observed date,
producing a deterministic, collision-resistant identifier.]{.mark}

[Within a given orchestrator version:]{.mark}

- [identical inputs ALWAYS produce identical IDs,]{.mark}

- [different inputs NEVER intentionally collide,]{.mark}

- [generation is stable across batches, weeks, and reprocessing.]{.mark}

**[Execution Boundary]{.mark}**

[The **exact executable implementation** used to generate incident
IDs:]{.mark}

- [is a **normative execution artifact**,]{.mark}

- [may be access-controlled,]{.mark}

- [is not required to be publicly distributed.]{.mark}

[This separation is intentional.]{.mark}

[The public specification defines:]{.mark}

- [**what** properties the ID system guarantees,]{.mark}

- [**when** IDs are generated,]{.mark}

- [**how** IDs may and may not be used downstream.]{.mark}

[The private implementation defines:]{.mark}

- [**how** those guarantees are mechanically enforced.]{.mark}

**[Auditability]{.mark}**

[Even without access to the implementation:]{.mark}

- [incident IDs remain externally verifiable,]{.mark}

- [downstream artifacts remain auditable,]{.mark}

- [identity stability can be validated empirically.]{.mark}

[Trust is established through **immutability and reproducibility**, not
through disclosure of executable code.]{.mark}

### [A.7 Incident ID Usage and Freezing Rules]{.mark}

**[Usage Pattern]{.mark}**

[Incident IDs are generated during the Human Collection Plane,
**before** any structured ingest occurs.]{.mark}

[Once generated:]{.mark}

- [IDs MUST be treated as immutable values,]{.mark}

- [IDs MUST be reused verbatim across all downstream artifacts,]{.mark}

- [IDs MUST serve as the primary reference key.]{.mark}

**[Freezing Requirement]{.mark}**

[After validation, incident IDs:]{.mark}

- [MUST be frozen (copied as values),]{.mark}

- [MUST NOT be recalculated,]{.mark}

- [MUST NOT be regenerated for published incidents.]{.mark}

[Any workflow that allows IDs to change due to:]{.mark}

- [sorting,]{.mark}

- [filtering,]{.mark}

- [recalculation,]{.mark}

- [or re-execution]{.mark}

[is considered invalid.]{.mark}

**[Failure Handling]{.mark}**

[If an incident ID cannot be generated due to invalid or missing
inputs:]{.mark}

- [the anomaly MUST be surfaced downstream,]{.mark}

- [the incident MAY proceed with an explicit warning,]{.mark}

- [identity MUST NOT be silently substituted.]{.mark}

**[Non-Negotiable Rule]{.mark}**

[Once an incident ID has been published, it is permanent.]{.mark}

[If identity logic ever changes:]{.mark}

- [the orchestrator version MUST change,]{.mark}

- [new incidents use the new logic,]{.mark}

- [historical IDs remain untouched.]{.mark}

### A.8 Validation Checks (MANDATORY)

Before finalizing any batch:

- Same URL + same date → same ID

- Same URL + different date → different ID

- Different URL + same date → different ID

- Sorting or filtering rows → IDs unchanged

Any violation indicates a pipeline error.

### A.9 Downstream Use

The Unique Incident ID MUST be reused consistently as:

- Canonical incident filename

- PSV / CSV primary key

- Cross-dataset reference ID

- De-duplication anchor

- Audit and governance reference

No alternative identifiers are permitted to replace it.

### A.10 Final Rule (NON-NEGOTIABLE)

**Never regenerate or modify incident IDs once published.**

If identity logic ever changes:

- version the orchestrator,

- version the pipeline,

- **do not retroactively alter IDs**.

This appendix defines the **canonical identity layer** of the Crypto
Incident Intelligence Pipeline.

## Appendix B --- incidents.psv Generation & Safe Ingest

**Status:** FINAL / PRODUCTION\
**Scope:** Weekly Production Tooling\
**Audience:** Analyst, Editor\
**Applies To:** Weekly aggregation and review workflows under
Orchestrator Spec v1.0+\
**Environment:** Excel (Windows) + Power Query

### B.1 Purpose

This appendix defines the **only approved method** for:

1.  generating incidents.psv from canonical Stage 1 incident records,
    and

2.  ingesting incidents.psv into Excel **without mutating data**.

This appendix exists to enforce a global invariant:

Canonical incident records must remain **verbatim** from Stage 1.\
Spreadsheet tooling must not silently coerce dates or types.

### B.2 Role of incidents.psv

incidents.psv is a **mechanical aggregation artifact**. It is:

- derived from canonical Stage 1 outputs,

- used as a bridge into weekly workflows (incidents.csv, analytics
  inputs, review),

- **not** a source of truth.

**Canonical vs. Derived**

- **Canonical truth:** Stage 1 PSV rows (and canonical per-incident
  files derived from them)

- **Derived weekly view:** incidents.psv and subsequent weekly artifacts

If a conflict exists, canonical records always take precedence.

### B.3 incidents.psv Generation (MANDATORY)

**B.3.1 Input Requirements**

The input to incidents.psv generation MUST be:

- a set of Stage 1 PSV rows,

- stored verbatim (no edits, no cleanup),

- in the exact Stage 1 field order and delimiter format.

**B.3.2 Construction Rules (NON-NEGOTIABLE)**

incidents.psv MUST be created by:

1.  concatenating Stage 1 PSV rows **verbatim**

2.  using \| (pipe) as the delimiter

3.  writing **no header row**

4.  writing **UTF-8 encoding**

5.  performing **no transformation** of any kind, including:

    - dates

    - whitespace

    - casing

    - punctuation

    - field content

    - field order

**B.3.3 Forbidden Creation Methods**

The following are explicitly forbidden due to silent mutation risk:

- Excel "Save As" workflows

- CSV export with auto-typing

- locale-aware date normalization

- reformatting or trimming fields

- column reordering or "cleanup" steps

If any transformation occurs, the resulting incidents.psv is invalid and
MUST be regenerated.

### B.4 Safe Ingest into Excel (Power Query)

**B.4.1 Why Power Query Is Required**

Excel frequently applies silent type coercion, especially:

- converting YYYY-MM-DD strings into locale-formatted dates,

- stripping leading zeros,

- auto-parsing numeric-like text.

To prevent this, ingestion MUST occur via Power Query with explicit
constraints.

**B.4.2 Approved Ingest Requirements (NON-NEGOTIABLE)**

When loading incidents.psv into Excel:

- Power Query MUST NOT infer column types

- Power Query MUST NOT promote headers

- All columns MUST be explicitly forced to **Text**

- No parsing, splitting, or type casting is allowed beyond delimiter
  parsing

- A single defensive step is permitted:

  - prefixing a leading space to first_observed_date **inside Power
    Query only** to prevent Excel date coercion

**Important boundary rule:**\
The leading-space prefix is a **display-layer safeguard only**. It MUST
NOT be exported back into canonical PSV rows or treated as canonical
data.

### [B.5 Safe Ingest Procedure --- Execution Authority (PUBLIC)]{.mark}

**[Purpose]{.mark}**

[This section defines the **authoritative behavioral requirements** for
safely ingesting incidents.psv into spreadsheet tooling without mutating
canonical incident data.]{.mark}

[The objective of safe ingest is:]{.mark}

- [to prevent silent type coercion,]{.mark}

- [to preserve canonical field values exactly as produced by Stage
  1,]{.mark}

- [to ensure downstream weekly artifacts remain reproducible and
  auditable.]{.mark}

**[Execution Boundary]{.mark}**

[The **exact executable implementation** used for safe ingest (including
Power Query definitions, column mappings, and defensive transformations)
is a **controlled execution artifact**.]{.mark}

[It:]{.mark}

- [is normative for CSF weekly production,]{.mark}

- [may be access-controlled,]{.mark}

- [is not required to be publicly distributed.]{.mark}

[This separation is intentional.]{.mark}

[The public specification defines **what properties the ingest process
MUST satisfy**.\
The private implementation defines **how those properties are
mechanically enforced**.]{.mark}

**[Mandatory Behavioral Requirements]{.mark}**

[Any workflow used to ingest incidents.psv into Excel or equivalent
tooling MUST satisfy **all** of the following conditions:]{.mark}

1.  [**No type inference**\
    All fields MUST be treated as text at ingest.\
    Automatic type detection or coercion is prohibited.]{.mark}

2.  [**No implicit header promotion**\
    Column headers MUST be applied explicitly and manually.\
    Headers MUST NOT be inferred from file contents.]{.mark}

3.  [**Delimiter-only parsing**\
    Parsing MUST be limited to delimiter separation (\|).\
    No additional parsing, splitting, or normalization is
    permitted.]{.mark}

4.  [**Date coercion defense**\
    The workflow MUST include an explicit safeguard to prevent
    spreadsheet software from coercing date-like text into native date
    types.]{.mark}

5.  [**No semantic transformation**\
    Field values MUST NOT be trimmed, reformatted, normalized, or
    reordered.]{.mark}

6.  [**No round-trip contamination**\
    Any display-layer safeguards applied during ingest MUST NOT be
    exported back into canonical or aggregated artifacts.]{.mark}

**[Validation Requirement]{.mark}**

[A safe ingest is considered valid **only if** all validation checks
defined in Section B.7 are satisfied.]{.mark}

[If any requirement is violated:]{.mark}

- [the ingest is invalid,]{.mark}

- [the resulting file MUST be discarded,]{.mark}

- [the process MUST be rerun using a compliant workflow.]{.mark}

**[Authority]{.mark}**

[This section defines the **minimum contract** for safe ingest
behavior.]{.mark}

[Any implementation that satisfies these requirements is acceptable.\
Any implementation that violates them is non-compliant, regardless of
tooling or intent.]{.mark}

### B.6 Forbidden Power Query Actions (NON-NEGOTIABLE)

Do NOT:

- use "Use First Row as Headers"

- allow an auto-generated "Changed Type" step

- parse or convert date fields

- apply locale transforms

- reorder columns

- trim, clean, or normalize text

If any forbidden step exists:

- the query is invalid,

- the file MUST be discarded and reloaded using the canonical method.

### B.7 Validation Check (MANDATORY)

After ingest:

- first_observed_date column type indicator MUST be **ABC (Text)**

- values must display as YYYY-MM-DD (optionally with a leading space in
  cells)

- Applied Steps MUST contain only:

  1.  Source

  2.  Force Text

  3.  Rename Columns

  4.  Prefix Date With Space

If these conditions are not met, the ingest is invalid.

### B.8 Versioning Note

Appendix B is tooling-only and does not alter Stage 0--3 behavior.

Changes to Appendix B may be treated as **MINOR** updates provided they
do not:

- change canonical record content,

- change field definitions,

- alter stage outputs.

## Appendix C --- incidents.csv Integrity Hashing

**Status:** FINAL / PRODUCTION\
**Scope:** Weekly Production Integrity\
**Audience:** Analyst, Editor, Automation\
**Applies To:** Weekly folders under weeks/YYYY/CWxx/\
**Effective From:** CW01 2026\
**Environment:** Windows (PowerShell)

### C.1 Purpose

This appendix defines the **authoritative method** for generating an
integrity hash for incidents.csv.

The integrity hash provides:

- tamper-evidence for published weekly artifacts,

- a stable audit anchor recorded in manifest.md,

- reproducible verification across time and environments.

This appendix answers one question only:

"Is this **exactly** the same incidents.csv file that was published that
week?"

### C.2 Role of the incidents.csv Hash

The incidents.csv hash is a **file-level integrity guarantee only**.

It:

- confirms byte-level identity of the published file,

- enables later verification without re-running the pipeline,

- supports audits, reviews, and downstream trust.

It does **not**:

- define incident identity,

- replace incident IDs,

- imply semantic meaning,

- validate correctness of classifications or content.

If the hash differs, the file has changed.\
No further inference is permitted.

### C.3 Hash Algorithm (LOCKED)

The canonical hashing algorithm is:

- **SHA-256**

- applied to the finalized incidents.csv file

- with **no normalization** of:

  - line endings

  - encoding

  - delimiters

  - whitespace

⚠️ Any change to the file --- even invisible formatting --- produces a
different hash.

### [C.4 Integrity Hash Generation --- Execution Contract (PUBLIC)]{.mark}

**[Purpose]{.mark}**

[This section defines the **authoritative behavioral contract** for
generating the integrity hash of incidents.csv used in weekly
bundles.]{.mark}

[The goal of hash generation is **tamper-evidence**, not
interpretation.]{.mark}

**[Execution Boundary]{.mark}**

[The **exact tooling and commands** used to generate the integrity hash
are **implementation details** and may be access-controlled.]{.mark}

[The public specification defines:]{.mark}

- [**what** file is hashed,]{.mark}

- [**when** hashing occurs,]{.mark}

- [**how** the hash must be interpreted.]{.mark}

[The private execution documentation defines:]{.mark}

- [**which tools** are used,]{.mark}

- [**how commands are invoked**,]{.mark}

- [**how environments are configured**.]{.mark}

[This separation is intentional and preserves long-term reproducibility
without exposing operational workflows.]{.mark}

**[Mandatory Hashing Requirements]{.mark}**

[Any compliant hash generation workflow MUST satisfy **all** of the
following conditions:]{.mark}

1.  [**Finalized input**\
    The hash MUST be generated on the **final, published version** of
    incidents.csv.]{.mark}

2.  [**Byte-level hashing**\
    Hashing MUST operate on the raw file bytes.\
    No normalization of:]{.mark}

    - [line endings,]{.mark}

    - [encoding,]{.mark}

    - [delimiters,]{.mark}

    - [whitespace\
      is permitted.]{.mark}

3.  [**Algorithm constraint**\
    The hash algorithm MUST be **SHA-256**.]{.mark}

4.  [**Ordering constraint**\
    Hash generation MUST occur **after** file finalization and
    **before** publication.]{.mark}

5.  [**Single-pass generation**\
    The hash MUST be generated exactly once per weekly bundle and MUST
    NOT be recalculated after publication.]{.mark}

6.  [**No post-hash mutation**\
    After hashing:]{.mark}

    - [the file MUST NOT be opened,]{.mark}

    - [MUST NOT be re-saved,]{.mark}

    - [MUST NOT be processed further.]{.mark}

[Any mutation after hashing invalidates the integrity guarantee.]{.mark}

**[Recording Requirement]{.mark}**

[The resulting hash:]{.mark}

- [MUST be recorded verbatim in manifest.md,]{.mark}

- [MUST NOT be altered, reformatted, or normalized,]{.mark}

- [MUST be treated as immutable once published.]{.mark}

**[Compliance Statement]{.mark}**

[Any implementation that satisfies the requirements above is considered
**compliant**, regardless of operating system or tooling.]{.mark}

[Any implementation that violates these requirements is
**non-compliant**, even if the resulting hash value appears
correct.]{.mark}

**[Interpretation Boundary]{.mark}**

[The integrity hash answers **one question only**:]{.mark}

*["Is this byte-for-byte the same file that was published that
week?"]{.mark}*

[No additional inference is permitted]{.mark}.

### C.5 Manifest Integration

The hash MUST be recorded verbatim in manifest.md:

incidents_csv_hash:
3f9c1e6a9a0d6d3b7c4a9c8e1f4e2b6c9d0f1a2b3c4d5e6f7a8b9c0d1e2f3

This field is:

- optional but **strongly recommended**

- immutable once published

- never recalculated retroactively

### C.6 Forbidden Practices (NON-NEGOTIABLE)

Do NOT:

- hash incidents.psv

- hash individual incident files

- re-hash after publication

- open or save incidents.csv in Excel before hashing

- normalize encoding or line endings

- include filename, algorithm, or metadata in the manifest

- substitute other hash algorithms

Any violation invalidates the integrity guarantee.

### C.7 Verification Procedure (Post-Publication)

To verify integrity at any later time:

1.  Re-run the same PowerShell command on incidents.csv

2.  Compare the output hash to manifest.md

Results:

- **Match** → file unchanged

- **Mismatch** → file modified

No interpretation beyond this comparison is allowed.

### C.8 Governance Note

Appendix C:

- introduces no behavioral change

- does not affect pipeline stages

- does not alter incident identity or classification

- applies only to weekly artifact integrity

This appendix is compatible with **Orchestrator Spec v1.0** and
qualifies as a **MINOR documentation hardening** if revised.

## Appendix D --- manifest.md Input Contract

**Status:** FINAL / PRODUCTION\
**Scope:** Weekly Production Metadata\
**Audience:** Analyst, Editor, Automation\
**Applies To:** All weekly folders under weeks/YYYY/CWxx/\
**Effective From:** CW01 2026\
**Breaking Change:** No (formalization only)

### D.1 Purpose

This appendix defines the **strict input contract** required to generate
a valid manifest.md.

The manifest is a **metadata anchor**, not an analytical artifact.\
It must be reproducible, auditable, and free of inference.

This appendix answers one question only:

"What exact inputs are required to generate a valid weekly manifest?"

### D.2 Role of manifest.md

manifest.md serves as:

- the entry point to a weekly folder,

- a human- and machine-readable integrity anchor,

- a stable reference for audits, automation, and review.

It does **not**:

- summarize incidents,

- restate taxonomy or prevention results,

- interpret or analyze data,

- derive values from other artifacts.

All values in manifest.md are **explicit inputs**, never inferred.

### D.3 Required Inputs (NON-NEGOTIABLE)

To generate manifest.md, the following inputs MUST be provided
explicitly.

**D.3.1 Week Identifier**

- Format: CWxx YYYY

- Example:

- CW02 2026

This identifier defines the scope of the weekly bundle.

**D.3.2 Ordered Incident ID List**

- Exact incident IDs generated during **Stage 1**

- Order MUST match the weekly aggregation order

- No sorting, deduplication, or inference is permitted

Example:

INC-20260102-c469c7d486

INC-20260103-a91f02bc12

INC-20260104-88de21a9ff

This list is authoritative for weekly traceability.

**D.3.3 Incident Count**

- Integer value

- MUST equal the number of incident IDs provided

- MUST NOT be derived or recalculated

Example:

incident_count: 68

**D.3.4 Generation Timestamp**

- ISO 8601 format

- Represents when the weekly bundle was finalized

- Not inferred from file timestamps

Example:

2026-01-14T18:42:11Z

### D.4 Optional Inputs (STRONGLY RECOMMENDED)

These inputs are optional but materially improve auditability.

**D.4.1 Orchestrator Version**

- Semantic version of the orchestrator used to generate weekly artifacts

Example:

orchestrator_version: v1.0

This links weekly outputs to a specific execution contract.

**D.4.2 incidents.csv Integrity Hash**

- SHA-256 hash of the finalized incidents.csv

- Generated per Appendix C

Example:

incidents_csv_hash:
3f9c1e6a9a0d6d3b7c4a9c8e1f4e2b6c9d0f1a2b3c4d5e6f7a8b9c0d1e2f3

**D.5 Canonical manifest.md Structure (REFERENCE)**

The following structure is recommended but not enforced by the
orchestrator:

\# Manifest --- CW02 2026

week: CW02 2026

incident_count: 68

incident_ids:

\- INC-20260102-c469c7d486

\- INC-20260103-a91f02bc12

\- INC-20260104-88de21a9ff

generated_at: 2026-01-14T18:42:11Z

orchestrator_version: v1.0

incidents_csv_hash: \<optional\>

Formatting may vary, but **values must remain identical**.

### D.6 Hard Constraints (NON-NEGOTIABLE)

The manifest generator MUST NOT:

- infer or reorder incident IDs

- recalculate incident_count

- derive timestamps automatically

- read or parse incident text

- depend on taxonomy or prevention outputs

- modify historical manifests

If any required input is missing:

- manifest generation MUST halt

- the missing field MUST be requested explicitly

### D.7 Governance Note

Appendix D:

- introduces no new pipeline behavior

- formalizes an existing implicit practice

- applies only to weekly metadata

- does not affect Stage 0--3 execution

This appendix is compatible with **Orchestrator Spec v1.0** and
qualifies as a **MINOR documentation hardening** if revised.

## Appendix E --- Single-Incident File Generation

**Status:** FINAL / PRODUCTION\
**Scope:** Canonical Incident Storage (Atomic Records)\
**Audience:** Analyst, Editor, Automation\
**Applies To:** /incidents/ directory\
**Effective From:** CW02 2026\
**Breaking Change:** No (tooling + storage workflow only)

### E.1 Purpose

This appendix defines the **authoritative method** for generating **one
file per incident** from a weekly incidents.csv snapshot.

This procedure enforces the core design principle of the pipeline:

**Atomic truth at the incident level.**

Each incident is stored as an immutable, standalone artifact that can be
referenced, audited, and reused independently of weekly outputs.

### E.2 Why Single-Incident Files Exist

Weekly artifacts under weeks/YYYY/CWxx/ are **editorial snapshots**.\
They can be regenerated at any time.

Canonical incident records under /incidents/ are the **source of
truth**.

Creating one file per incident:

- preserves immutability of Stage 1 outputs,

- enables precise audit trails,

- prevents "quiet rewrites" of historical incidents,

- improves version-control diffs (one incident = one file),

- allows weekly artifacts to be rebuilt without loss of provenance.

This mirrors storage practices used in:

- vulnerability databases,

- incident response timelines,

- regulated reporting systems.

### E.3 Inputs (REQUIRED)

Before running this procedure, you MUST have:

- a finalized incidents.csv for the week,

- containing at minimum:

  - id

  - first_observed_date (ISO 8601: YYYY-MM-DD)

The incidents.csv file MUST already comply with:

- Orchestrator Spec v1.0

- Appendix B (safe ingest)

- Appendix C (if hashing is used)

### E.4 Outputs (CANONICAL ARTIFACTS)

This procedure produces:

- **one CSV file per incident**

- each file contains:

  - the CSV header

  - exactly one incident row

**Filename Rule (LOCKED)**

\<incident_id\>.csv

Example:

INC-20260104-c469c7d486.csv

Filenames are authoritative and MUST NOT be altered after creation.

### E.5 Hard Constraints (NON-NEGOTIABLE)

The generator MUST NOT:

- reclassify incidents

- modify text fields

- normalize or reformat dates

- reorder fields

- change delimiters

- "clean up" whitespace

- silently overwrite existing incident files

If any row is invalid (e.g., missing id, invalid date format), the
process MUST **fail fast**.

### [E.6 Canonical Single-Incident File Generation (Implementation-Controlled)]{.mark}

**[Purpose]{.mark}**

[This section defines the **authority boundary** for generating
canonical single-incident files.]{.mark}

[The creation of one file per incident is a **deterministic, governed
operation** that enforces the immutability guarantees defined in this
specification. The goal is to persist each incident as an atomic,
standalone artifact without introducing reinterpretation or
drift.]{.mark}

**[Execution Boundary]{.mark}**

[The executable tooling used to generate single-incident files:]{.mark}

- [is a **normative execution artifact**,]{.mark}

- [enforces the constraints defined in this appendix,]{.mark}

- [may be **access-controlled**, and]{.mark}

- [is **not required to be publicly distributed**.]{.mark}

[This separation is intentional.]{.mark}

[The public specification defines:]{.mark}

- [*what* properties the storage system guarantees,]{.mark}

- [*when* single-incident files are generated,]{.mark}

- [*how* they relate to weekly artifacts,]{.mark}

- [*which invariants must never be violated*.]{.mark}

[The private implementation defines:]{.mark}

- [*how* those guarantees are mechanically enforced.]{.mark}

**[Contractual Guarantees]{.mark}**

[Regardless of implementation details, the following guarantees MUST
hold:]{.mark}

- [Exactly one file is generated per incident.]{.mark}

- [Filenames are derived directly and exclusively from the incident
  ID.]{.mark}

- [File contents reflect the canonical structured record
  exactly.]{.mark}

- [Existing canonical files are never overwritten.]{.mark}

- [Any invalid row causes the generation process to fail fast.]{.mark}

[Any implementation that violates these guarantees is non-compliant with
this specification.]{.mark}

### [E.7 Operational Use and Immutability Rules]{.mark}

**[Generation Timing]{.mark}**

[Single-incident file generation occurs **after weekly aggregation is
finalized** and any applicable integrity anchoring (e.g., hashing) has
completed.]{.mark}

[This operation:]{.mark}

- [does not alter canonical incident content,]{.mark}

- [does not affect weekly analytics,]{.mark}

- [and does not introduce new interpretation.]{.mark}

**[Immutability Rules]{.mark}**

[Once a single-incident file is created:]{.mark}

- [it MUST be treated as immutable,]{.mark}

- [it MUST NOT be edited, regenerated, or replaced,]{.mark}

- [its filename MUST NOT change,]{.mark}

- [its contents MUST remain byte-for-byte stable.]{.mark}

[Canonical incident files represent **atomic truth**, not working
documents.]{.mark}

**[Relationship to Weekly Artifacts]{.mark}**

[Weekly artifacts under weeks/YYYY/CWxx/:]{.mark}

- [are editorial snapshots,]{.mark}

- [may be regenerated,]{.mark}

- [may evolve across tooling or formatting changes.]{.mark}

[Canonical incident files under /incidents/:]{.mark}

- [are the authoritative record,]{.mark}

- [persist independently of weekly outputs,]{.mark}

- [always take precedence in case of conflict.]{.mark}

**[Failure Handling]{.mark}**

[If canonical file generation fails due to:]{.mark}

- [missing incident IDs,]{.mark}

- [invalid date formats,]{.mark}

- [duplicate filenames,]{.mark}

- [or any constraint violation,]{.mark}

[the process MUST halt and surface the error explicitly. Silent partial
generation is prohibited.]{.mark}

### E.8 Forbidden Practices (NON-NEGOTIABLE)

Do NOT:

- open and re-save incident files in Excel

- regenerate and overwrite existing incident files

- change filenames after publication

- manually edit incident CSVs

- apply corrections without governance approval

Violations break the canonical identity and audit chain.

### E.9 Governance Note

Appendix E:

- does not modify Stage 0--3 behavior

- introduces a deterministic storage workflow

- formalizes canonical incident persistence

- applies only after weekly aggregation is complete

This appendix is compatible with **Orchestrator Spec v1.0** and
qualifies as a **MINOR documentation hardening** if revised.

## Appendix F --- Prompt 0: Duplicate Incident Detection

[**Status:** Status: FINAL / CONTRACTUAL]{.mark}\
**Stage:** 0 --- Human Collection Plane → Intelligence Plane Boundary\
**Scope:** Link-level duplicate detection\
**Audience:** Analyst, Automation, Auditor\
**Execution Mode:** Standalone / Isolated\
**Breaking Change:** No (behavior already enforced)

### F.1 Purpose

Prompt 0 defines the **only approved mechanism** for detecting duplicate
incident entries **before ingestion** into the Intelligence Plane.

Its purpose is to:

- identify duplicate source links deterministically,

- prevent accidental double-ingest of identical sources,

- preserve atomic incident truth downstream.

Prompt 0 operates **only on source links**.\
It does not reason about incidents, mechanisms, or outcomes.

### F.2 Design Constraints (NON-NEGOTIABLE)

**Execution Authority Notice**

[Prompt 0 is a **normative execution artifact** governed by the CSF
Orchestrator.]{.mark}

[This public appendix defines:]{.mark}

- [the scope of duplicate detection,]{.mark}

- [the guarantees Prompt 0 provides,]{.mark}

- [and the boundaries it must not cross.]{.mark}

[The **exact executable prompt text and implementation details** used in
production:]{.mark}

- [may be access-controlled,]{.mark}

- [are not required to be publicly distributed,]{.mark}

- [and are authoritative only within CSF-governed execution
  environments.]{.mark}

[This separation preserves auditability while preventing silent
divergence or misuse.]{.mark}

### F.3 F.3 Conceptual Inputs

Prompt 0 operates on a minimal, link-level input set sufficient to
identify potential duplicate sources.

Conceptually, inputs include:

- a human reference identifier (e.g., entry number),

- a reported date (reference-only),

- a source link (URL).

Only source links are used for duplicate detection.\
All other fields are treated as non-authoritative context.

The exact input schema and formatting requirements are defined in the
controlled execution artifact.

### F.4 Duplicate Definition (LOCKED)

Two or more entries are considered duplicates **if and only if** their
Source Link values are identical **after normalization**.

No other signals are permitted.

**Explicitly NOT Allowed for Duplicate Inference**

Prompt 0 MUST NOT infer duplicates based on:

- similar titles,

- similar descriptions,

- same date,

- same domain alone,

- same subreddit or account,

- same incident mechanism.

Only normalized URL equality is valid.

### [F.5 URL Normalization (Contractual Guarantee)]{.mark}

[Duplicate detection relies on a **locked, deterministic URL
normalization procedure**.]{.mark}

[The normalization process:]{.mark}

- [operates only on the source URL,]{.mark}

- [is order-sensitive and deterministic,]{.mark}

- [produces a single canonical string used for matching.]{.mark}

[Normalization explicitly does not:]{.mark}

- [infer semantic equivalence across different URLs,]{.mark}

- [merge related but distinct reports,]{.mark}

- [rely on titles, text content, or metadata.]{.mark}

[The authoritative normalization rules are defined in the controlled
execution implementation referenced by this specification.]{.mark}

[Any change to normalization logic:]{.mark}

- [REQUIRES a MAJOR orchestrator version change,]{.mark}

- [MUST NOT be applied retroactively to existing outputs.]{.mark}

### [F.6 Execution Responsibilities]{.mark}

[Prompt 0 performs the following responsibilities in a deterministic
sequence:]{.mark}

1.  [Validate input integrity.]{.mark}

2.  [Normalize source links using the locked normalization
    procedure.]{.mark}

3.  [Group entries by normalized link.]{.mark}

4.  [Flag groups containing more than one entry.]{.mark}

[Prompt 0 does not resolve duplicates.\
It flags potential duplication and exits.]{.mark}

### F.7 Output Rules (STRICT)

[Output structure is stable within a MAJOR orchestrator version.\
Minor formatting details may vary across implementations provided
semantic equivalence is preserved.]{.mark}

**If NO duplicates exist**

Output exactly:

No duplicate entries found.

No additional text is permitted.

**If duplicates exist**

Output **only** the following table:

Duplicate Group \| Entry Numbers \| Normalized Source Link

Where:

- Duplicate Group

  - sequential numbering starting at 1

- Entry Numbers

  - comma-separated

  - ascending order

- Normalized Source Link

  - the canonical URL used for matching

No commentary, explanation, or remediation advice is allowed.

### F.8 Forbidden Actions (NON-NEGOTIABLE)

Prompt 0 MUST NOT:

- suggest deletions,

- select a "primary" record,

- recommend merges,

- comment on correctness,

- invent data,

- reinterpret incidents,

- use dates or text for matching.

Any such behavior invalidates the output.

### F.9 Outputs and Boundary Rules

The output of Prompt 0 MUST be stored verbatim as:

DUPLICATE_REPORT

**Boundary Rule (CRITICAL)**

Downstream stages:

- MUST NOT modify the duplicate report,

- MUST NOT reinterpret its results,

- MUST NOT auto-delete or suppress entries.

Prompt 0 flags potential duplicates; it does not resolve them.

### F.10 Governance Note

[Publication of this appendix does not grant permission to reimplement
Prompt 0 outside CSF governance without explicit authorization.]{.mark}

Prompt 0:

- operates entirely within the Human Collection Plane,

- is advisory, not authoritative for incident identity,

- does not affect Stage 1 classification immutability,

- preserves deterministic, link-based provenance.

This prompt is **normative** for Orchestrator Spec v1.0 and any future
compatible minor versions.

## Appendix G --- Prompt 1: Atomic Incident Ingest

[**Status:** FINAL / CONTRACTUAL / LOCKED]{.mark}\
**Stage:** 1 --- Atomic Incident Ingest\
**Scope:** Canonical incident record creation\
**Audience:** Analyst, Automation, Auditor\
**Execution Mode:** Standalone / Isolated\
**Output Format:** PSV (pipe-separated values)\
**Breaking Change:** Yes if modified (Stage 1 is immutable)

### G.1 Purpose

**[Execution Authority Notice]{.mark}**

[Prompt 1 is a **normative execution artifact** governed by the CSF
Orchestrator.]{.mark}

[This public appendix defines:]{.mark}

- [the guarantees Prompt 1 provides,]{.mark}

- [the invariants it enforces,]{.mark}

- [and the boundaries it must not cross.]{.mark}

[The **exact executable prompt text**, including internal decision
heuristics and formatting enforcement:]{.mark}

- [may be access-controlled,]{.mark}

- [is not required to be publicly distributed,]{.mark}

- [is authoritative only within CSF-governed execution
  environments.]{.mark}

[This separation is intentional and preserves:]{.mark}

- [immutability,]{.mark}

- [auditability,]{.mark}

- [and resistance to adversarial prompt gaming.]{.mark}

### G.2 Design Principles (NON-NEGOTIABLE)

Prompt 1 is designed to enforce:

- **atomic truth** --- one incident, one record,

- **determinism** --- same input, same output,

- **immutability** --- no silent edits downstream,

- **explicit ambiguity** --- uncertainty is surfaced, never resolved
  silently.

Prompt 1 MUST be executable in isolation.\
It MUST NOT rely on memory, prior prompts, or downstream stages.

### G.3 Conceptual Inputs (ALWAYS REQUIRED)

Prompt 1 receives **exactly** the following inputs:

- incident_id

- source_url

- incident_text

**Input Authority Rules**

- incident_id is **pre-generated**, globally unique, and authoritative

- Prompt 1 MUST NOT generate, hash, normalize, or reinterpret
  incident_id

- Missing or malformed inputs do **not** prevent output (see error
  handling)

[The exact input serialization and invocation format are defined by the
controlled execution environment and are not part of the public
contract.]{.mark}

### G.4 Date Handling (LOCKED)

The incident date is derived **only** from incident_id.

**Rules**

- incident_id format is guaranteed as:

- INC-YYYYMMDD-hash

- first_observed_date MUST be derived by converting YYYYMMDD →
  YYYY-MM-DD

- Prompt 1 MUST NOT:

  - infer dates from incident_text

  - infer dates from source_url

  - normalize or reinterpret dates

**Failure Handling**

If incident_id is malformed or the date cannot be derived:

- output **exactly one PSV row**

- set:

- classification_warning = invalid incident id date

### [G.5 Source Name Detection (Contractual Rules)]{.mark}

[source_name is derived deterministically from the source_url
domain.]{.mark}

[Rules:]{.mark}

- [Domain root only (no paths or subdomains).]{.mark}

- [Title Case formatting.]{.mark}

- [No inference beyond observable URL structure.]{.mark}

[If the source cannot be reliably determined:]{.mark}

[source_name = Unknown]{.mark}

[The authoritative domain-to-name mappings are defined in the controlled
execution artifact and are stable within a MAJOR orchestrator
version.]{.mark}

### G.6 Output Format (STRICT --- PSV)

Prompt 1 MUST output:

- **exactly one line**

- **exactly 10 fields**

- **pipe-separated (\|)**

- **no commas**

- **no quotes**

- **no line breaks**

**Field Order (LOCKED)**

1.  id

2.  first_observed_date

3.  incident_type

4.  incident_subtype

5.  source_name

6.  source_url

7.  summary

8.  user_mistake

9.  prevention

10. classification_warning

⚠️ Pipes (\|) are the ONLY delimiter.\
⚠️ Any comma renders the output invalid.

### G.7 Incident Type Classification (LOCKED)

Exactly **one** incident_type MUST be chosen.

Allowed values:

- scam

- hack

- user_mistake

**Classification Precedence (MANDATORY)**

1.  Deception, impersonation, manipulation, psychological pressure →
    scam

2.  Technical compromise without intentional user approval → hack

3.  No attacker involved → user_mistake

If unsure between scam and hack → **default to scam**.

### [G.8 Incident Subtype Taxonomy (LOCKED --- CONTRACTUAL)]{.mark}

[Exactly one incident_subtype MUST be selected for each incident,
consistent with the chosen incident_type.]{.mark}

[Subtype selection is governed by a **locked, finite taxonomy** that is
stable within a MAJOR orchestrator version.]{.mark}

**[Contractual Rules]{.mark}**

- [Subtypes reflect the **primary mechanism of loss or compromise**, not
  secondary effects.]{.mark}

- [Selection MUST be based solely on observable claims in the incident
  text.]{.mark}

- [Exactly one subtype MUST be chosen.]{.mark}

- [Subtypes MUST belong to the allowed set for the selected
  incident_type.]{.mark}

- [New, ad-hoc, or inferred subtypes are strictly forbidden.]{.mark}

**[Interpretation Constraints]{.mark}**

- [Subtype selection MUST NOT:]{.mark}

  - [infer attacker sophistication,]{.mark}

  - [speculate on intent,]{.mark}

  - [merge multiple mechanisms into a single label,]{.mark}

  - [resolve ambiguity silently.]{.mark}

- [When multiple mechanisms appear plausible, the **initial access
  vector** takes precedence.]{.mark}

**[Authority and Versioning]{.mark}**

[The authoritative subtype lists and their exact definitions are defined
in the controlled execution artifact referenced by this
specification.]{.mark}

[Any change to:]{.mark}

- [subtype membership,]{.mark}

- [subtype definitions,]{.mark}

- [or subtype selection rules]{.mark}

[REQUIRES a **MAJOR orchestrator version change** and MUST NOT be
applied retroactively.]{.mark}

### G.9 Ambiguity Handling (MANDATORY)

- incident_type and incident_subtype MUST NEVER be blank

- If uncertain:

  - choose the closest allowed value

  - surface uncertainty in classification_warning

Silent ambiguity is forbidden.

### [G.10 Field Content Rules (CONTRACTUAL)]{.mark}

[Prompt 1 produces structured text fields that are governed by strict
content constraints. These rules exist to preserve auditability, prevent
narrative drift, and block speculative interpretation.]{.mark}

**[summary]{.mark}**

- [Length: 1--3 sentences.]{.mark}

- [Content MUST describe:]{.mark}

  - [who was affected,]{.mark}

  - [what occurred,]{.mark}

  - [how the loss or compromise happened.]{.mark}

- [Focus MUST remain on the **mechanism**, not consequences or
  emotions.]{.mark}

- [Speculation, assumptions, or probability language are
  forbidden.]{.mark}

[Formatting rules:]{.mark}

- [No commas.]{.mark}

- [Avoid non-ISO date formats.]{.mark}

- [Use clear, literal wording only.]{.mark}

**[user_mistake]{.mark}**

- [Represents the **single primary enabling decision**, if any.]{.mark}

- [If no clear enabling action is present, output:]{.mark}

[none_obvious]{.mark}

**[prevention (FREE TEXT --- CONTRACTUAL)]{.mark}**

- [MUST describe **concrete, actionable behavior** that would have
  prevented the incident.]{.mark}

- [MUST be specific to the incident mechanism.]{.mark}

- [Use imperative verbs.]{.mark}

- [Limit to one or two actions, separated by /.]{.mark}

[Prevention text MUST NOT:]{.mark}

- [include generic or boilerplate safety advice,]{.mark}

- [restate common security slogans,]{.mark}

- [generalize beyond the incident context.]{.mark}

[If no safe, specific preventive action can be stated without
inference:]{.mark}

[none_obvious]{.mark}

[The authoritative enforcement rules for prevention phrasing, including
disallowed generic patterns, are defined in the controlled execution
artifact and are stable within a MAJOR orchestrator version.]{.mark}

### G.11 classification_warning

Allowed values:

- none (default)

- ≤ 10 words describing uncertainty or issue

Examples:

- insufficient detail to classify confidently

- mixed scam and technical vectors

- taxonomy pressure resolved

- invalid incident id date

- missing incident id

### G.12 Invalid Output Handling (MANDATORY)

If ANY of the following occur:

- missing incident_id

- invalid incident_id date

- taxonomy violation

- ambiguous classification

- formatting risk

Prompt 1 MUST:

- still output **exactly one PSV row**

- surface the issue explicitly in classification_warning

Prompt 1 MUST NOT fail silently.

### G.13 Final Output Rule

After analysis, output **ONLY** the PSV row.

Do NOT include:

- explanations

- commentary

- headers

- formatting

### G.14 Governance Note

Prompt 1:

- is the **classification authority** for the pipeline

- defines immutable incident truth

- feeds all downstream analytics and governance

- MUST NOT be modified without a MAJOR version bump

Any change to Prompt 1:

- invalidates historical comparability

- requires explicit versioning and migration notes

[Publication of this appendix does not authorize independent
reimplementation of Prompt 1 outside CSF governance without explicit
permission.]{.mark}

## Appendix H --- Prompt 2: Taxonomy Analytics

[**Status:** FINAL / CONTRACTUAL / HARDENED]{.mark}\
**Stage:** 2 --- Dataset Analytics\
**Scope:** Taxonomy distribution, integrity checks, and pattern
visibility\
**Audience:** Analyst, Automation, Auditor\
**Execution Mode:** Standalone / Isolated\
**Breaking Change:** Yes if taxonomy or output contract changes

### H.1 Purpose

**[Execution Authority Notice]{.mark}**

[Prompt 2 is a **normative execution artifact** governed by the CSF
Orchestrator.]{.mark}

[This public appendix defines:]{.mark}

- [the analytical guarantees Prompt 2 provides,]{.mark}

- [the integrity checks it enforces,]{.mark}

- [and the invariants governing its outputs.]{.mark}

[The exact executable prompt text and implementation details:]{.mark}

- [may be access-controlled,]{.mark}

- [are not required to be publicly distributed,]{.mark}

- [are authoritative only within CSF-governed execution
  environments.]{.mark}

[This separation preserves auditability, determinism, and resistance to
analytical drift.]{.mark}

### H.2 Design Principles (NON-NEGOTIABLE)

Prompt 2 is designed to enforce:

- **immutability of classification** --- no re-labeling or correction,

- **determinism** --- identical inputs yield identical outputs,

- **zero-fill completeness** --- all taxonomy categories are always
  represented,

- **explicit uncertainty disclosure** --- warnings are surfaced, never
  resolved.

Prompt 2 MUST be executable in isolation.\
It MUST NOT rely on Prompt 1 or Prompt 3 behavior beyond provided
inputs.

### H.3 Inputs (STRICT)

Prompt 2 receives a dataset consisting of multiple incident records with
**exactly** the following extracted fields:

- entry_number

- incident_type

- incident_subtype

- classification_warning

**Input Authority Rules**

- entry_number is run-scoped and used **only for traceability**

- Prompt 2 MUST NOT assume global stability of entry_number

- Missing or malformed inputs MUST be reported, not corrected

[The exact input serialization and invocation format are defined by the
controlled execution environment and are not part of the public
contract.]{.mark}

### H.4 Locked Taxonomy Reference (MANDATORY)

[Prompt 2 operates against the same locked incident_type and
incident_subtype taxonomies defined by the orchestrator.]{.mark}

[The taxonomy:]{.mark}

- [is finite and versioned,]{.mark}

- [is stable within a MAJOR orchestrator version,]{.mark}

- [requires zero-fill reporting for all categories.]{.mark}

[Prompt 2 MUST:]{.mark}

- [validate values against the locked taxonomy,]{.mark}

- [surface invalid values explicitly,]{.mark}

- [never correct, merge, or reinterpret classifications.]{.mark}

[The authoritative taxonomy lists are defined in the controlled
execution artifact and versioned alongside the orchestrator.]{.mark}

### H.5 Input Integrity & QC Checks (MANDATORY)

Prompt 2 MUST perform the following checks before analysis.

**H.5.1 Schema Presence Check**

- Confirm all records contain all required fields

- If missing fields exist:

  - report the number of affected records

  - list affected entry_number values

  - continue analysis using available data

**H.5.2 Entry Number Integrity**

- entry_number values MUST be unique integers

- If duplicates, gaps, or non-integers exist:

  - report count and affected values

  - do NOT correct them

**H.5.3 Taxonomy Validity Check**

- Verify incident_type and incident_subtype values against the locked
  taxonomy

- If invalid values exist:

  - list affected entry_number values

  - report the invalid values

  - do NOT reclassify or correct them

  - continue analysis using provided values

**H.5.4 Classification Warning Audit**

- Count records where classification_warning ≠ none

- If missing, null, or empty:

  - treat as unknown_missing_warning_field

- Report:

  - total count

  - affected entry_number values

If the same warning pattern appears across multiple runs, flag this as a
**taxonomy pressure signal**.

### H.6 Dataset Scope Declaration

Prompt 2 MUST explicitly state:

- total number of incidents analyzed

If zero incidents exist:

- explicitly state that the dataset is empty

- still output all required tables with zero-fill

### H.7 Incident Type Distribution

For each incident_type, Prompt 2 MUST report:

- total count

- percentage of total incidents

- percentages rounded to **1 decimal place**

If total incidents = 0:

- all percentages MUST be 0.0

### H.8 Subcategory Tables (MANDATORY)

Prompt 2 MUST output **three tables in this exact order**:

1.  Hack Subcategories

2.  Scam Subcategories

3.  User Mistake Subcategories

**Table Rules (STRICT)**

Each table MUST:

- include **all** subcategories listed in the locked taxonomy

- use zero-fill for unused categories

- include the following columns:

  - Subcategory

  - Count

  - Entry Numbers (comma-separated, ascending)

  - \% of Total Incidents (rounded to 1 decimal)

**Traceability Rules**

- Entry numbers MUST match input exactly

- Records with classification warnings are included normally

- Counts are never altered to "clean" the data

### H.9 Insight Blocks (STRICT)

After **each** subcategory table, Prompt 2 MUST:

- identify the top subcategories by share

- if multiple subcategories are tied:

  - explicitly state that no single dominant subcategory exists

  - list tied subcategories alphabetically

- state whether insights are affected by classification warnings

❌ No speculation\
❌ No advice\
❌ No extrapolation beyond provided data

### H.10 Big-Picture Takeaways (EXACTLY THREE)

Prompt 2 MUST output **exactly three numbered takeaways**:

1️⃣ Dominant incident type by share (numerically supported)\
2️⃣ Top three most common subcategories across all types

- ranked by count

- ties broken alphabetically for determinism\
  3️⃣ Upper-bound prevention relevance estimate

- based solely on the dominant incident type's share

- no prevention actions inferred or referenced

### H.11 Output Rules (NON-NEGOTIABLE)

Prompt 2 MUST:

- always output all tables

- preserve zero-fill categories

- round percentages to 1 decimal

- report all classification warnings explicitly

- base conclusions **only** on provided records

- NOT reference Prompt 1, Prompt 3, or external schemas

### H.12 Governance Note

Prompt 2:

- is analytical and observational only

- does not alter incident truth

- provides early warning of taxonomy pressure

- supports auditability and longitudinal analysis

Any change to:

- taxonomy lists,

- required tables,

- or output structure

constitutes a **breaking change** requiring a MAJOR version bump.

[Publication of this appendix does not authorize independent
reimplementation of Prompt 2 outside CSF governance without explicit
permission.]{.mark}

## Appendix I --- Prompt 3: Prevention Action Normalization

**Status:** [FINAL / CONTRACTUAL / HARDENED]{.mark}\
**Stage:** 3 --- Prevention Action Normalization\
**Scope:** Dataset-level prevention mapping and coverage analysis\
**Audience:** Analyst, Automation, Auditor\
**Execution Mode:** Standalone / Isolated\
**Breaking Change:** Yes if action set or output contract changes

### I.1 Purpose

[Place right after **I.1 Purpose**:]{.mark}

[**Execution Authority Notice (Public)**\
Prompt 3 is a **normative execution artifact** governed by the CSF
Orchestrator.]{.mark}

[This public appendix defines:]{.mark}

- [the guarantees Prompt 3 provides,]{.mark}

- [the required validation checks,]{.mark}

- [and the output invariants that make weekly results auditable.]{.mark}

[The exact executable prompt text, mapping implementation details, and
any automation used to run Prompt 3:]{.mark}

- [may be access-controlled,]{.mark}

- [are not required to be publicly distributed,]{.mark}

- [are authoritative only within CSF-governed execution
  environments.]{.mark}

### I.2 Design Principles (NON-NEGOTIABLE)

Prompt 3 enforces:

- **determinism** --- identical inputs yield identical mappings,

- **conservatism** --- no forced mappings,

- **comparability** --- a fixed, zero-filled action set,

- **explicit uncertainty** --- unmappable cases are disclosed.

Prompt 3 MUST be executable in isolation.\
It MUST NOT rely on memory, prior prompts, or external schemas.

### I.3 Inputs (STRICT)

Prompt 3 receives a dataset of structured incident records with
**exactly** the following fields:

- entry_number

- incident_type

- incident_subtype

- summary

- user_mistake

- prevention

- classification_warning

**Input Authority Rules**

- entry_number is run-scoped and used **only for traceability**

- Prompt 3 MUST NOT assume global stability of entry_number

- Missing or malformed fields MUST be reported, not corrected

[The exact input serialization and invocation format are defined by the
controlled execution environment and are not part of the public
contract.]{.mark}

### I.4 Locked Prevention Action Set [(CONTRACTUAL)]{.mark}

Prompt 3 maps free-text prevention guidance into a **finite, versioned
prevention action set** maintained by CSF.

Public guarantees:

- The action set is **locked within a MAJOR orchestrator version**.

- Outputs are **zero-filled**, so all actions are reported even when
  unused.

- Prompt 3 **MUST NOT** invent new actions, rename existing actions, or
  generalize beyond recorded text.

- Any change to the action set is a **breaking change** requiring a
  MAJOR version bump and explicit changelog entry.

The authoritative action list is defined in the controlled execution
artifact referenced by this specification.

### I.5 Input Integrity Checks (MANDATORY)

Before normalization, Prompt 3 MUST perform the following checks.

**I.5.1 Schema Presence Check**

- Confirm all records contain all required fields

- If missing fields exist:

  - report the number of affected records

  - list affected entry_number values

  - continue using available fields only

**I.5.2 Entry Number Integrity**

- entry_number values MUST be unique integers

- If duplicates or non-integers exist:

  - report affected entry_number values

  - do NOT correct them

**I.5.3 Classification Warning Audit**

- Count records where classification_warning ≠ none

- If missing, null, or empty:

  - treat as unknown_missing_warning_field

- Report:

  - total count

  - affected entry_number values

Normalization MUST proceed conservatively when warnings are present.

### I.6 Dataset Scope Declaration

Prompt 3 MUST explicitly state:

- total number of incidents analyzed

If zero incidents exist:

- explicitly state that the dataset is empty

- still output the full prevention action table with zero-fill

### I.7 Prevention Action Normalization (CORE TASK-[CONTRACTUAL]{.mark})

[or each incident, Prompt 3 MUST normalize recorded prevention guidance
according to the following rules.]{.mark}

**[Source of Truth]{.mark}**

- [The **prevention field** is the primary and authoritative
  input.]{.mark}

- [The **summary** and **user_mistake** fields MAY be used **only to
  clarify intent**, never to invent or generalize prevention
  actions.]{.mark}

- [Prompt 3 MUST NOT infer prevention actions that are not explicitly
  stated or unambiguously implied in the prevention field.]{.mark}

**[Mapping Rules (STRICT)]{.mark}**

- [Mapping is restricted to the **locked prevention action set** defined
  by the orchestrator.]{.mark}

- [One incident MAY map to **zero, one, or multiple** prevention
  actions.]{.mark}

- [An incident MUST be counted **at most once per action**.]{.mark}

- [Purely narrative, descriptive, or cautionary text MUST NOT be
  converted into prevention actions.]{.mark}

- ["Best practice" inference beyond the recorded text is explicitly
  forbidden.]{.mark}

**[Determinism Rule (MANDATORY)]{.mark}**

[Identical prevention text MUST always result in **identical action
mappings**, regardless of differences in:]{.mark}

- [incident type or subtype,]{.mark}

- [summary wording,]{.mark}

- [user_mistake description,]{.mark}

- [or dataset ordering.]{.mark}

[Determinism applies to the **mapping outcome**, not to any narrative
explanation.]{.mark}

**[Classification Warning Handling]{.mark}**

[If classification_warning ≠ none:]{.mark}

- [mapping MUST proceed conservatively,]{.mark}

- [ambiguous or borderline mappings SHOULD be avoided,]{.mark}

- [uncertainty MUST be surfaced explicitly in the analytical
  output.]{.mark}

**[Unmappable Prevention Text]{.mark}**

[If prevention text is:]{.mark}

- [missing, null, or empty,]{.mark}

- [vague or non-actionable,]{.mark}

- [internally contradictory,]{.mark}

- [incompatible with the locked action set,]{.mark}

[then Prompt 3 MUST:]{.mark}

- [produce **no forced mappings**,]{.mark}

- [distinguish between:]{.mark}

  - [missing prevention text,]{.mark}

  - [vague or non-actionable text,]{.mark}

  - [present but unmappable text,]{.mark}

- [surface this condition explicitly in the analysis.]{.mark}

**[Boundary Rule]{.mark}**

[Prompt 3 normalizes **recorded guidance only**.\
It does not assess ideal prevention, effectiveness, or
completeness.]{.mark}

### I.8 Prevention Actions Table (MANDATORY)

Prompt 3 MUST output **one table** containing **all 12 prevention
actions**, even if unused.

**Table Format (STRICT)**

Prevention Action \| Count \| Entry Numbers \| % of Total

**Table Rules**

- Count = number of incidents mapped to that action

- Entry Numbers = comma-separated, ascending

- percentages rounded to **1 decimal**

- unused actions:

  - Count = 0

  - Entry Numbers = empty

  - \% of Total = 0.0

If total incidents = 0:

- all percentages MUST be 0.0

### I.9 Prevention Insights (STRICT)

After the table, Prompt 3 MUST:

- identify the **top 3 prevention actions by coverage**

- rank by count

- break ties alphabetically for determinism

- state their **combined percentage** of total incidents

- explicitly state whether coverage is affected by:

  - classification warnings

  - missing or vague prevention text

  - unmappable prevention text

- explicitly note if mapped actions conflict with previously published
  guidance

❌ No speculation\
❌ No new advice\
❌ No recommendations beyond the locked action set

### I.10 Output Rules (NON-NEGOTIABLE)

Prompt 3 MUST:

- always output the full action table

- preserve zero-fill rows

- round percentages to 1 decimal

- surface ambiguity explicitly

- base conclusions **only** on provided records

- NOT reference Prompt 1, Prompt 2, or external schemas

### I.11 Governance Note

Prompt 3:

- standardizes actionability without inventing guidance

- enables longitudinal prevention coverage analysis

- makes gaps and vagueness measurable

- supports evidence-based education without speculation

Any change to:

- the locked action set,

- mapping rules,

- or output structure

constitutes a **breaking change** requiring a MAJOR version bump.

[Publication of this appendix does not authorize independent
reimplementation of Prompt 3 outside CSF governance without explicit
permission.]{.mark}

## Appendix J --- Documentation Conversion & Verification (DOCX → Markdown)

**Status:** FINAL / PRODUCTION\
**Scope:** Editorial Documentation Pipeline\
**Audience:** Editor, Maintainer, Auditor, Contributor\
**Applies To:** All published .md documentation derived from .docx
sources\
**Effective From:** Orchestrator Spec v1.0\
**Breaking Change:** No (documentation process only)

### J.1 Purpose

This appendix defines the authoritative, reproducible process for
converting Word (.docx) source documents into Markdown (.md) files for
publication.

Its purpose is to ensure that:

- published Markdown files are faithful representations of approved
  source documents,

- formatting changes do not introduce semantic drift,

- documentation artifacts remain auditable and reproducible over time.

This appendix governs **documentation conversion only**.\
It does not affect incident data, analytical outputs, or pipeline
execution behavior.

### J.2 Design Principles

The documentation pipeline follows the same integrity principles as the
intelligence pipeline:

- **Source authority** --- .docx files are the editorial source of truth

- **Mechanical conversion** --- no semantic rewriting during conversion

- **Determinism** --- identical inputs produce identical outputs

- **Auditability** --- reviewers can verify conversion fidelity

- **Separation of concerns** --- formatting ≠ interpretation

Markdown is treated as a **publication format**, not an authoring
format.

### J.3 Authoritative Conversion Tool

The only approved conversion tool is:

**Pandoc**\
https://pandoc.org

Rationale:

- deterministic output

- broad .docx support

- transparent CLI usage

- stable, widely audited toolchain

No GUI tools or online converters are permitted.

### J.4 Canonical Conversion Procedure

Conversion MUST be executed from the directory containing the source
.docx files.

Approved commands:

pandoc taxonomy_report.docx -o taxonomy_report.md

pandoc prevention_report.docx -o prevention_report.md

pandoc manifest.docx -o manifest.md

pandoc governance-notes.docx -o governance_notes.md

pandoc readme.docx -o README.md

Rules:

- one .docx → one .md

- filenames MUST match semantic intent

- no intermediate formats are permitted

### J.5 Post-Conversion Verification (MANDATORY)

After conversion, each .md file MUST be manually verified against its
.docx source.

Verification checklist:

1.  **Section order**

    - Headings appear in the same order

    - No missing or duplicated sections

2.  **Heading hierarchy**

    - Heading levels preserved (#, ##, ###)

    - No collapsed or promoted sections

3.  **Lists and tables**

    - Bullet and numbered lists preserved

    - Tables render completely and accurately

4.  **Normative language**

    - Keywords such as MUST, MUST NOT, SHOULD remain unchanged

    - No weakening or strengthening of requirements

5.  **No semantic edits**

    - No rewording

    - No summarization

    - No clarification added during conversion

If discrepancies are found:

- correct the **Markdown output only**

- do NOT modify the .docx source unless a documented editorial change is
  intended

### J.6 Forbidden Practices (NON-NEGOTIABLE)

The following actions are explicitly forbidden:

- Manual rewriting during conversion

- Editing .md files to "improve clarity"

- Using AI tools to paraphrase or restructure content

- Treating .md as an authoritative source over .docx

- Converting via copy-paste instead of Pandoc

- Merging multiple .docx files into one .md without governance approval

Any of the above invalidates the documentation artifact.

### J.7 Source of Truth Rule

For documentation artifacts:

- .docx = editorial source of truth

- .md = published representation

If a conflict exists:

- the .docx version prevails

- the .md file MUST be regenerated

Markdown files MUST NOT become the sole surviving authoritative version.

### J.8 Version Control and Publication

Best practices (strongly recommended):

- Commit .docx and .md files together when possible

- Use commit messages that explicitly state:

- docs: convert docx → md (no semantic changes)

- Avoid committing regenerated .md files without explanation

If only .md files are published:

- .docx files SHOULD be retained privately as provenance artifacts

### J.9 Governance Boundary

Appendix J:

- introduces no changes to pipeline logic

- affects no analytical or incident artifacts

- governs documentation integrity only

Revisions to this appendix:

- qualify as **MINOR version changes**

- MUST NOT alter incident outputs or historical intelligence

### J.10 Rationale

By documenting the documentation pipeline, CSF ensures that:

- published specifications are trustworthy

- formatting changes cannot quietly alter meaning

- auditors can verify editorial fidelity

- contributors understand the boundary between formatting and authorship

This appendix exists to prevent **silent drift** in the most overlooked
layer of security systems: documentation.

## Appendix M --- Weekly Governance Notes Input Contract

**Status:** FINAL / PRODUCTION\
**Scope:** Governance Plane --- Weekly Closure\
**Audience:** Analyst, Editor, Automation\
**Applies To:** governance_notes.md under weeks/YYYY/CWxx/\
**Effective From:** CW03 2026\
**Breaking Change:** No (documentation and workflow hardening only)

### M.1 Purpose

This appendix defines a **minimal, repeatable input contract** for
producing governance_notes.md.

It exists to:

- eliminate week-to-week cognitive load,

- prevent analytical or interpretive drift,

- ensure governance notes remain non-authoritative,

- make governance note generation deterministic and reproducible.

This appendix answers **one question only**:

**"What must be provided to generate governance notes --- and what must
never be inferred?"**

### M.2 Role of governance_notes.md

governance_notes.md serves as:

- a lightweight governance signal,

- a record of observed ambiguity or pressure,

- a forward-looking marker for future review.

It does **not**:

- summarize incidents,

- restate analytics,

- compute metrics,

- introduce conclusions,

- modify taxonomy or prevention logic,

- alter historical records.

Governance notes surface **friction**, not facts.

### M.3 Governance Position (Normative)

Canonical authority remains with:

- canonical incident records (/incidents/)

- analytical outputs (taxonomy_report.md, prevention_report.md)

- manifest.md (weekly scope anchor)

governance_notes.md is:

- non-canonical

- non-analytical

- advisory only

In the event of conflict:

**Canonical records and analytical outputs always override governance
notes.**

### M.4 Allowed Inputs (STRICT)

To generate weekly governance notes, the author or generator **MAY use
only**:

- qualitative observations made during weekly curation,

- classification_warning patterns already present in records,

- analyst awareness of conservative or refused mappings,

- explicit confirmation of integrity conditions.

The generator **MUST NOT**:

- read or parse raw incident text,

- compute counts or percentages,

- restate analytical conclusions,

- infer trends or rankings,

- introduce recommendations or guidance.

### M.5 Required Weekly Input Block (MANDATORY)

Each weekly governance note **MUST** be derived from the following
**copy-paste input block**, completed by a human.

Weekly Governance Input Block

CWXX Governance Inputs

1\. Classification ambiguity observed?

\- yes / no

\- if yes: short phrase describing the boundary or uncertainty

2\. Taxonomy pressure observed?

\- yes / no

\- if yes: subtype or category experiencing strain

3\. Prevention mapping friction?

\- yes / no

\- if yes: reason (e.g. vague text, narrative-only, conservative
refusal)

4\. Dataset integrity confirmation:

\- no reclassification performed

\- no scope changes made

\- no post-generation edits identified

Rules:

- Responses **MUST be qualitative only**

- One-line phrases are sufficient

- "no" is a valid and expected answer

### M.6 Output Constraints (NON-NEGOTIABLE)

From the input block, the generated governance_notes.md **MUST**:

- contain no tables,

- contain no metrics or counts,

- contain no rankings or trends,

- contain no decisions or recommendations,

- preserve a neutral, advisory tone,

- remain forward-looking only.

If all inputs are "no", the governance note **MUST still exist** and
explicitly state that no material governance signals were observed.

### M.7 Determinism & Reproducibility

- Governance notes may be written manually or generated.

- Given the same Weekly Governance Input Block, the output **MUST be
  reproducible**.

- Governance notes **MUST NOT** depend on hidden state, memory, or prior
  weeks.

Changes to governance notes do not invalidate weekly artifacts but
**MUST NOT** retroactively change meaning.

### M.8 Relationship to Other Appendices

- Appendix D defines weekly scope and integrity anchoring.

- Appendices F--I define analytical execution.

- Appendix J governs documentation conversion.

- Appendix M governs governance note **inputs only**.

No appendix supersedes another except where explicitly stated.

### M.9 Governance Note

Appendix M:

- introduces no new pipeline stages,

- adds no analytical authority,

- formalizes an existing practice,

- reduces cognitive and procedural risk,

- qualifies as **MINOR documentation hardening**.

## Appendix N --- Weekly Orchestration Map & End-to-End Process Flow

**Status:** INFORMATIONAL / NON-NORMATIVE\
**Scope:** Weekly CSF Incident Intelligence Lifecycle\
**Applies To:** All CWXX cycles\
**Authority:** None (navigational only)

### N.1 Purpose

This appendix provides:

1.  a **chronological orchestration map** showing which appendices apply
    at each phase of a weekly cycle, and

2.  a **reference end-to-end description** of the observed weekly
    operating flow.

It exists to:

- reduce onboarding and review friction,

- align human and automation mental models,

- make appendix applicability explicit by phase.

This appendix:

- introduces **no new requirements**,

- defines **no execution rules**,

- overrides **no authoritative appendix**.

In the event of conflict, **authoritative appendices always prevail**.

### N.2 Weekly Orchestration Map (Appendix Applicability)

This section indicates which authoritative appendices are relevant at
each phase of a standard CWXX cycle.\
It is **navigational only**.

**Phase 0 --- Ongoing Collection**

→ Appendix A (Incident ID system)\
→ Appendix F (Duplicate detection)

**Phase 1 --- Weekly Aggregation**

→ Appendix B (incidents.psv generation and safe ingest)

**Phase 2 --- Canonical Snapshot**

→ Appendix C (Integrity hashing)\
→ Appendix D (manifest.md input contract)

**Phase 3 --- Analytics**

→ Appendix G (Prompt 1 --- ingest authority)\
→ Appendix H (Prompt 2 --- taxonomy analytics)\
→ Appendix I (Prompt 3 --- prevention normalization)

**Phase 4 --- Governance & Editorial**

→ §7 Governance Plane\
→ Appendix M (Governance notes input contract)

**Phase 5 --- Persistence**

→ Appendix E (Single-incident canonical files)

**Phase 6 --- Documentation Conversion & Verification**

→ Appendix J (DOCX → Markdown)

### N.3 Reference End-to-End Weekly Process Flow

This section describes the **current observed weekly operating model**.\
It is **descriptive**, not prescriptive.

High-level flow:

**Raw signals → structured ingest → canonical dataset → analytics →
governance → immutable storage**

Detailed phase descriptions are distributed across §§3--9 and the
supporting appendices listed above.

This appendix does not restate those rules; it provides **orientation
only**.

### N.4 Mental Model (Non-Normative)

Each weekly cycle produces:

- immutable incident truth (canonical records),

- regenerable analytical snapshots (weekly artifacts),

- explicit governance signals (notes and manifest),

- a closed, auditable boundary.

Appendix N exists solely to help readers see that whole without
redefining any part of it.

### N.5 Governance Note

Appendix N:

- adds no authority,

- changes no behavior,

- documents existing practice,

- reduces mis-ordering and misinterpretation risk,

- qualifies as **MINOR documentation hardening**.
