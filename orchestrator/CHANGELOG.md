**Orchestrator Specification Change Log**

This file records all changes to the CSF Crypto Incident Intelligence
Pipeline\
Orchestrator Specification.

No change is considered valid unless recorded here.

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
