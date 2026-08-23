# Reproducibility Guide

1. Download the selected official J-SHIS datasets and record their version/date.
2. Store original files under `data/raw/` without modification.
3. Perform cleaning and transformations into `data/processed/`.
4. Open the QGIS project from `qgis/` and verify layer sources.
5. Apply the documented normalization and weighted-overlay rules.
6. Export final maps into `maps/`.
7. Record any changes to weights, thresholds, CRS, or source datasets in the project notes.

## Reproducibility principle

The repository should never contain an undocumented numerical result. Every map or index should be traceable to a source dataset, processing step, and modelling assumption.
