# Perturbed-Input

This project develops a standalone Python module capable of generating **perturbed input time series** for use in ensemble modelling workflows. The approach uses ARIMA modelling to characterize a time series, extracts residual errors, and resamples from those errors to produce statistically consistent perturbations of the original signal.

The project is structured as a sequence of six self-contained steps, each building directly on the last. By the end, we will have a well-documented, tested Python module suitable for inclusion in a larger modelling pipeline.

**Estimated Total Duration:** 7–8 weeks of core project work (full-time, ~35 hrs/week), leaving time for extensions, real-data validation and implementation in existing models, or a final technical report (which can lead to a full publication).

## Estimated/Suggested Timeline

This is just an estimated timeline, somethings may take less or more time depending on availability etc. It should not be taken to **heart**.

| Week | Stage | Daily Focus | Milestone |
|------|-------|-------------|-----------|
| 1 | Stage 1 | Reading (3 days) + environment setup + concept summary (2 days) | ARIMA theory solid; written summary complete |
| 2 | Stage 2 | Sine wave notebook (2 days) + noisy signal + diagnostics (3 days) | Residual diagnostic 4-panel function done |
| 3–4 | Stage 3 | Reading (2 days) + four sampling methods (4 days) + comparison plots (2 days) | `sampling_methods.py` complete; ensemble plots generated |
| 5 | Stage 4 | `auto_arima` fitting (2 days) + `arima_utils.py` functions (3 days) | Automated pipeline working on four test signals |
| 6–7 | Stage 5 | API design + `perturb_ts.py` (3 days) + pytest suite (2 days) + README + examples (2 days) | `perturb_ts.py` v1.0 passing all tests |
| 8–9 | Stage 6 | VAR theory reading (2 days) + VAR fitting (2 days) + correlated sampling (2 days) + module extension (3 days) | Multivariate module complete; all tests passing |
| 10 | Validation | Apply module to real-world datasets (see below) | Real-data validation notebook complete |
| 11 | Extensions | Choose 1–2 optional extensions (see below) | Selected extension implemented and tested |
| 12 | Wrap-up | Final technical report + code cleanup + documentation polish | Submission-ready module and report |
