# Alabama Intense Rainfall & Flood Fact Sheet

A reproducible statewide screening project examining where intense rainfall and flood impacts are concentrated across Alabama.

## Project purpose

This repository organizes the data-processing workflow, notebooks, outputs (maps, figures, derived tables, and final fact sheet) for the Alabama intense-rainfall and flood analysis.

The fact sheet summarizes:
- Long-term intense-rainfall patterns across Alabama HUC-12 watersheds.
- Rainfall rarity relative to NOAA Atlas 14 precipitation-frequency benchmarks.
- Major flood-producing storms linked to USGS streamgages.
- Reported flood and flash-flood hotspots.
- Top statewide rainfall events and rainfall accumulation by duration.
- Seasonality, storm attribution, and rainfall-to-river response timing.

## Repository structure

```text
alabama-intense-rainfall-flood-fact-sheet/
|-- README.md
|-- .gitignore
|-- environment.yml
|-- requirements.txt
|-- data/
|   |-- raw/
|   |-- external/
|   |-- interim/
|   `-- processed/
|-- notebooks/
|-- config/
|-- metadata/
|-- outputs/
|   |-- figures/
|   |-- maps/
|   |-- tables/
|   `-- fact_sheet/
|-- docs/
|   |-- methodology/
|   `-- references/
`-- dashboard/
```

## Main data sources

- NOAA Analysis of Record for Calibration (AORC) precipitation
- NOAA Atlas 14 precipitation-frequency estimates
- USGS annual peak streamflow and streamgage records
- NOAA Storm Events
- NOAA HURDAT2 tropical-cyclone tracks
- Alabama HUC-12 watershed boundaries

## Data policy

Do not commit large raw precipitation, radar, streamflow, NetCDF, Zarr, or GIS archives directly to GitHub. Keep those on local/HPC storage and commit only small reproducibility samples, compact processed summaries, metadata, download manifests, scripts, notebooks, and documentation.

## Recommended workflow

1. Keep source-data manifests under `metadata/`.
2. Store exploratory and sequential analysis in `notebooks/`.
3. Move reusable functions into `src/`.
4. Put one-off download and batch-processing utilities in `scripts/`.
5. Save publication-ready figures, maps, and tables under `outputs/`.
6. Keep final fact-sheet products under `outputs/fact_sheet/`.
7. Document methods, assumptions, and limitations under `docs/methodology/`.

## Final fact sheet

[`outputs/fact_sheet/Alabama_Intense_Rainfall_Flood_Fact_Sheet_3page.pdf`](outputs/fact_sheet/Alabama_Intense_Rainfall_Flood_Fact_Sheet_3page.pdf)

## Author

Ismail Olajide  
University of Alabama / Alabama Water Institute

## Before publishing

Check notebooks and configuration files for hard-coded local paths, API keys, access tokens, personal credentials, large outputs, and redistribution-restricted datasets.
