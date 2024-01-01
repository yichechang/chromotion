# chromotion


## Dependencies
Dependencies can be found in [pyproject.toml](pyproject.toml).

## Installation
### Git submodules
`bim-xarray` is used interanlly and distributed as a git submodule
in this repo. Please make sure to properly clone the submodule contents
before proceeding the following.

### Installing dependencies
If using mamba (or conda) for dependency management, you may find
[environment.yaml](environment.yaml) useful. For example, install
by issuing
```
mamba create -n chromotion
mamba env update -n chromotion -f environment.yaml
```

## Git submodules
As stated above, [bim-xarray](https://github.com/SoftLivingMatter/bim-xarray/tree/release/chromotion)
is available as a git submodule.

- For end-users, just make sure to set up the submodule. Its use is only
internal to chromotion.

- For developers, you will use it in any modules in `chromotion` as
    ```python
    # Not pretty with all these dir layouts but it's needed
    import .bim_xarray.src.bim_xarray
    # Or, more conveniently as:
    import .bim_xarray.src.bim_xarray as bim
    ```

If you want to use `bim-xarray` in your project, it's best to install
it separately as a standalone package.
