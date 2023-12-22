[bim-xarray](https://github.com/SoftLivingMatter/bim-xarray/tree/release/chromotion)
is available as a git submodule.

For end-users, just make sure to set up the submodule. Its use is only
internal to chromotion.

For developers, you will use it in any modules in `chromotion` as 
```python
import .bim_xarray.src.bim_xarray

# Or, more conveniently as:
import .bim_xarray.src.bim_xarray as bim
```