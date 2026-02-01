**Orchestrator Specification Change Log**

This file records all changes to the CSF Crypto Incident Intelligence
Pipeline\
Orchestrator Specification.

No change is considered valid unless recorded here.
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
