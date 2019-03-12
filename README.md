# Repository for gdalcubes image collection formats

Central place for gdalcubes image collection formats that formalize file / directory structures
of common Earth observation products. The list of available formats (see below) is expected
to grow continuously.

Collection formats are defined as JSON files, containing regular expressions how
image identifiers and aquisition date / time can be derived from filenames and which files store which
bands of the data. 

## Available formats

The repository currently contains the following formats:

|Format                      |Description                                                                                                                                                                                                                                                                                   |
|:---------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|CHIRPS_v2_0_daily_p05_tif   |Image collection format for CHIRPS v 2.0 daily global precipitation dataset (0.05 degrees resolution) from GeoTIFFs, expects list of .tif or .tif.gz files as input. [TAGS: CHIRPS, precipitation]                                                                                            |
|CHIRPS_v2_0_monthly_p05_tif |Image collection format for CHIRPS v 2.0 monthly global precipitation dataset (0.05 degrees resolution) from GeoTIFFs, expects list of .tif or .tif.gz files as input. [TAGS: CHIRPS, precipitation]                                                                                          |
|L8_L1TP                     |Collection format for Landsat 8 Level 1 TP product [TAGS: Landsat, USGS, Level 1, NASA]                                                                                                                                                                                                       |
|L8_SR                       |Collection format for Landsat 8 surface reflectance product [TAGS: Landsat, USGS, Level 2, NASA, surface reflectance]                                                                                                                                                                         |
|MxD10A2                     |Collection format for selected bands from the MODIS MxD10A2 (Aqua and Terra) v006 Snow Cover product [TAGS: MODIS, Snow Cover]                                                                                                                                                                |
|MxD11A1                     |Collection format for selected bands from the MODIS MxD11A2 (Aqua and Terra) v006 Land Surface Temperature product [TAGS: MODIS, LST]                                                                                                                                                         |
|MxD11A2                     |Collection format for selected bands from the MODIS MxD11A2 (Aqua and Terra) v006 Land Surface Temperature product [TAGS: MODIS, LST]                                                                                                                                                         |
|MxD13A3                     |Collection format for selected bands from the MODIS MxD13A3 (Aqua and Terra) product [TAGS: MODIS, VI, NDVI, EVI]                                                                                                                                                                             |
|Sentinel2_L1C               |Image collection format for Sentinel 2 Level 1C data as downloaded from the Copernicus Open Access Hub, expects a list of file paths as input. The format works on original ZIP compressed as well as uncompressed imagery. [TAGS: Sentinel, Copernicus, ESA, TOA]                            |
|Sentinel2_L1C_AWS           |Image collection format for Sentinel 2 Level 1C data in AWS [TAGS: Sentinel, Copernicus, ESA, TOA]                                                                                                                                                                                            |
|Sentinel2_L2A               |Image collection format for Sentinel 2 Level 2A data as downloaded from the Copernicus Open Access Hub, expects a list of file paths as input. The format should work on original ZIP compressed as well as uncompressed imagery. [TAGS: Sentinel, Copernicus, ESA, BOA, Surface Reflectance] |