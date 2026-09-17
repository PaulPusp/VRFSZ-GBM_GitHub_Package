# Data layout

Large datasets are not stored in GitHub.

The master notebook expects a project data tree beneath `data/`, including the frozen GBM
Delta boundary, paired DeltaDTM terrain representations, Sentinel-1 pre/event imagery,
JRC permanent-water information, and corrected event flood/valid masks for downstream-only reruns.

The acquisition stages can rebuild many inputs when provider access and credentials are available.

Do not upload credentials, tokens, or private data.
