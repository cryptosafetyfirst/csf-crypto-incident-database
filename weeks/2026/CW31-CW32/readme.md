**CW31 + CW32 2026**

**Purpose**

This weekly package provides the operational and publication artifacts
for CW31 + CW32 2026. It serves as the navigation layer for the weekly
aggregation package and provides access to canonical metadata, the
incident dataset, analytical outputs, and governance material.

**Folder Contents**

- manifest.md --- canonical weekly metadata and integrity anchor.

- incidents.csv --- canonical weekly incident dataset.

- taxonomy_report.md --- taxonomy analytics and classification output.

- prevention_report.md --- normalized prevention-action output.

- governance_notes.md --- non-canonical governance observations for
  future review.

**Artifact Registry**

  -------------------------------------------------------------------------------
  **Artifact**           **Role**          **Authority   **Primary Use**
                                           Level**       
  ---------------------- ----------------- ------------- ------------------------
  manifest.md            Weekly metadata   Canonical     Scope, traceability,
                         and integrity                   generation metadata, and
                         anchor                          dataset integrity

  incidents.csv          Weekly incident   Canonical     Structured incident
                         dataset                         records used by
                                                         downstream processing

  taxonomy_report.md     Taxonomy          Analytical    Classification
                         analytics output                distribution, integrity
                                                         checks, and taxonomy
                                                         visibility

  prevention_report.md   Prevention        Analytical    Standardized
                         normalization                   prevention-action
                         output                          coverage and
                                                         traceability

  governance_notes.md    Governance        Advisory      Recording governance
                         observation                     friction and signals for
                         record                          future review
  -------------------------------------------------------------------------------

**Navigation**

- [manifest.md](https://chatgpt.com/c/manifest.md)

- [incidents.csv](https://chatgpt.com/c/incidents.csv)

- [taxonomy_report.md](https://chatgpt.com/c/taxonomy_report.md)

- [prevention_report.md](https://chatgpt.com/c/prevention_report.md)

- [governance_notes.md](https://chatgpt.com/c/governance_notes.md)

**Repository Topology**

The weekly folder represents the aggregation layer for the reporting
period.

Canonical incident records provide the atomic incident layer from which
the weekly structured dataset is assembled.

The weekly analytical artifacts provide deterministic taxonomy and
prevention outputs derived from the structured dataset.

Governance artifacts provide a separate advisory layer for recording
classification, taxonomy, prevention-mapping, or integrity signals
without modifying canonical records or analytical outputs.

Publication and visualization artifacts, where present, form the
presentation layer and remain separate from canonical incident data and
weekly metadata.

**Incident Traceability**

Weekly aggregation is anchored by manifest.md, which identifies the
reporting period and provides the ordered incident identifiers
associated with the package.

The identifiers provide the traceability path between the weekly
aggregation layer and the corresponding atomic incident records.

**Suggested Navigation Order**

1.  manifest.md --- confirm weekly scope, traceability, and integrity
    metadata.

2.  incidents.csv --- access the canonical structured incident dataset.

3.  taxonomy_report.md --- review taxonomy analytics and classification
    integrity.

4.  prevention_report.md --- review normalized prevention-action output.

5.  governance_notes.md --- review advisory governance signals.

6.  Publication and visualization artifacts --- inspect presentation
    outputs where present.

**Processing Integrity**

This README is informational and non-canonical.

Canonical weekly metadata authority resides in manifest.md, while
incident-level authority resides in the canonical incident records and
structured weekly dataset. Analytical authority resides in the
referenced analytical outputs.

This README provides orientation and navigation only. It does not
compute, normalize, classify, reinterpret, or authoritatively summarize
incidents.
