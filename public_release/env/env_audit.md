# Environment & Tooling Audit
- Timestamp (UTC): **2026-03-06T10:41:12+00:00**
- Output directory: `C:/Users/cgauj/OneDrive/Área de Trabalho/heatflow-intraplate-residuals/public_release/env`

## System
- Platform: `Windows-11-10.0.26200-SP0`
- OS: `Windows 11`
- Architecture: `AMD64`
- Python: `3.12.4 (tags/v3.12.4:8e8a4ba, Jun  6 2024, 19:30:16) [MSC v.1940 64 bit (AMD64)]`
- Executable: `C:\projetos\sismologia\Scripts\python.exe`

## Paths
- Saved: `path_resolution.txt`

## Pip
- Saved: `pip_list.txt` and `pip_freeze.txt`
### pip --version
```text
pip 25.2 from C:\projetos\sismologia\Lib\site-packages\pip (python 3.12)
```

### pip list (head)
```text
Package                   Version
------------------------- -------------------
access                    1.1.9
affine                    2.4.0
anyio                     4.10.0
arch                      7.2.0
argon2-cffi               25.1.0
argon2-cffi-bindings      25.1.0
arrow                     1.3.0
arviz                     0.22.0
astropy                   7.0.1
astropy-iers-data         0.2025.3.17.0.34.53
asttokens                 3.0.0
async-lru                 2.0.5
attrs                     25.1.0
babel                     2.17.0
beautifulsoup4            4.13.4
bleach                    6.2.0
blinker                   1.9.0
branca                    0.8.1
cachetools                6.1.0
Cartopy                   0.24.1
certifi                   2025.1.31
cffi                      1.17.1
cftime                    1.6.4.post1
charset-normalizer        3.4.1
click                     8.1.8
click-plugins             1.1.1
cligj                     0.7.2
cloudpickle               3.1.1
...
```

### pip freeze (head)
```text
access==1.1.9
affine==2.4.0
anyio==4.10.0
arch==7.2.0
argon2-cffi==25.1.0
argon2-cffi-bindings==25.1.0
arrow==1.3.0
arviz==0.22.0
astropy==7.0.1
astropy-iers-data==0.2025.3.17.0.34.53
asttokens==3.0.0
async-lru==2.0.5
attrs==25.1.0
babel==2.17.0
beautifulsoup4==4.13.4
bleach==6.2.0
blinker==1.9.0
branca==0.8.1
cachetools==6.1.0
Cartopy==0.24.1
certifi==2025.1.31
cffi==1.17.1
cftime==1.6.4.post1
charset-normalizer==3.4.1
click==8.1.8
click-plugins==1.1.1
cligj==0.7.2
cloudpickle==3.1.1
colorama==0.4.6
comm==0.2.2
...
```

## Conda
- conda not detected

## Jupyter
- Saved: `jupyter_version.txt`
```text
Selected Jupyter core packages...
IPython          : 9.2.0
ipykernel        : 6.30.1
ipywidgets       : 8.1.7
jupyter_client   : 8.6.3
jupyter_core     : 5.8.1
jupyter_server   : 2.16.0
jupyterlab       : 4.4.6
nbclient         : 0.10.2
nbconvert        : 7.16.6
nbformat         : 5.10.4
notebook         : 7.4.5
qtconsole        : not installed
traitlets        : 5.14.3
```

## Key scientific packages
| package | version | status |
|---|---|---|
| numpy | 2.3.4 | OK |
| pandas | 2.2.3 | OK |
| scipy | 1.15.2 | OK |
| matplotlib | 3.10.0 | OK |
| sklearn | 1.7.0 | OK |
| geopandas | 1.0.1 | OK |
| shapely | 2.1.1 | OK |
| pyproj | 3.7.0 | OK |
| cartopy | 0.24.1 | OK |
| rasterio | 1.4.3 | OK |
| xarray | 2025.6.1 | OK |
| statsmodels | 0.14.4 | OK |
| tqdm | 4.67.1 | OK |

## Notes

- Full `pip list` and `pip freeze` are stored as separate artifacts.
- `pip` is invoked via `python -m pip` to ensure interpreter consistency.
