**README --- CW33 + CW34 2026**

**Weekly Package**

**Reporting period:** CW33 + CW34 2026

This folder contains the weekly aggregation, analytical publication
outputs, governance material, and supporting artifacts for the reporting
period.

The README provides orientation and navigation only. It does not
independently compute, classify, normalize, or interpret incident data.

**Folder Contents**

  ---------------------------------------------------------------------------
  **Artifact**           **Role**                          **Authority
                                                           Level**
  ---------------------- --------------------------------- ------------------
  manifest.md            Weekly metadata and scope anchor  Canonical

  incidents.csv          Weekly aggregated incident        Canonical
                         dataset                           

  taxonomy_report.md     Taxonomy analysis and publication Canonical
                         output                            analytical output

  prevention_report.md   Prevention action normalization   Canonical
                         and publication output            analytical output

  governance_notes.md    Governance observations and       Advisory
                         review signals                    

  Visualization assets   Publication renderings derived    Publication layer
                         from approved outputs             
  ---------------------------------------------------------------------------

The reporting-period identifier used throughout the package is CW33 +
CW34 2026.

**Artifact Registry**

  ---------------------------------------------------------------------------
  **Artifact**           **Purpose**              **Intended Use**
  ---------------------- ------------------------ ---------------------------
  manifest.md            Establish weekly scope   Integrity verification and
                         and metadata             package identification

  incidents.csv          Preserve the aggregated  Incident-level traceability
                         incident records         and analytical processing

  taxonomy_report.md     Present taxonomy         Analytical and publication
                         analysis                 review

  prevention_report.md   Present normalized       Analytical and publication
                         prevention-action        review
                         analysis                 

  governance_notes.md    Record governance        Governance review
                         signals                  

  Visualization assets   Present approved         Publication and
                         information visually     distribution
  ---------------------------------------------------------------------------

The prevention report identifies itself as covering the CW33 + CW34
incident dataset. The governance artifact likewise identifies CW33 +
CW34 as its reporting scope.

**Navigation**

- manifest.md --- start here for weekly scope and metadata.

- incidents.csv --- use for the aggregated incident records.

- taxonomy_report.md --- use for taxonomy analysis.

- prevention_report.md --- use for prevention-action analysis.

- governance_notes.md --- use for advisory governance observations.

- Visualization assets --- use for publication-ready visual
  representations where present.

**Repository Topology**

The repository separates atomic incident records, weekly aggregation,
analytical outputs, governance material, and publication renderings.

**Incident layer** contains normalized atomic incident records used for
traceability.

**Weekly aggregation layer** groups the applicable incident records for
the reporting period and establishes the weekly package.

**Analytical layer** contains taxonomy and prevention outputs generated
from the weekly dataset.

**Governance layer** contains advisory observations relating to
classification, taxonomy, prevention mapping, or processing integrity.
Governance notes do not modify canonical records or analytical outputs.

**Publication layer** contains approved renderings and visualization
assets derived from the relevant publication outputs.

**Incident Traceability**

Weekly aggregation artifacts maintain a relationship to their underlying
atomic incident records. incidents.csv provides the weekly aggregation
dataset, while manifest.md establishes the scope and metadata anchor for
the package.

Incident-level records remain the appropriate layer for tracing
individual incidents. Weekly analytical and publication artifacts do not
replace those atomic records.

**Suggested Navigation Order**

For general package review:

1.  manifest.md

2.  incidents.csv

3.  taxonomy_report.md

4.  prevention_report.md

5.  governance_notes.md

6.  Visualization and publication assets

For publication review, begin with the relevant analytical output and
then inspect its corresponding rendering or visualization.

For governance review, use the manifest and canonical outputs as the
authoritative reference before consulting governance_notes.md.

**Processing Integrity**

This README is informational and non-canonical.

Canonical authority resides in the weekly metadata anchor, incident
dataset, and referenced analytical outputs. Governance notes remain
advisory.

The README does not compute metrics, normalize prevention actions,
classify incidents, reinterpret analytical results, or independently
summarize the incident dataset.
