# Crypto Safety Incident Dataset — GitHub Schema (v1)

This document defines the **canonical schema** for the Crypto Safety Incident Dataset
hosted in this GitHub repository.

The dataset is built using a **three-stage processing pipeline**:

1. **Stage 0 — Incident Text → CSV Row (Primary Ingest)**
2. **Stage 1 — Taxonomy Analytics (Scams / Hacks / User Mistakes)**
3. **Stage 2 — Prevention Action Normalization**

This repository stores the **structured records** of Stage 0 and serves as the
authoritative, version-controlled source of truth for curated incidents.

---

## 1. Design Principles

- One incident = one structured record
- Taxonomy is **locked and non-extensible**
- IDs are **human-readable and date-based**
- Classification uncertainty is **explicitly surfaced**
- Dataset favors **correctness and auditability over completeness**

This dataset is **OSINT-based** and **confidence-scored**.  
It is not a law-enforcement or forensic attribution system.

---

## 2. Canonical Record Format (CSV-Derived)

Each incident record originates from a **single CSV row** produced by the
Stage 0 ingestion prompt.

### Required Fields (Exact Order)

| # | Field Name | Description |
|---|------------|-------------|
| 1 | `id` | Provisional incident ID |
| 2 | `first_observed_date` | Date first publicly observed (YYYY-MM-DD) |
| 3 | `incident_type` | High-level category |
| 4 | `incident_subtype` | Locked subtype |
| 5 | `source_name` | Auto-detected source |
| 6 | `source_url` | Original report URL |
| 7 | `summary` | 1–3 sentence mechanism-focused summary |
| 8 | `user_mistake` | Primary enabling decision |
| 9 | `prevention` | 1–2 prevention actions |
|10 | `classification_warning` | Explicit ambiguity flag |

---

## 3. Incident ID Rules

### Format

INC-YYYYMMDD-XXX

### Rules

- `YYYYMMDD` MUST match `first_observed_date`
- Sequence (`XXX`) starts at `001` per date
- IDs generated during ingestion are **provisional**
- **Canonical uniqueness is enforced externally**
  (e.g., GitHub filename, spreadsheet, or dataset review)
- Provisional IDs may be renumbered before commit

The **GitHub filename is the canonical ID reference**.

---

## 4. Allowed `incident_type` (LOCKED)

Exactly **one** per record:

- `scam`
- `hack`
- `user_mistake`

### Classification Precedence

1. Deception or manipulation → `scam`
2. Technical compromise without user approval → `hack`
3. No attacker involvement → `user_mistake`

If ambiguous between scam and hack → **default to `scam`**.

---

## 5. Allowed `incident_subtype` (LOCKED)

### 5.1 Hacks (choose ONE)

- social_engineering_hack
- malware
- trojan
- spyware
- keylogger
- clipboard_hijacker
- ransomware
- cryptojacking
- network_mitm
- wifi_sniffing
- dns_spoofing
- session_hijacking
- ssl_stripping
- fake_app_or_extension_hack
- exchange_vulnerability
- insider_attack
- wallet_software_exploit

Rules:
- Use **initial access vector**
- Fake apps/extensions are hacks **only if malware executes**
- SIM swap is **not** a hack

---

### 5.2 Scams (choose ONE)

- social_engineering
- phishing
- social_media_scam
- crypto_wallet_scam
- smart_contract_scam
- fake_app_or_extension
- exchange_scam
- token_launch_scam
- pump_dump
- rug_pull
- airdrop_scam
- nft_scam
- sim_swap
- job_scam
- blackmail_extortion
- romance_scam

Rules:
- If user approved, signed, sent, or shared → scam
- Impersonation, fake support, deepfakes → scam

---

### 5.3 User Mistakes (choose ONE)

- wrong_address
- wrong_network
- seed_phrase_exposure
- approval_misunderstanding
- backup_failure
- address_poisoning_copy_paste
- lost_wallet_access
- poor_wallet_backup_practice

Rules:
- No attacker involvement
- If attacker exists → do not use `user_mistake`

---

## 6. Field Content Rules

### `summary`

- 1–3 sentences
- Who / what / how
- Mechanism-focused
- No speculation

### `user_mistake`

- Single primary decision
- If unclear → `none_obvious`

### `prevention`

- 1–2 actions maximum
- Imperative phrasing
- Practical and specific

### `classification_warning`

- `none` if clean classification
- Short warning (≤10 words) if ambiguous

Examples:
- `mixed scam and technical vectors`
- `unclear attacker involvement`
- `insufficient detail to classify confidently`

---

## 7. Dataset Integrity Rules

- No new categories or subtypes may be added
- Ambiguity must be flagged, not hidden
- Rows with warnings remain valid but must be surfaced in analytics
- Corrections require commit history (no silent edits)

---

## 8. Relationship to Analytics & Prevention Layers

This schema feeds:

- **Taxonomy analytics**
  (scam / hack / user_mistake distributions with zero-fill)
- **Prevention action normalization**
  (standardized actions with coverage metrics)

All downstream analysis must rely **only on these fields**.

---

## 9. What This Dataset Is — and Is Not

**This dataset is:**
- Curated
- Deterministic
- Auditable
- Behavior-focused

**This dataset is not:**
- A blacklist
- A real-time alert feed
- A forensic attribution engine
- A guarantee of factual completeness

---

## 10. Versioning

- Schema version: `v1`
- Breaking changes require documentation
- Taxonomy changes are not permitted without formal migration

---

End of document.
