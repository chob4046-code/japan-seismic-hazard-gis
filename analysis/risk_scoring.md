# Seismic Exposure Index

This framework is a portfolio demonstration model. It is not an official Japanese risk standard.

## Formula

`SEI = 0.40H + 0.20G + 0.20P + 0.10I + 0.10F`

Where:

- `H` = normalized seismic hazard
- `G` = normalized ground amplification / ground-condition indicator
- `P` = normalized population exposure
- `I` = normalized critical-infrastructure exposure
- `F` = normalized contextual fault-proximity score

Each component is scaled to 0–1 before combination.

## Interpretation

| Index | Screening class |
|---:|---|
| 0.00–0.24 | Low |
| 0.25–0.49 | Moderate |
| 0.50–0.74 | High |
| 0.75–1.00 | Very High |

The thresholds are project-defined and should be tested with sensitivity analysis before any substantive interpretation.
