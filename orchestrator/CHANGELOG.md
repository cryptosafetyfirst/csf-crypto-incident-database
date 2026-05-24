**Orchestrator Specification Change Log**

This file records all changes to the CSF Crypto Incident Intelligence
Pipeline\
Orchestrator Specification.

No change is considered valid unless recorded here.

**v1.5 \-\-- 2026-05-24**

Status: MINOR (governance visibility expansion, analytical layer
separation, and registry governance hardening; non-breaking)

Revised Appendix K \-\-- README Generation Contract.

Clarified downstream artifact positioning and orchestration alignment
behavior.

Strengthened separation between canonical intelligence artifacts and
downstream analytical/governance overlays.

Preserved README generation as a derived publication artifact only.

Revised Appendix G \-\-- Atomic Incident Ingest Governance Hardening.

Expanded deterministic validation and schema enforcement visibility.

Clarified repair visibility boundaries and deterministic schema
correction behavior.

Preserved canonical ingest immutability and Stage 1 authority
boundaries.

Revised Appendix P \-\-- CSF Rule Alignment Snapshot Contract.

Replaced prior Defensive Coverage Gap governance appendix with a formal
downstream defensive alignment visibility layer.

Introduced deterministic governance visibility for:

- recurrence concentration,

- defensive layer distribution,

- alignment coverage,

- and residual / uncertain mappings.

Established csf_rule_alignment_snapshot.md as a downstream governance
visibility artifact.

Explicitly confirmed:

- non-canonical authority,

- non-modification of incidents,

- non-modification of taxonomy,

- non-modification of prevention mappings,

- and non-modification of governance rules.

Introduced fixed rendering structure and locked table schemas:

- \| Rule \| Occurrences \|

- \| Defensive Layer \| Occurrences \|

Introduced Appendix Q \-\-- CSF Rule Governance Delta Contract.

Established a governance advisory visibility layer for:

- recurrence pressure,

- persistent concentration behavior,

- uncovered defensive patterns,

- registry fragmentation visibility,

- and candidate rule emergence visibility.

Introduced csf_rule_governance_delta.md as a downstream governance
advisory artifact.

Explicitly prohibited:

- autonomous governance actions,

- automatic rule creation,

- registry modification,

- and reinterpretation of canonical incident intelligence.

Introduced fixed recurrence serialization schema:

- \| Rule \| Occurrences \|

Introduced Appendix R \-\-- Defensive Coverage Gap Report Contract.

Formalized deterministic downstream defensive sufficiency visibility
against the existing CSF Defensive Canon.

Established defensive coverage evaluation against:

- Practical Crypto & Web3 Safety Tools,

- Three-Wallet Model materials,

- CSF books,

- and governance-approved defensive canon artifacts.

Confirmed defensive coverage outputs as:

- downstream,

- non-canonical,

- governance-oriented,

- and non-authoritative.

Introduced explicit downstream attribution governance boundaries.

Established the Defensive Attribution Layer as:

- a downstream analytical overlay,

- non-canonical,

- read-only relative to canonical intelligence,

- and linked exclusively through incident_id.

Clarified that attribution mappings:

- do not modify incident records,

- do not modify taxonomy outputs,

- do not modify prevention mappings,

- and do not redefine defensive canon authority.

Authorized downstream attribution outputs including:

- primary_rule_id,

- primary_rule_name,

- primary_tool_id,

- primary_tool_name,

- mapping_status,

- and mapping_confidence.

Introduced explicit derived artifact classification separation.

Defined two derived artifact categories:

- Derived Publication Artifacts

- Derived Analytical Artifacts

Clarified governance and authority distinctions between:

- editorial/publication outputs,

- and downstream analytical overlays.

Introduced registry authority boundary formalization.

Established governance-controlled registry behavior for:

- subtype registries,

- prevention registries,

- CSF Rule Registry,

- CSF Tools Registry,

- and defensive canon reference registries.

Explicitly prohibited registries from:

- modifying canonical incident records,

- silently reinterpreting history,

- overriding immutable Stage 1 intelligence,

- or redefining historical incident meaning.

Introduced registry version pinning requirements.

Authorized explicit registry version declarations including:

- rules_registry_version

- tools_registry_version

Clarified that downstream analytical outputs dependent on registries
MUST remain reproducible against declared registry versions active
during generation.

Introduced attribution historical stability and non-retroactivity
controls.

