# Raw data (not versioned)

This directory refers to external raw datasets required to execute the analysis pipeline.

These datasets are **not included in the GitHub repository** due to file size limitations, licensing constraints, and reproducibility design. Instead, they are provided via external archives (see Data availability section).

Users must download and place the required datasets locally following the directory structure below.

## Expected structure

- `IHFC/`  
  Global surface heat-flow measurements (IHFC Global Heat Flow Database, 2024 release; Excel format)

- `GEM/`  
  Global active fault database (GEM Global Active Faults)

- `PB2002/`  
  Global plate boundary model (PB2002)

- `NaturalEarth/`  
  Country boundaries and base layers (Natural Earth)

- `earthquakes/`  
  Global seismicity catalogs (CSV/Parquet; see Zenodo auxiliary dataset)

- `strain/`  
  Global strain-rate model (GSRM; NetCDF)

- `gravity/`  
  Bouguer gravity grids (WGM2012; see Zenodo auxiliary dataset)

## Notes

- The pipeline assumes this directory layout by default.
- Paths can be overridden via environment variables (see configuration section).
- Raw datasets must be used without preprocessing to ensure full reproducibility of the reported results.