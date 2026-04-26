# Persistence of Intraplate Heat-Flow Anomalies and Tectonic Distance Analysis

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19493652.svg)](https://doi.org/10.5281/zenodo.19493652)

This repository provides a fully reproducible analysis pipeline supporting the study:

## Persistence of intraplate heat-flow anomalies far from tectonic boundaries

This study demonstrates that statistically significant heat-flow anomalies persist at large distances from tectonic boundaries, challenging classical models in which tectonic proximity is the dominant control on terrestrial heat flow.

Using global datasets and a strictly reproducible analytical framework, we show that the heat-flow signal remains robust beyond conventional tectonic domains, with implications for lithospheric processes and internal heat generation mechanisms.

All results reported in the manuscript are fully reproducible from this pipeline.

---

# Correspondence

**Cristiano Gaujac**
Independent Researcher
📧 [papers.gaujac@gmail.com](mailto:papers.gaujac@gmail.com)

---

# 1. Repository Structure

```
heatflow-intraplate-residuals/
│
├── pipeline/                         # Jupyter notebooks and analysis scripts
│
├── public_release/                  # Generated outputs (created at runtime; not versioned)
│ │
│ ├── figures_main/
│ ├── figures_supplementary_methods/
│ ├── figures_supplementary_results/
│ │
│ ├── pipeline_kmeans/
│ ├── qa/
│ ├── flow/
│ │
│ ├── env/
│ └── freeze/
│
├── public_release_package/          # Curated submission-ready export package
│
├── data/                            # Input datasets (partially redistributed)
│
├── environment.yml                  # Conda environment specification
├── CITATION.cff                     # Citation metadata
├── LICENSE                          # MIT license
├── .gitignore
└── README.md
```

---

# 2. Reproducibility

## 2.1. Create environment (recommended)

```bash
conda env create -f environment.yml
conda activate heatflow-intraplate-residuals
```

---

## 2.2. Run the pipeline

```bash
cd pipeline
jupyter lab
```

Open:

```
pipeline_heatflow_vs_tectonics.ipynb
```

---

## 2.3. Outputs

All figures, tables, and reproducibility artifacts are generated locally when running the pipeline.

These outputs are written to:

```
public_release/
```

This directory is generated automatically during execution and is **not versioned in this repository**.

A frozen version corresponding to the manuscript is archived on Zenodo.

---

# 3. Frozen Results

The canonical frozen outputs corresponding to the manuscript are archived on Zenodo:

https://doi.org/10.5281/zenodo.19493652

These include:

• final figures used in the manuscript
• robustness diagnostics
• QA fragmentation tests
• pipeline reproducibility manifests
• computational environment audits

This archive represents the **canonical reference for all results reported in the manuscript**.

---

# 4. Publication Figures

Publication figures are organized as:

```
public_release/
├── figures_main/
├── figures_supplementary_methods/
└── figures_supplementary_results/
```

These directories are generated during pipeline execution.

The version used in the manuscript is archived on Zenodo and corresponds exactly to the reproducibility package.

---

# 5. Reproducibility Records

The pipeline generates dedicated reproducibility artifacts:

```
public_release/env/
public_release/freeze/
```

These directories are created during execution and are not stored in this repository.

• `env/` contains the computational environment audit
• `freeze/` contains the reproducibility manifest (hashes + configuration)

The frozen versions of these artifacts are included in the Zenodo archive.

---

# 6. Data Sources

Main datasets used in this study:

• IHFC Global Heat Flow Database (2024 release)
• GEM Global Active Faults database
• PB2002 plate boundary model

All datasets are cited in the manuscript.

Raw data are not redistributed when licensing restrictions apply.

---

# 7. Reproducing Figures

Running the full pipeline reproduces:

• main manuscript figures
• distance–heat flow statistical analyses
• robustness tests and sensitivity analyses
• supplementary figures and diagnostics

Generated outputs are written to:

```
public_release/
```

---

# 8. Reproducibility and Traceability

This project follows strict reproducibility practices:

• deterministic analytical pipeline
• versioned figure outputs
• cryptographic fingerprints (SHA-256)
• environment audit
• frozen reproducibility manifest

These measures ensure that all reported results are fully traceable and reproducible.

---

# 9. Code Availability

The complete reproducible pipeline is available in this repository.

The code corresponds exactly to the version used to generate the archived results.

A frozen version is archived at:
https://doi.org/10.5281/zenodo.19493652

---

# 10. License and Data Use

This repository is provided for scientific reproducibility and peer verification.

The code is released under the **MIT License**.

Original datasets remain subject to their respective licenses and are cited in the manuscript. Redistribution of restricted datasets may not be permitted.

Some large raw datasets are not included in this repository due to GitHub file size limitations. These datasets are standard public geophysical resources and can be obtained from their original providers (e.g., IHFC, GEM, PB2002, WGM2012, GSRM, and global earthquake catalogs).

All processing steps remain fully reproducible using the provided code and data access instructions.

---

# 11. Data availability

The datasets required for full reproducibility are available via Zenodo:

* Main reproducibility archive (pipeline outputs and frozen results):
  https://doi.org/10.5281/zenodo.19493652

* Large auxiliary datasets (earthquakes, gravity grids):
  https://doi.org/10.5281/zenodo.19784141

All datasets correspond to the versions used in the manuscript and ensure full independent reproducibility of the analysis.
