# CW29 + CW30 2026

## Purpose

This folder contains the weekly aggregation package for **CW29 + CW30 2026**. It provides the canonical weekly dataset together with publication, governance, and supporting artifacts used for navigation, review, and publication. This document is an orientation guide only and does not serve as a source of analytical authority.

---

## Folder Contents

- **manifest.md** — Canonical weekly metadata anchor.
- **incidents.csv** — Canonical weekly incident dataset.
- **taxonomy_report.md** — Taxonomy analytics report.
- **prevention_report.md** — Prevention action normalization report.
- **governance_notes.md** — Governance observations for the weekly package.
- **Visualization assets** — Publication graphics and supporting visual material (when present).

---

## Artifact Registry

| Artifact | Role | Authority | Intended Audience |
|---|---|---|---|
| manifest.md | Weekly metadata anchor | Canonical | Analysts, Automation |
| incidents.csv | Weekly incident dataset | Canonical | Analysts, Automation |
| taxonomy_report.md | Taxonomy analytics | Canonical analytical output | Analysts, Reviewers |
| prevention_report.md | Prevention normalization | Canonical analytical output | Analysts, Reviewers |
| governance_notes.md | Governance observations | Advisory | Analysts, Editors |
| Visualization assets | Publication support | Informational | Editors, Publication |

---

## Navigation

- manifest.md
- incidents.csv
- taxonomy_report.md
- prevention_report.md
- governance_notes.md
- Visualization assets (if present)

---

## Repository Structure

The weekly folder groups together the canonical dataset, publication artifacts, governance documentation, and supporting materials for a single reporting period.

Atomic incident records remain separate from the weekly aggregation package. Publication artifacts are generated from the canonical dataset, while governance documents provide operational context without modifying canonical records.

---

## Incident Traceability

The weekly aggregation package is derived from normalized atomic incident records. Weekly artifacts reference those records for traceability while preserving the separation between incident-level data and weekly publication materials.

---

## Suggested Navigation Order

1. manifest.md
2. incidents.csv
3. taxonomy_report.md
4. prevention_report.md
5. governance_notes.md
6. Visualization assets (if present)

---

## Processing Integrity

This README is informational and non-canonical.

Canonical authority resides in **manifest.md** and the referenced publication artifacts.

This document does not compute, normalize, classify, summarize, or reinterpret incident data. It exists solely to support navigation and orientation within the weekly package.
