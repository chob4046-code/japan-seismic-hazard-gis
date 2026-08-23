# Japan Seismic Hazard & Exposure GIS

A QGIS-based disaster-risk mapping project for Japan that combines seismic hazard, ground amplification, population exposure, faults, and critical infrastructure into a reproducible spatial-analysis workflow.

## Project goal

Build a transparent **Seismic Exposure Index** that demonstrates how GIS can connect earthquake hazard with people and infrastructure. This is an educational screening workflow, not an engineering safety assessment or an earthquake prediction system.

## Core workflow

```text
Seismic hazard
      +
Ground amplification / terrain
      +
Population exposure
      +
Critical infrastructure
      ↓
Standardize indicators
      ↓
Weighted overlay
      ↓
Seismic Exposure Index
      ↓
Low / Moderate / High / Very High
```

## Data strategy

The preferred authoritative source is **J-SHIS (Japan Seismic Hazard Information Station)** operated by the National Research Institute for Earth Science and Disaster Resilience (NIED). J-SHIS provides probabilistic seismic hazard maps, scenario earthquake shaking maps, fault coordinates, site amplification factors, subsurface structure data, and exposed-population statistics.

Reference: https://www.j-shis.bosai.go.jp/en/downloads

J-SHIS also provides a web API that can return seismic-hazard mesh information as GeoJSON, including probabilities of exceeding specified seismic-intensity levels.

Reference: https://www.j-shis.bosai.go.jp/en/api-pshm-meshinfo

## Planned layers

- Japan administrative boundary
- Probabilistic seismic hazard mesh
- Scenario earthquake shaking
- Active faults / seismic source faults
- Site amplification factor
- Historical earthquake observations where appropriate
- Population exposure
- Roads and railways
- Hospitals and other critical facilities
- Optional tsunami/coastal exposure layer

## Analysis

The project will demonstrate:

1. CRS and spatial-data preparation
2. Raster/vector layer integration
3. Hazard classification
4. Proximity analysis around faults
5. Population exposure calculation
6. Critical-infrastructure exposure analysis
7. Weighted-overlay modelling
8. Map composition and export

### Example scoring framework

| Indicator | Weight |
|---|---:|
| Seismic hazard | 40% |
| Ground amplification | 20% |
| Population exposure | 20% |
| Critical infrastructure exposure | 10% |
| Fault proximity | 10% |

Weights are illustrative and should be treated as a modelling choice, not an official Japanese risk standard.

## Repository structure

```text
japan-seismic-hazard-gis/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── qgis/
├── maps/
├── analysis/
└── docs/
```

## Important limitation

A GIS screening index cannot predict when or where an earthquake will occur. It also cannot replace structural engineering, official hazard assessments, evacuation planning, or site-specific investigations.

## Data attribution

When J-SHIS data are downloaded or reproduced, follow the J-SHIS terms and the attribution/citation requirements associated with the individual dataset.

## Status

**Portfolio project — methodology and repository structure established.** Official datasets should be downloaded and processed before presenting quantitative results as real-world findings.

## Author

[chob4046-code](https://github.com/chob4046-code)
