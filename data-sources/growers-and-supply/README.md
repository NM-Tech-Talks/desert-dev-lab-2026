# Growers, Land, Water, And Supply Chain Datasets

This guide supports grower, land, and resilience project ideas, especially:

- new growers facing land and startup barriers
- experienced growers facing aging-workforce and succession risk
- small growers struggling with land, infrastructure, and capital
- producers lacking demand and distribution visibility
- water scarcity, value-add infrastructure, fertilizer, and procurement-adjacent ideas

## Best Starting Sources

### USDA NASS Quick Stats API

- **Link:** [Quick Stats API](https://quickstats.nass.usda.gov/api) and [API tutorial](https://quickstats.nass.usda.gov/tutorials)
- **Coverage:** National, state, county, and other geographies where available
- **What it contains:** Census of Agriculture and survey data for farm counts, acreage, sales, production, and producer demographics
- **Why it matters:** Best all-purpose agricultural baseline for New Mexico counties
- **Access:** REST API with a free key
- **Format:** JSON, CSV, XML
- **Use in an app:** Query by county, year, and data item to build dashboards for production trends, producer age, or operation scale

### NRCS Soil Data Access / SSURGO

- **Link:** [Soil Data Access](https://sdmdataaccess.nrcs.usda.gov/) and [spatial web services](https://sdmdataaccess.sc.egov.usda.gov/Spatial2/)
- **Coverage:** National, soil-map-unit scale
- **What it contains:** Soil texture, drainage, depth, salinity risk, and available water capacity
- **Why it matters:** Land is not useful for agriculture just because it is available; this helps determine whether a site is actually viable
- **Access:** Public web services and SSURGO-related tools
- **Format:** Tabular outputs, WMS, WFS, and downloadable soil resources
- **Use in an app:** Precompute parcel or site suitability scores rather than querying live for every map click

### Bernalillo County Parcel Data Via Albuquerque GIS

- **Link:** [Parcel layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/AddressReport/MapServer/4)
- **Coverage:** Bernalillo County
- **What it contains:** Parcel geometry and assessor-related attributes
- **Why it matters:** Most practical local source for land-discovery and parcel-ranking projects
- **Access:** Public ArcGIS REST layer
- **Format:** GIS feature service with JSON-style query responses
- **Use in an app:** Export parcels into a spatial database, then enrich them with soil, zoning, infrastructure, and market-distance fields

### New Mexico Agriculture And Food Supply Chain Atlas

- **Link:** [Atlas](https://nmfoodchainatlas.nmsu.edu/) and [data hub](https://supply-chain-data-hub-nmcdc.hub.arcgis.com/)
- **Coverage:** New Mexico statewide
- **What it contains:** Aggregators, processors, commercial kitchens, warehouses, storage facilities, transportation firms, and markets
- **Why it matters:** Excellent for the “missing middle” between growers and buyers
- **Access:** Public map tools and ArcGIS Hub resources
- **Format:** GIS-style resources and web map layers
- **Use in an app:** Build infrastructure search, routing, or gap-analysis tools for growers and food-system planners

### USGS Water Data APIs

- **Link:** [USGS Water Data APIs](https://api.waterdata.usgs.gov/) and [daily values service details](https://waterservices.usgs.gov/docs/dv-service/daily-values-service-details/)
- **Coverage:** National with local station-level data
- **What it contains:** Monitoring locations, streamflow, groundwater, and hydrologic time series
- **Why it matters:** Water scarcity is a core agricultural constraint in New Mexico
- **Access:** Open API
- **Format:** JSON, WaterML, tab-delimited outputs
- **Use in an app:** Cache nearby station data, then compute simple indicators like low-flow warnings, seasonal comparisons, or irrigation-risk flags

### NOAA Climate Data Online

- **Link:** [API docs](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) and [token request](https://www.ncdc.noaa.gov/cdo-web/token)
- **Coverage:** National, station-level
- **What it contains:** Temperature, precipitation, daily summaries, and station metadata
- **Why it matters:** Useful for planting windows, extreme-heat risk, and long-term resilience planning
- **Access:** REST API with a free token
- **Format:** JSON with pagination
- **Use in an app:** Pull Albuquerque-area weather history and generate simplified climate summaries for users

## Useful Secondary Sources

### USDA Cropland Data Layer

- **Link:** [Cropland Data Layer web service](https://www.nass.usda.gov/Research_and_Science/Cropland/docs/WebService.html)
- **Why it matters:** Helps answer what is being grown nearby and where agricultural land use is active or changing
- **Best use:** Preprocessed summary maps and land-use trend analysis

### USDA Local Food Directories

- **Link:** [Data sharing page](https://www.usdalocalfoodportal.com/fe/datasharing/)
- **Why it matters:** Useful for the demand side of grower projects because it exposes possible markets and food hubs
- **Best use:** Local sales-channel discovery, producer routing, and “where can I sell?” tools

## Recommended Source Combinations

- **New grower land matcher:** parcels + SSURGO + zoning from the civic guide
- **Grower resilience dashboard:** NASS Quick Stats + USGS Water Data + NOAA Climate Data
- **Supply chain finder:** NM Food Supply Chain Atlas + USDA Local Food Directories + NASS Quick Stats

## Integration Notes

- GIS-heavy sources here are best used in a preprocessing step.
- For a weekend project, teams should prefer derived summary tables over raw raster or map-service layers.
- Some problems in this cluster, especially around capital access and water rights, may need partner interviews or non-public administrative context in addition to open datasets.
- For a deeper water-focused source list, see [Water and climate](../water-and-climate/README.md).
