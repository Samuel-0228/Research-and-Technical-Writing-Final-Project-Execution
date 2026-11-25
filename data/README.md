# Data Directory & Management Protocols

This directory contains data management protocols, codebook mappings, and segregated storage for raw and cleaned research data.

---

## Directory Organization

```
data/
├── raw/ # Raw, unmodified survey export files (CSV/Excel) - Phase 3
├── processed/ # Cleaned, validated, and coded data files - Phase 3/4
├── codebook.md # Comprehensive data dictionary and coding schema (Phase 3)
└── README.md # Data management plan, ethics, and anonymization guide
```

---

## Data Protection & Anonymization Standards

1. **No Personally Identifiable Information (PII):** The survey does not collect names, email addresses, student identification numbers, phone numbers, or IP addresses.
2. **De-identification of Open-Ended Responses:** Any mention of specific instructor names or student identities in the qualitative text area is stripped and replaced with generic tokens (e.g., `[Instructor A]`, `[Department Head]`) prior to placing files in `processed/`.
3. **Immutability of Raw Data:** Files inside `raw/` remain unaltered as the single source of truth. All cleaning, imputations, dummy encoding, and scale transformations are programmatically executed via `analysis/analysis_pipeline.py` and output to `processed/`.
4. **Public Archiving Ethics:** In accordance with course guidelines and the Institutional Ethics Statement, only anonymized datasets are published to the repository.
