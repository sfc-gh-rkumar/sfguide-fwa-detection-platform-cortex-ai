# FWA Detection Platform with Snowflake Cortex AI — Sample Files

Companion files for the Snowflake Developer Guide
**Build a Fraud, Waste, and Abuse Detection Platform with Snowflake Cortex AI**.

All files are **synthetic** and created for demonstration only. They contain no real patient, provider, or claims information.

| Path | Purpose |
|---|---|
| `data/documents/claim_C3002_invoice.pdf` | Invoice billing 99215 for a 12-minute follow-up (upcoding signal) |
| `data/documents/claim_C3003_clinical_notes.pdf` | Clinical note documenting a low-complexity visit billed as 99215 |
| `data/documents/claim_C3013_procedure_report.pdf` | Procedure report with a different CPT/diagnosis than claimed and no patient check-in (phantom billing signal) |
| `data/audio/hotline_call_20240201.mp3` | Synthetic fraud-hotline call about provider P-1001 |
| `data/audio/whistleblower_report_20240315.mp3` | Synthetic whistleblower report about providers P-1002 / P-1003 |
| `semantic_model/fwa_semantic_model.yaml` | Semantic model used by the Investigation Agent's Cortex Analyst tool |

The guide loads these files into Snowflake stages directly from this repository using a Snowflake Git repository, so no local download is needed.

Author: Ravi Kumar, Partner Solutions Architect
