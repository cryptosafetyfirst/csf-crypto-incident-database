**README --- CW27 + CW28 2026**

**Weekly Package**

This directory contains the publication package for **CW27 + CW28
2026**. It provides the canonical weekly dataset together with
publication outputs, governance documentation, and supporting artifacts
intended for review, publication, and repository navigation. The weekly
scope, generation metadata, and artifact integrity are defined by the
manifest.

------------------------------------------------------------------------

**Folder Contents**

  -------------------------------------------------------------------------
  **Artifact**           **Role**
  ---------------------- --------------------------------------------------
  manifest.md            Weekly metadata anchor defining scope,
                         identifiers, generation metadata, and artifact
                         integrity.

  incidents.csv          Canonical normalized incident dataset for the
                         reporting period.

  taxonomy_report.md     Publication report describing normalized taxonomy
                         outputs.

  prevention_report.md   Publication report describing normalized
                         prevention actions.

  governance_notes.md    Advisory governance observations recorded during
                         weekly processing.

  visualizations/ *(if   Publication graphics and rendered visual assets.
  present)*              
  -------------------------------------------------------------------------

------------------------------------------------------------------------

**Artifact Registry**

  ---------------------------------------------------------------------
  **Artifact**           **Purpose**                 **Authority**
  ---------------------- --------------------------- ------------------
  manifest.md            Weekly metadata and         Canonical
                         traceability                

  incidents.csv          Canonical incident records  Canonical

  taxonomy_report.md     Taxonomy publication output Canonical
                                                     Publication

  prevention_report.md   Prevention publication      Canonical
                         output                      Publication

  governance_notes.md    Governance observations     Advisory

  Visualization assets   Publication support         Informational
                         material                    
  ---------------------------------------------------------------------

------------------------------------------------------------------------

**Navigation**

Recommended entry points:

1.  manifest.md

2.  incidents.csv

3.  taxonomy_report.md

4.  prevention_report.md

5.  governance_notes.md

6.  Visualization assets (if available)

------------------------------------------------------------------------

**Repository Structure**

This weekly package forms part of the repository\'s aggregation layer.

The repository is organized into:

- Atomic incident records

- Weekly aggregation datasets

- Publication outputs

- Governance documentation

- Visualization assets

Each layer serves a distinct operational role while remaining
structurally linked through the weekly package.

------------------------------------------------------------------------

**Incident Traceability**

The weekly dataset is produced from normalized atomic incident records
collected during the reporting period. The manifest provides the
authoritative list of incident identifiers included within the weekly
aggregation package, ensuring end-to-end traceability between the weekly
dataset and individual incident records.

------------------------------------------------------------------------

**Suggested Review Order**

For operational review, the recommended sequence is:

1.  Manifest

2.  Incident dataset

3.  Taxonomy report

4.  Prevention report

5.  Governance notes

6.  Visualization assets

------------------------------------------------------------------------

**Processing Integrity**

This README is provided solely for orientation and repository
navigation.

It does not compute, classify, normalize, summarize, or interpret
incident data. Canonical authority resides in the manifest, the incident
dataset, and the referenced publication artifacts.
