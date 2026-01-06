# Contributing to the Crypto Safety Incident Dataset

Thank you for your interest in contributing to the Crypto Safety Incident Dataset.

This repository is a **curated, structured, OSINT-based dataset** of real-world crypto
security incidents. Contributions are welcome, but they must follow **strict rules**
to preserve data quality, consistency, and long-term usefulness.

This is **not** a discussion forum or news feed.  
It is a **version-controlled incident database**.

---

## 1. What Qualifies as an Incident

An incident **must** meet all of the following criteria:

- Represents a **real-world crypto or Web3 security event**
- Is supported by **publicly accessible sources**
- Involves one of:
  - Scams
  - Hacks
  - User mistakes resulting in loss or risk
- Can be classified using the **locked taxonomy** defined in `schema.md`

The following do **not** qualify:
- Hypothetical scenarios
- Rumors or unverified claims
- General warnings without a specific incident
- Pure opinion or speculation
- Marketing content

---

## 2. Source Requirements

Every incident must include at least **one credible source URL**, such as:

- Reddit posts or comments
- X / Twitter threads
- News articles
- Official disclosures
- User reports with sufficient detail

Sources must be:
- Publicly accessible
- Relevant to the incident described
- Directly supportive of the summary

Do **not** submit incidents based solely on private messages or unverifiable claims.

---

## 3. Schema Compliance (MANDATORY)

All contributions **must strictly follow** the schema defined in `schema.md`.

This includes:
- Exact field names
- Exact field order
- Allowed values only
- Locked incident types and subtypes
- Explicit handling of ambiguity via `classification_warning`

Submissions that do not conform to the schema will be rejected.

---

## 4. Taxonomy Rules (STRICT)

The taxonomy is **locked**.

You may **not**:
- Invent new incident types
- Invent new subtypes
- Rename existing categories
- Combine multiple subtypes in one record

If an incident does not cleanly fit the taxonomy:
- Classify it using the closest valid option
- Set `classification_warning` accordingly

Ambiguity should be **flagged, not hidden**.

---

## 5. Incident IDs

Incident IDs follow the format:

INC-YYYYMMDD-XXX

Rules:
- IDs generated during ingestion are **provisional**
- Canonical uniqueness is enforced externally (e.g., by GitHub filename)
- IDs may be renumbered during review before merge
- The GitHub filename is the canonical ID reference

Do not assume your submitted ID will remain unchanged.

---

## 6. Writing Standards

### Summary
- 1–3 sentences
- Plain, neutral language
- Describe **who / what / how**
- Focus on the mechanism, not emotion
- No speculation or assumptions

### User Mistake
- Describe the **single primary decision** that enabled the incident
- If unclear, use `none_obvious`

### Prevention
- 1–2 actions maximum
- Imperative phrasing
- Practical and specific
- Do not include vague advice

---

## 7. Pull Request Process

1. Fork the repository
2. Add or modify incident records following `schema.md`
3. Ensure your changes are minimal and focused
4. Open a pull request with:
   - A brief description of the incident(s)
   - Source links
   - Any classification uncertainty explained

All pull requests are reviewed manually.

Review may include:
- Schema validation
- Taxonomy consistency checks
- Comparison with existing incidents
- Requests for clarification or revision

---

## 8. Editorial Standards

This dataset prioritizes:
- Accuracy over speed
- Clarity over completeness
- Evidence over interpretation

Records may be edited, corrected, or archived over time.
All changes must occur via commit history — **no silent edits**.

---

## 9. What This Repository Is — and Is Not

**This repository is:**
- A curated incident database
- An educational and analytical resource
- A foundation for downstream analytics and prevention research

**This repository is not:**
- A blacklist
- A real-time alerting system
- A customer support channel
- A law-enforcement attribution database

---

## 10. Code of Conduct

Be respectful, factual, and professional.

Personal attacks, harassment, or inflammatory language are not acceptable and may
result in contribution privileges being revoked.

---

Thank you for helping keep this dataset accurate, useful, and trustworthy.
