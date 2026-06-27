**README --- CW25 + CW26 2026**

**Week Identifier**

**CW25 + CW26 2026**

------------------------------------------------------------------------

**Purpose**

This folder contains the weekly aggregation package for the reporting
period. It provides the canonical metadata, normalized incident dataset,
publication artifacts, governance documentation, and supporting
materials required for review, publication, and repository navigation.

------------------------------------------------------------------------

**Folder Contents Overview**

- **manifest.md** --- Weekly metadata anchor.

- **incidents.csv** --- Canonical normalized incident dataset.

- **taxonomy_report.md** --- Dataset taxonomy classification report.

- **prevention_report.md** --- Prevention action normalization report.

- **governance_notes.md** --- Weekly governance observations.

- **Visualization assets** --- Supporting publication graphics and
  figures (if present).

------------------------------------------------------------------------

**Artifact Registry**

  ----------------------------------------------------------------------------
  **Artifact**           **Role**           **Authority**       **Primary
                                                                Audience**
  ---------------------- ------------------ ------------------- --------------
  manifest.md            Weekly metadata    Canonical           Analysts,
                         anchor                                 Automation

  incidents.csv          Canonical incident Canonical           Analysts,
                         dataset                                Automation

  taxonomy_report.md     Taxonomy analytics Canonical           Analysts,
                                            publication         Editors
                                            artifact            

  prevention_report.md   Prevention         Canonical           Analysts,
                         normalization      publication         Editors
                                            artifact            

  governance_notes.md    Governance         Advisory            Analysts,
                         observations                           Reviewers

  Visualization assets   Publication        Informational       Editors,
                         support material                       Publication
  ----------------------------------------------------------------------------

------------------------------------------------------------------------

**Navigation**

Recommended entry points:

- manifest.md

- incidents.csv

- taxonomy_report.md

- prevention_report.md

- governance_notes.md

- visualization assets (if available)

------------------------------------------------------------------------

**Repository Topology**

The weekly folder contains aggregation-level artifacts for the reporting
period.

Atomic incident records are maintained separately within the incident
repository.

Publication artifacts are generated from the canonical weekly dataset.

Governance documentation accompanies the weekly package as an advisory
layer.

Supporting visualization assets, where available, are maintained
alongside the publication artifacts.

------------------------------------------------------------------------

**Incident Traceability**

The weekly aggregation package references normalized incident records
contained within the canonical dataset.

Each weekly artifact is traceable to the corresponding atomic incident
records maintained within the incident repository.

**Suggested Navigation Order**

1.  manifest.md

2.  incidents.csv

3.  taxonomy_report.md

4.  prevention_report.md

5.  governance_notes.md

6.  Visualization assets

------------------------------------------------------------------------

**Processing Integrity Statement**

This README is provided for orientation and navigation purposes only.

Canonical authority resides in **manifest.md** and the referenced
canonical publication artifacts.

This document does not compute, normalize, classify, summarize, or
interpret incident data and does not supersede any canonical artifact.
