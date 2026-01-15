# Replication notebook (Google Colab)

This repository contains the Google Colab notebook used to reproduce figures, tables,
and key numerical results for the manuscript:

**A seasonal two-sex matrix framework that links caregiver stages to management thresholds**  
Shaikh Obaidullah  
Submitted to *Ecological Modelling*

---

## How to run (recommended)

The analysis is implemented as a single Google Colab notebook.

Open the notebook directly in Colab using the badge below and run all cells top-to-bottom.

**Open in Colab**

No local installation is required.

---

## What the notebook does

The notebook reproduces the main computational components of the manuscript:

### Polar bear (Southern Beaufort Sea; P = 1)

- caregiver-structured female block
- annual net reproductive number \( R_0 \)
- growth rate \( \lambda \)
- elasticities and population projections

### Black-tailed prairie dog (P = 12)

- data-driven ingestion of USGS survival and reproduction CSVs
- construction of monthly survival and fecundity blocks
- periodic next-generation operator \( R_{0,\mathrm{per}} \)
- seasonal diagnostics and invasion calculations

All modeling conventions match those stated in the manuscript:

- column-vector (to–from) matrix convention,
- newborns treated as reported output (not a state),
- periodic monodromy and next-generation operators defined on the female stage space.

---

## Outputs

Running the notebook generates an `out/` directory containing:

- `out/figs/` — PNG figures used in the manuscript  
- `out/tables/` — LaTeX-ready tables and CSV summaries  
- `out/params/` — machine-readable inputs, schema, and audit reports  
- `out/summary/` — JSON summaries for cross-checking results  

All outputs are **regenerated each time the notebook is run** and are not version-controlled.

---

## Data sources

Prairie-dog data are from the U.S. Geological Survey data release:

Eads, D. A. (2022). *Black-tailed prairie dog survival and reproduction*.  
DOI: https://doi.org/10.5066/P9QTWGP4

Polar-bear parameters are literature-derived and documented in the manuscript.

---

## Notes for reviewers

Running the notebook is **not required** to review the manuscript.  
The notebook is provided for transparency and reproducibility.  
All figures and tables referenced in the manuscript are produced by this workflow.

---

## Citation

Please cite the manuscript and the USGS data release if you use this code or notebook.
