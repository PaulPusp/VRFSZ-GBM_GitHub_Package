# Reproducibility notes

The public repository is notebook-first and has one canonical code artifact:

`notebooks/MASTER_VRFSZ_GBM_REPRODUCIBILITY.ipynb`

## Frozen inferential design

- primary threshold: 1 m;
- sensitivity thresholds: 0.5 and 2 m;
- primary block width: 80 km;
- original 1 km sufficient-statistic lattice;
- active block rule: either VRFSZ or Stable High has at least one valid cell-event observation;
- primary bootstrap: 2,000 paired block resamples;
- robustness: 40/60/80/100/120 km × four fixed origins × 5,000 resamples;
- minimum inferential block count: 20;
- seed: 20260830.

## Expected primary result

At T = 1 m, corrected pooled RR ≈ 0.9681 with 95% spatial block-bootstrap CI ≈ 0.8702–1.0610.

If a fresh execution materially departs from the frozen result, stop and inspect the input/event
state before interpreting the output.
