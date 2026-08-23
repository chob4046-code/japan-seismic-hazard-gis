# Methodology

## 1. Define the study question

Where do high seismic hazard and high human/infrastructure exposure overlap in Japan?

## 2. Prepare data

Use a consistent projected CRS for analysis, document source dates, inspect geometry, remove duplicates, and record metadata for every layer.

## 3. Standardize hazard indicators

Convert seismic-hazard values into comparable 0–1 scores. Higher hazard receives a higher score.

## 4. Add ground-condition information

Use J-SHIS site amplification or related subsurface/terrain information. Higher amplification receives a higher screening score.

## 5. Measure exposure

Intersect hazard meshes with population and critical-infrastructure layers. Summarize exposed population/facilities by analysis unit.

## 6. Fault proximity

Create distance bands around selected active faults or seismic-source features. Use this only as a contextual indicator; proximity to a mapped fault is not a prediction of earthquake occurrence or damage.

## 7. Weighted overlay

Combine normalized indicators using documented weights. The example model in the README is intentionally illustrative.

## 8. Validate and communicate

Check the output against source metadata, inspect extreme values, document assumptions, and clearly label the result as a screening index rather than an official hazard or engineering map.