Established that published attribution outputs:

- MUST NOT be silently rewritten,

- MUST disclose material regeneration,

- and MUST preserve deterministic reproducibility for identical declared
  inputs and registry versions.

Clarified that attribution outputs remain:

- downstream analytical overlays,

- non-canonical,

- and advisory only.

No changes were made to:

- pipeline stage ordering,

- canonical incident ingest structure,

- Stage 1 authority boundaries,

- taxonomy structure or labels,

- prevention normalization logic,

- immutable incident identity guarantees,

- canonical intelligence authority,

- or deterministic execution guarantees.

Artifacts produced under v1.0\--v1.4 remain valid and unaffected.


**v1.4 --- 2026-02-10**

**Status: MINOR (governance extension; non-breaking)**

- Introduced Appendix O --- FAQ Signal Report Output Contract (private
  governance appendix).

  - Defines a deterministic, CW-scoped output contract for
    faq_signal_report.md.

  - Establishes FAQ alignment as a governance-only, downstream
    validation mechanism.

  - Constrains FAQ updates to evidence derived solely from canonical
    weekly inputs.

  - Explicitly prohibits intuition-driven, anecdotal, UX-, SEO-, or
    marketing-led FAQ changes.

  - Confirms FAQ signal reports as non-public, non-educational,
    non-analytical, and non-canonical.

- Introduced Appendix P --- Defensive Coverage Gap Governance (private
  governance appendix).

  - Defines a CW-scoped defensive sufficiency audit for existing CSF
    defensive materials.

  - Evaluates whether observed prevention failures are already addressed
    by the Defensive Canon.

  - Establishes explicit halt authority if defensive canon materials are
    unavailable or ambiguous.

  - Prohibits inference, prioritization, recommendation, or feedback
    into intelligence outputs.

  - Confirms defensive coverage gap reports as non-public,
    non-educational, and non-analytical.

- • Added explicit authorization for non-public derived governance
  artifacts in the public specification.

  - Clarifies that downstream governance artifacts may exist for
    editorial or educational alignment checks.

  - o Affirms that such artifacts are read-only consumers of
    intelligence with no upstream authority.

No changes were made to:

- pipeline stage ordering,

- incident ingest or classification logic,

- taxonomy structure or labels,

- prevention mapping definitions,

- intelligence outputs or verdict generation,

- risk scoring behavior, or

- immutability and determinism guarantees.

Artifacts produced under v1.0--v1.3 remain valid and unaffected.

**v1.3 --- 2026-01-01**

**Status:** MINOR (governance automation enablement and schema
enforcement hardening; non-breaking)

- Revised Appendix M --- Weekly Governance Notes Input Contract.

  - Authorized a machine-declared Weekly Governance Input Block as an
    alternative to human-declared inputs.

  - Preserves governance notes as non-canonical, non-analytical, and
    advisory only.

  - Enables deterministic, auditable automation of governance_notes.md
    without introducing inference or analytical authority.

- Introduced explicit authorization for deterministic governance
  extractors.

  - Allows governance inputs to be declared by a documented, fixed-rule
    extractor when conditions are explicitly met.

  - Requires all machine-declared inputs to remain qualitative only
    (yes/no + short phrases).

  - Prohibits metrics, counts, rankings, trend inference, or raw
    incident text parsing.

- Defined non-inferential governance declaration triggers.

  - Classification ambiguity may be declared when classification_warning
    ≠ none exists.

  - Taxonomy pressure may be declared only when taxonomy analytics
    explicitly label a "taxonomy pressure signal."

  - Prevention mapping friction may be declared when conservative
    refusal or unmappable prevention text is reported.

  - Dataset integrity confirmation may be declared only when manifest
    and pipeline integrity conditions are satisfied.

- Preserved backward compatibility with human-declared governance
  workflows.

  - Manual Weekly Governance Input Blocks remain valid and supported.

  - No changes required for existing analyst-led processes.

- Hardened atomic incident ingest classification enforcement (Stage 1).

  - Locked incident_type to the canonical set {scam, hack,
    user_mistake}.

  - Enforced incident_subtype compatibility with the selected
    incident_type.

  - Explicitly prohibited mechanism, domain, technology, or outcome
    concepts from appearing in incident_type or incident_subtype.

  - Introduced deterministic schema repair rules to prevent ingest
    failure while preserving auditability.o Added mandatory
    SCHEMA_VIOLATION_REPORT.md artifact to surface repaired fields
    without silent correction.\
    o Explicitly clarified that schema enforcement does not constitute
    analytical reclassification.

