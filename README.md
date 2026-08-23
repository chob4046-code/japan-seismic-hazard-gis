# 🇯🇵 Japan Seismic Hazard & Exposure GIS

A QGIS-based portfolio project demonstrating earthquake-event and population-exposure screening for Japan, with an explicit integration path to official J-SHIS seismic-hazard data.

## Objective

Demonstrate how GIS can connect earthquake reference events, population exposure, and spatial proximity into a transparent screening workflow.

## Included outputs

- `data/historical_earthquakes.geojson` — curated historical earthquake reference points
- `data/cities_exposure.geojson` — city exposure screening points
- `data/exposure_results.json` — calculated screening results
- `data/jshis_api_reference.json` — official J-SHIS API integration reference
- `qgis/project.qgs` — QGIS project referencing the layers
- `maps/japan_seismic_exposure_map.svg` — portfolio map output
- `analysis/results.md` — interpretation and official-data upgrade path

## Screening method

The demonstration combines distance to a curated historical earthquake reference event with a population-proxy rank. It is intentionally **not** presented as an official seismic hazard model or earthquake prediction system.

## Official J-SHIS integration

J-SHIS/NIED provides probabilistic seismic hazard maps, scenario earthquake shaking maps, fault information, site amplification factors, subsurface structure information, and exposed-population statistics. The J-SHIS API can return 250 m seismic-hazard mesh information as GeoJSON. The repository records the 2024 API endpoint and `T30_I45_PS` attribute as the production-data integration target.

## QGIS workflow

1. Open `qgis/project.qgs`.
2. Inspect historical events and city exposure points.
3. Add official J-SHIS hazard mesh data.
4. Reproject layers into a suitable Japanese projected CRS.
5. Standardize hazard, ground-condition, population, and infrastructure indicators.
6. Build a documented weighted exposure index.
7. Validate the analysis and clearly separate hazard from exposure.
8. Export the final cartographic layout.

## Status

**Completed portfolio screening demonstration.** The repository now contains GIS data, a QGIS project, calculated results, a map output, and a documented route to official J-SHIS hazard integration.

## Safety / interpretation

This project does not predict earthquakes and does not replace structural engineering, official hazard assessments, evacuation planning, or site-specific investigations.

## Author

[chob4046-code](https://github.com/chob4046-code)
