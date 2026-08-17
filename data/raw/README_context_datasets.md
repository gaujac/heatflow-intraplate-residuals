# Context datasets used by the revised pipeline

This directory contains the curated contextual inputs required for the
boundary-type, CRUST1.0, and ocean-age analyses added during revision. Original
datasets remain subject to the terms of their respective providers and should
be cited from the manuscript references.

## Required structure

```text
data/raw/
├── CRUST1/
│   └── crust1_moho.xyz
├── ocean_age/
│   ├── age.3.2.nc.bz2
│   └── age.3.2.nc              # created locally; not versioned
└── plate_boundaries_typed/
    └── utig_noaa_plate_boundaries.geojson
```

## 1. Typed plate boundaries

- File: `plate_boundaries_typed/utig_noaa_plate_boundaries.geojson`
- Role: assigns convergent, divergent, or transform context to canonical
  intraplate observations.
- Source: NOAA National Centers for Environmental Information, Plate
  Boundaries (from UTIG), layer 12.
- Source URL:
  <https://gis.ngdc.noaa.gov/arcgis/rest/services/web_mercator/hazards/MapServer/12>
- SHA-256:
  `348D51F0727B6DDD845E33E59B676704B999FCA12E55240E79E961CF2BE82992`

## 2. CRUST1.0 Moho depth

- File: `CRUST1/crust1_moho.xyz`
- Role: continental crustal-context predictor.
- Source: CRUST1.0, Laske et al. (2013).
- Project URL: <https://igppweb.ucsd.edu/~gabi/crust1.html>
- SHA-256:
  `167A9CBD698AB709DBAB9EC65E9701454533D264E9A446E424F4D4F02CEEB98C`

## 3. Oceanic crustal age

- Versioned file: `ocean_age/age.3.2.nc.bz2`
- Runtime file: `ocean_age/age.3.2.nc`
- Role: oceanic lithospheric-age predictor.
- Source: global seafloor-age grid associated with Müller et al. (2008).
- SHA-256 of the compressed file:
  `49003831DB78F7BB044532DAF31FDC49218F75876668EE0C96877F383214B827`

The pipeline decompresses `age.3.2.nc.bz2` when `age.3.2.nc` is absent. The
uncompressed NetCDF file is intentionally ignored by Git because it is about
117 MB.

## Main analysis outputs

```text
public_release/pipeline_kmeans/analysis/boundary_type_context/
public_release/pipeline_kmeans/analysis/crust1_ocean_age_context/
public_release/figures_main/fig7_boundary_type_context_panel.(png|pdf)
public_release/figures_main/fig8_crust1_ocean_age_context_panel.(png|pdf)
```

Paths may be overridden through the routing variables defined in Snippet 2,
including `UTIG_TYPED_BOUNDARIES_GEOJSON`, `CRUST1_MOHO_PATH`, and
`OCEAN_AGE_GRID_PATH`.
