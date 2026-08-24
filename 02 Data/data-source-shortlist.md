# Data Source Shortlist — Neil Panchal

This note ranks the 8 sources in `01 Research/source-tracker.csv` by how easy each one is to bring into QGIS, so the team knows where to start once a pilot region is picked.

## Easiest to use in QGIS

**OpenStreetMap** — Export directly as GeoJSON/Shapefile from the OSM web export tool or Overpass Turbo, then drag into QGIS. No account or processing needed for small areas.

**NASA FIRMS** — Active fire points download as CSV or Shapefile with lat/long already included. Import as a delimited text layer or vector layer directly.

**GADM** — Downloads as GeoPackage per country, opens directly in QGIS with no reprojection needed for a first pass.

## Moderate effort

**WorldPop** — GeoTIFF rasters, straightforward to load as a raster layer, but files can be large at 100m resolution for bigger countries. May need to clip to the study area first.

**Healthsites.io / OSM emergency services tags** — Healthsites data downloads as GeoJSON and loads directly. The OSM fire station tags need a separate Overpass query, which takes a bit more setup than a straight export.

## More setup required

**ESA WorldCover** — Downloads as Cloud Optimized GeoTIFFs in large tiles (3x3 degree or 60x60 degree grouping). Requires clipping to the study area before it is usable, and file sizes are large.

**NASA POWER** — Comes through an API rather than a direct file download. Needs a small script or the Data Access Viewer tool to pull a CSV/NetCDF before it can be loaded into QGIS.

**MODIS NDVI (MOD13Q1)** — Distributed in HDF format on a sinusoidal grid. Needs reprojection and format conversion (GDAL or the MODIS reprojection tool) before it lines up with the other layers.

## Recommendation

Start building the base map with OpenStreetMap, NASA FIRMS, and GADM first since they load with the least friction. Bring in WorldPop and the emergency services proxy next. Save ESA WorldCover, NASA POWER, and MODIS NDVI for after the study area is locked (Week 4), since clipping and reprojecting them ahead of time would be wasted work if the region changes.
