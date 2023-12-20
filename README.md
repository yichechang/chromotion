## Installation
1. Install `bim-xarray` (a git submodule)
    ```bash
    # at the root of the repo
    pip install -e ./bim-xarray
    ```
2. Install `chromotion` (this project)
    ```bash
    # at the root of the repo
    pip install -e .
    ```

Above steps can be included into a conda environment file. But the 
critical part is to install `bim-xarray` first, because `chromotion`
depends on it and it is not on PyPI yet.