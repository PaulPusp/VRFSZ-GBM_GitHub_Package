# Data provenance and claim boundaries

## DeltaDTM

The analysis uses paired DeltaDTM representations on an exact common source grid. The native
representation used during the project came from a third-party Earth Engine mirror. Exact grid
compatibility does not by itself prove cell-value equivalence to the official native release.

Required framing: **paired-product comparison** unless official-source equivalence is independently demonstrated.

## Sentinel-1

The frozen flood classifier uses VV/VH dB change with equal weights and an event-specific Otsu
threshold under one common algorithm. Permanent water is excluded using JRC Global Surface Water.
DEM/VRFSZ information is not used to tune or classify the Sentinel-1 flood masks.

## External corroboration

GFDS is retained only as coarse independent passive-microwave corroboration and is not used for
10 m flood-mask accuracy. GloFAS, CYGNSS and gauge branches that did not yield consistent
analysis-ready event-matched observations are not promoted to final quantitative validation.
