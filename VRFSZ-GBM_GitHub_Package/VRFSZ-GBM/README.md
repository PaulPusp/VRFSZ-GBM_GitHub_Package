# VRFSZ–GBM

Reproducibility repository for the study of vertical-reference false-safe zones (VRFSZ)
in the Ganges–Brahmaputra–Meghna Delta using paired DeltaDTM representations and
Sentinel-1 flood evidence.

## Canonical code

All scientific code is consolidated into one notebook:

`notebooks/MASTER_VRFSZ_GBM_REPRODUCIBILITY.ipynb`

No secondary analysis notebook is required for the public code release.

## Final corrected scientific state

- Primary terrain threshold: **T = 1.0 m**
- Sensitivity thresholds: **0.5 m and 2.0 m**
- Corrected EVENT003 flood fraction: **0.205340**
- T = 0.5 m: RR **1.0031**, 95% CI **0.9025–1.0904**
- T = 1.0 m: RR **0.9681**, 95% CI **0.8702–1.0610**
- T = 2.0 m: RR **0.9003**, 95% CI **0.7769–1.0383**
- Final inference: **NO SUPPORT** for the predeclared positive VRFSZ–SAR flood-detection association.

`NO SUPPORT` means that the corrected analysis did not support the hypothesized positive
direction; it does not prove a causal negative effect or prove no association.

## Scientific boundaries

1. Unless official cell-value equivalence is separately demonstrated, the DeltaDTM analysis is a **paired-product comparison**.
2. The Sentinel-1 classifier is frozen before multi-event application and does not use DEM/VRFSZ information.
3. Missing SAR observations are not treated as dry.
4. GFDS is used only as **coarse independent passive-microwave corroboration**.
5. GloFAS, CYGNSS and gauge routes that did not yield analysis-ready event-matched evidence are not used as final quantitative validation.

## Repository structure

```text
VRFSZ-GBM/
├── README.md
├── requirements.txt
├── CITATION.cff
├── .gitignore
├── config/project_freeze.json
├── metadata/events.csv
├── metadata/provenance_table_TEMPLATE.csv
├── notebooks/MASTER_VRFSZ_GBM_REPRODUCIBILITY.ipynb
├── data/README.md
├── outputs/README.md
└── docs/
    ├── DATA_PROVENANCE.md
    └── REPRODUCIBILITY.md
```

## Environment

```bash
pip install -r requirements.txt
```

Acquisition cells may require authenticated access to Google Earth Engine or other data providers.

## Data

Large source/intermediate rasters are intentionally excluded from GitHub. See
`data/README.md` and `docs/DATA_PROVENANCE.md`.

## License

No software license has been selected in this package yet. Choose and add a license
before the public archival release if code reuse is intended.
