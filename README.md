[![Latest Release](https://img.shields.io/github/v/release/geoschem/netcdf-scripts?label=Latest%20Release)](http://github.com/geoschem/netcdf-scripts/releases) [![Release date](https://img.shields.io/github/release-date/geoschem/netcdf-scripts)](https://github.com/geoschem/netcdf-scripts) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7377643.svg)](https://doi.org/10.5281/zenodo.7377643) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/geoschem/netcdf-scripts/blob/main/LICENSE.txt)

# netcdf-scripts

This repository contains convenience scripts for viewing and editing netCDF files.

## Contents

All scripts are in the `scripts/` folder:

1. `isCoards`: Determines whether a netCDF file adheres to the COARDS netCDF conventions.  This is required if the files are to be read by GEOS-Chem Classic or GCHP.
   
2. `nc_chunk.pl`: Deflates and chunks a netCDF file.  See the [Work with netCDF files](https://geos-chem.readthedocs.io/en/stable/geos-chem-shared-docs/supplemental-guides/netcdf-guide.html#chunk-and-deflate-a-netcdf-file-to-improve-i-o) for more information.
   
3. `ncd`: Wrapper script for the `ncdump` command, which lets you view the header information of a netCDF file.
   
4. `time_units`: Wrapper script that allows you to reset the `time:units` attribute of a netCDF file.
   
5. `time_unlimited`: Wrapper script that allows you to set the `time` dimension of a netCDF file to `UNLIMITED`.  NetCDF files must have an `UNLIMITED` time dimension before they can be concatenated with e.g. the NCO `ncrcat` command.
