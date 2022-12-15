# Changelog

This file documents all notable changes to the netcdf-scripts repository.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.5] -- 2022-12-15
### Fixed
- Fixed bug in checking whether `time:units` has decimals or not

## [0.1.4] -- 2022-12-15
### Added
- Added extra checks to `isCoards` for issues that would prevent a netCDF file from being read into GCHP

### Changed
- Changed the temporary filename in `nc_chunk.pl` from `tmp.nc` to `tmp.$ncFile`.  This allows files named "tmp.nc" to be chunked & compressed.

## [0.1.3] - 2022-12-01
### Changed
- Exit `isCoards` if the netCDF input file is not found
- Now point user to more information about editing netCDF files at geos-chem.readthedocs.io

## [0.1.2] - 2022-11-30
### Changed
- Updated CHANGELOG.md with latest version information

## [0.1.1] - 2022-11-30
- `isCoards` now checks for variables of type int (not allowed for GCHP)
- Remove debug printout from `isCoards`

## [0.1.0] - 2022-11-30
### Added
- Add badges to README.md
- Add .gitignore in root folder
- Add GitHub issue and pull-request templates

## [0.0.2] - 2022-11-29
- No changes
- This release was issued to force auto-DOI generation with Zenodo

## [0.0.1] - 2022-11-29
- Initial release
