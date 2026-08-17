# Raw data

This directory refers to external raw datasets required to execute the analysis pipeline.

Small or compressed contextual inputs needed by the revised pipeline are
included when redistribution and repository size permit. Large auxiliary
datasets remain available from their original providers or the Zenodo archive
described in the main README.

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

- `plate_boundaries_typed/`
  UTIG/NOAA plate-boundary layer with convergent, divergent, and transform
  classes. The curated GeoJSON used by the pipeline is versioned.

- `CRUST1/`
  CRUST1.0 Moho-depth grid used for continental contextual models. The curated
  `crust1_moho.xyz` file is versioned.

- `ocean_age/`
  Global oceanic crustal-age grid. The compressed `age.3.2.nc.bz2` input is
  versioned; the pipeline creates the ignored `age.3.2.nc` file locally.

## Notes

- The pipeline assumes this directory layout by default.
- Paths can be overridden via environment variables (see configuration section).
- Dataset-specific provenance, checksums, and expected filenames are provided
  in `README_context_datasets.md`.
