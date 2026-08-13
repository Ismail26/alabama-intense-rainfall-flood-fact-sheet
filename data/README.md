# Data

- `raw/`: selected original source-data folders committed for project reproducibility; archived binary files use Git LFS.
- `external/`: supporting third-party datasets; generally excluded if large.
- `interim/`: intermediate processing outputs; generally excluded.
- `processed/`: compact analysis-ready products that may be committed when reasonably small.

Each derived dataset should document its source, processing date, generating notebook/script, and variable definitions.