- Hardened weekly CSV splitting utility to prevent false schema
  validation failures (operational tooling).

  - Updated the incidents.csv → single-incident CSV splitter to
    normalize id and first_observed_date using trim and NBSP
    sanitization prior to validation.

  - Prevents fail-fast regex validation from rejecting valid dates due
    to leading/trailing whitespace or non-breaking spaces introduced
    during export.

  - Maintains canonical safety guarantees (no overwrites; one row per
    output file) while improving reproducibility across Windows export
    environments.

**No changes were made to:**

- pipeline stage ordering,

- required inputs or outputs,

- prompt execution behavior (Appendices F--I),

- taxonomy structure,

- prevention action sets, or

- immutability guarantees.

Artifacts produced under v1.0--v1.2 remain valid and unaffected.
------------------------------------------------------------------------

**v1.2 --- 2026-01-25**

**Status:**MINOR (documentation hardening; non-breaking)

- Added **Appendix H-R --- Prompt 2 Reference Specimen
  (Informational).**

  - Provides a concrete, real-world reference specimen illustrating a
    fully compliant Prompt 2 (Taxonomy Analytics) output.

  - Demonstrates required section ordering, zero-fill enforcement,
    insight block placement, classification warning disclosure, and
    deterministic "Big-Picture Takeaways."

  - Explicitly designated as non-normative and non-authoritative;
    Appendix H remains the sole execution contract.

- Clarified publication rendering boundaries for Prompt 2 outputs.

  - Added a non-normative \*Publication Rendering Note\* to Appendix H.

  - Explicitly states that Prompt 2 governs analytical structure and
    content, not presentation tooling or file formats.

  - Affirms that table-native renderings (e.g., Word, Markdown, HTML)
    are permitted provided row and column structure, ordering, zero-fill
    completeness, and values are preserved verbatim.

  - Prevents misinterpretation of "table-native" as allowing column
    loss, renaming, reflow, or semantic alteration.

- Hardened documentation-to-publication alignment without altering
  execution behavior.

  - Aligns Prompt 2 analytical outputs with existing copy-paste → Word →
    Pandoc → Markdown workflows already used for Prompt 3 outputs.

  - Removes ambiguity around table serialization while preserving
    determinism, auditability, and immutability guarantees.

**No changes were made to:**

- pipeline stage ordering,

- required inputs or outputs,

- prompt execution behavior (Appendices F--I),

- taxonomy structure,

- prevention action sets, or

- immutability guarantees.

Artifacts produced under v1.0 and v1.1 remain valid and unaffected.

------------------------------------------------------------------------

**v1.1 --- 2026-02-01**

**Status:** MINOR (documentation hardening; non-breaking)

- Added **Appendix M --- Weekly Governance Notes Input Contract**.

  - Formalizes the allowed inputs, forbidden inference, and determinism
    guarantees for governance_notes.md.

  - Explicitly constrains governance notes to be non-canonical,
    non-analytical, and advisory only.

  - Introduces a mandatory human-provided Weekly Governance Input Block.

- Added **Appendix N --- Weekly Orchestration Map & End-to-End Process
  Flow**.

  - Provides a navigational, non-normative index mapping appendices to
    phases of a CWXX cycle.

  - Documents the observed end-to-end weekly operating model without
    introducing new requirements or authority.

- Clarified governance behavior in the main specification body:

  - Explicitly stated determinism and input-bound nature of
    governance_notes.md.

  - Added cross-references from §7 (Governance Plane) and §2 (System
    Overview) to Appendices M and N.

**No changes were made to:**

- pipeline stage ordering,

- required inputs or outputs,

- prompt behavior (Appendices F--I),

- taxonomy structure,

- prevention action sets, or

- immutability guarantees.

Artifacts produced under v1.0 remain valid and unaffected.

------------------------------------------------------------------------

**v1.0 --- 2026-01-21**

**Status:** Initial public release

- First public publication of the CSF Crypto Incident Intelligence
  Pipeline\
  Orchestrator Specification.

- Defines Collection, Intelligence, and Governance planes.

- Establishes atomic incident identity, immutability guarantees,\
  and weekly governance closure.

- Includes Appendices A--J as normative references.

No prior versions exist.
