# QGIS Workflow

## Recommended layer order

1. Basemap / Japan boundary
2. Administrative boundaries
3. Seismic hazard mesh
4. Site amplification
5. Active faults
6. Population exposure
7. Roads and railways
8. Critical facilities
9. Final Seismic Exposure Index

## Core QGIS operations

- Add vector/raster layers
- Reproject layers where required
- Clip to the study area
- Join attributes by spatial location
- Create fault buffers/distance surfaces
- Rasterize or aggregate indicators when appropriate
- Normalize indicators to 0–1
- Calculate the weighted index with Field Calculator or raster algebra
- Classify the final index into four screening classes
- Compose a map with legend, scale bar, north arrow, source notes, and disclaimer

The `.qgz` project should be created only after the actual source datasets are downloaded and their paths are known.
