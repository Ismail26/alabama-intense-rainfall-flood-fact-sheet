# Complete pipeline outputs

This directory preserves the complete output trees from the two analysis pipelines:

- `13_atlas14_event_catalog/` - Atlas 14 storm-event catalog pipeline
- `14_flood_response/` - integrated rainfall-flood response pipeline

These folders include final products as well as inventories, downloaded public-data caches, checkpoints, logs, intermediate data, spatial layers, and duplicate files present in the original output trees. The smaller curated publication products remain available in `outputs/atlas14_event_catalog/` and `outputs/flood_response/`.

Large scientific and binary formats (`.asc`, `.gpkg`, `.tif`, `.parquet*`, and `.png`) are stored with Git LFS. Install Git LFS and run `git lfs pull` after cloning to retrieve their contents. GitHub-generated ZIP archives may contain LFS pointer files unless the repository setting to include LFS objects in archives is enabled.
