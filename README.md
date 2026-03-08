# Desert Dev Lab 2026

Resources for the Desert Dev Lab Hackathon 2026.

This repository is a starting point for teams building around the **Food & Agriculture** theme. It turns the working list of problem statements in the [Food & Ag review sheet](https://docs.google.com/spreadsheets/d/1EN2ns9BAI97obRXzsCTIX5tEi8aBhEP8/edit?usp=sharing&ouid=102887163016251251248&rtpof=true&sd=true) into a README-first guide with recommended datasets, APIs, and practical notes on how to use them.

The rows marked `Go` in the sheet are treated as the featured hackathon prompts and are listed first below.

## How To Use This Repo

1. Pick a featured problem statement or an additional prompt.
2. Choose 1-3 data sources from the matching recommendations.
3. Build a thin prototype first: map, search tool, dashboard, matching engine, alerting workflow, or planning assistant.
4. Add your own assumptions, local partner input, and user interviews. These datasets are starting points, not the whole solution.

## Featured Problem Statements

### 1. Strengthen Albuquerque's local food resilience

**Problem statement:** Nearly all food consumed in Albuquerque is sourced from outside the region, which makes the city vulnerable to supply-chain disruption and makes it harder for local producers to compete.

**Why it matters:** This is a strong systems-level challenge for teams interested in food security, local purchasing, supply-chain visibility, and local economic development.

**Recommended data sources**

- [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/) to find nearby farmers markets, food hubs, CSAs, and other direct-to-consumer channels.
- [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/) to map processors, aggregators, commercial kitchens, warehouse/storage sites, transportation firms, and markets across New Mexico.
- [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api) to estimate local production capacity, commodity mix, farm counts, and producer demographics at the state and county level.
- [USDA SNAP Retailer Data](https://www.fns.usda.gov/snap/retailer/historicaldata) to understand the current retail network where food purchasing already happens.
- [USGS Water Data APIs](https://api.waterdata.usgs.gov/) and [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) to layer water and climate risk into local food-system resilience.

**Starter build ideas**

- A map showing where Albuquerque depends on outside supply versus where local alternatives already exist.
- A local procurement or sourcing assistant that matches nearby producers and food-system infrastructure to buyers.
- A resilience dashboard combining local food infrastructure, water conditions, and climate stress indicators.

### 2. Help new growers overcome land and startup barriers

**Problem statement:** New growers lack affordable land, infrastructure, and startup capital, and these barriers are intensified by urban sprawl and desertification.

**Why it matters:** This prompt is a good fit for teams working on land discovery, parcel scoring, small-farm planning, incubator programs, and local food entrepreneurship.

**Recommended data sources**

- [Bernalillo County parcel layers via Albuquerque GIS](https://coageo.cabq.gov/cabqgeo/rest/services/agis/AddressReport/MapServer/4) to identify candidate parcels by size, location, and assessor data.
- [NRCS Soil Data Access / SSURGO](https://sdmdataaccess.nrcs.usda.gov/) to evaluate soil conditions, water-holding capacity, drainage, and land suitability.
- [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api) to benchmark farm sizes, production patterns, and agricultural trends in New Mexico counties.
- [USDA Cropland Data Layer](https://www.nass.usda.gov/Research_and_Science/Cropland/docs/WebService.html) to understand what land is currently in agricultural use and how land use has changed over time.
- [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/) to locate nearby infrastructure such as commercial kitchens, storage, transportation, and aggregators.

**Starter build ideas**

- A parcel-scoring tool that ranks sites for small-scale growing based on soil, size, and proximity to markets or infrastructure.
- A “getting started as a grower” planner that highlights land, infrastructure, and likely sales channels in one workflow.

### 3. Support an aging producer workforce and succession planning

**Problem statement:** Farming and ranching are experiencing an aging and declining workforce in New Mexico, creating urgency around succession planning, knowledge transfer, and long-term continuity.

**Why it matters:** This prompt works well for teams interested in workforce planning, mentorship matching, risk forecasting, and tools that make agricultural operations more sustainable over time.

**Recommended data sources**

- [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api) for producer age and county-level agricultural indicators from the Census of Agriculture and related surveys.
- [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) for temperature, precipitation, and long-term climate patterns that affect planning.
- [USGS Water Data APIs](https://api.waterdata.usgs.gov/) for streamflow and hydrologic observations, especially around the Rio Grande and nearby monitoring stations.
- [USDA Cropland Data Layer](https://www.nass.usda.gov/Research_and_Science/Cropland/docs/WebService.html) for crop and land-cover context.
- [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/) for downstream sales and distribution channels that may matter in a succession plan.

**Starter build ideas**

- A county-by-county dashboard showing where aging producer risk is highest and which areas have nearby markets or infrastructure.
- A mentorship or farm transition app that combines demographic risk, climate exposure, and local market context.

### 4. Improve community influence over food-related public spaces

**Problem statement:** Community members lack consistent ways to influence how food-related public spaces are designed, named, activated, and evaluated over time.

**Why it matters:** This prompt fits civic-tech teams interested in community markets, neighborhood participation, site selection, public-space activation, and accountability.

**Recommended data sources**

- [Albuquerque public facilities GIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer) to find community centers, libraries, and other civic sites that could host food-related activity.
- [Albuquerque GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data) for parks, administrative boundaries, municipal layers, and other place-based data.
- [Albuquerque public zoning viewer](https://coagisweb.cabq.gov/Geocortex/Essentials/geo482/REST/sites/Public_Zoning_Viewer/map) and [land use service](https://coageo.cabq.gov/cabqgeo/rest/services/agis/Land_Use/FeatureServer) to understand siting and land-use context.
- [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/) to identify existing markets and local food businesses.
- [U.S. Census ACS API](https://www.census.gov/programs-surveys/acs/data/data-via-api.html) to add neighborhood demographics, vehicle access, age, income, and other community context.

**Starter build ideas**

- A public map where residents can propose food-space improvements and see which neighborhood, district, and city facilities are involved.
- A site-selection tool for community markets or pop-up food events that balances public space, zoning, and neighborhood need.

## Additional Problem Statements

These are the remaining prompts from the working sheet. They may be a better fit for teams who want a narrower operational problem than the featured prompts above.

### Food Access & Affordability

| Problem | Problem statement | Strong starting data |
| --- | --- | --- |
| Food waste | About one-third of food produced in the United States is wasted, creating cost, water, and emissions losses across the supply chain. | [EPA Excess Food Opportunities Map](https://www.epa.gov/sustainable-management-food/excess-food-opportunities-map), [Feeding America Map the Meal Gap](https://www.feedingamerica.org/research/map-the-meal-gap/by-county), [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/) |
| FA-01 | Many households in Albuquerque face inconsistent access to fresh, healthy food due to neighborhood-level retail gaps, especially in underserved areas. | [USDA Food Access Research Atlas](https://www.ers.usda.gov/data-products/food-access-research-atlas/), [U.S. Census ACS API](https://www.census.gov/programs-surveys/acs/data/data-via-api.html), [USDA SNAP Retailer Data](https://www.fns.usda.gov/snap/retailer/historicaldata) |
| FA-02 | Residents experience confusion and delays when trying to locate timely food assistance resources during disruptions or emergencies. | [USDA SNAP Retailer Data](https://www.fns.usda.gov/snap/retailer/historicaldata), [NM-IBIS food insecurity and SNAP indicators](https://ibis.doh.nm.gov/query/builder/acs/ACSEconomic/FoodSNAP.html), [Albuquerque public facilities GIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer) |

### Local Production & Growers

| Problem | Problem statement | Strong starting data |
| --- | --- | --- |
| LP-01 | Small-scale growers struggle to increase production because land, infrastructure, and capital are limited or expensive. | [Bernalillo County parcel layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/AddressReport/MapServer/4), [NRCS Soil Data Access / SSURGO](https://sdmdataaccess.nrcs.usda.gov/), [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/) |
| LP-02 | Local producers lack clear visibility into demand, distribution channels, and pricing needed to plan sustainable operations. | [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/), [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/), [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api) |
| Equipment emissions | Local producers have aging, expensive, high-emissions equipment, making replacements and emissions reductions costly. | [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api), [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/webservices/v2), [USGS Water Data APIs](https://api.waterdata.usgs.gov/) |
| Large grower emissions | Large producers may face future emissions-reduction requirements under climate policy. | [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api), [USDA Cropland Data Layer](https://www.nass.usda.gov/Research_and_Science/Cropland/docs/WebService.html), [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) |
| Water scarcity | Producers face rising water scarcity and inconsistency for watering crops. | [USGS Water Data APIs](https://api.waterdata.usgs.gov/), [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/webservices/v2), [NRCS Soil Data Access / SSURGO](https://sdmdataaccess.nrcs.usda.gov/) |
| Water rights complexity | Water law and water-rights systems create uneven access and usage. | [USGS Water Data APIs](https://api.waterdata.usgs.gov/), [NRCS Soil Data Access / SSURGO](https://sdmdataaccess.nrcs.usda.gov/), local legal or administrative records collected by subject-matter partners |
| Producer wages | Local producers struggle to earn a living and pay thriving wages. | [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api), [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/), [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/) |
| Value-add infrastructure | Producers and value-add businesses lack commercial kitchens, cold storage, and cold transportation. | [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/), [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/), [Albuquerque GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data) |
| Fertilizer impacts | Nitrogen-intensive fertilizer use is emissions-heavy and can contaminate water. | [NRCS Soil Data Access / SSURGO](https://sdmdataaccess.nrcs.usda.gov/), [USGS Water Data APIs](https://api.waterdata.usgs.gov/), [NOAA Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) |

### Permitting, Regulation, Distribution, and Markets

| Problem | Problem statement | Strong starting data |
| --- | --- | --- |
| PR-01 | Entrepreneurs face complex permitting and registration processes when starting or expanding small food retail or market activities. | [Albuquerque public zoning viewer](https://coagisweb.cabq.gov/Geocortex/Essentials/geo482/REST/sites/Public_Zoning_Viewer/map), [Albuquerque GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data), [ABQ Data](https://www.cabq.gov/abq-data) |
| PR-02 | City departments lack a shared view of food-system-related activities, leading to fragmented coordination and inconsistent support. | [ABQ Data](https://www.cabq.gov/abq-data), [Albuquerque GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data), [Albuquerque public facilities GIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer) |
| DW-01 | Surplus food from retailers and institutions is not consistently captured or redirected to organizations serving food-insecure residents. | [EPA Excess Food Opportunities Map](https://www.epa.gov/sustainable-management-food/excess-food-opportunities-map), [Albuquerque public facilities GIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer), [Feeding America Map the Meal Gap](https://www.feedingamerica.org/research/map-the-meal-gap/by-county) |
| DW-02 | Composting and organic waste diversion are unevenly adopted and difficult to track across neighborhoods and organizations. | [EPA Excess Food Opportunities Map](https://www.epa.gov/sustainable-management-food/excess-food-opportunities-map), [ABQ Data](https://www.cabq.gov/abq-data), local solid-waste program data from partners |
| MC-01 | Community markets face operational barriers such as limited hours, safety concerns, and unclear requirements that reduce participation. | [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/), [Albuquerque public facilities GIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer), [Albuquerque GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data) |
| Procurement | Large public entities struggle to buy food from local vendors because procurement processes favor lowest bids, consistent product, and existing internal workflows. | [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/), [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/), [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api) |

## Dataset And API Catalog

This section explains what each source contains, why it matters, how to access it, and how teams can use it in a hackathon project.

### 1. USDA Food Access Research Atlas

- **Link:** [Food Access Research Atlas](https://www.ers.usda.gov/data-products/food-access-research-atlas/) and [download page](https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data)
- **Coverage:** U.S. census tracts
- **What it contains:** Tract-level indicators for low income, low access, distance to supermarkets, vehicle access, and related food-access measures
- **Why it is relevant:** Best source for mapping neighborhood-level food access gaps and building food-desert-style analyses
- **Access:** Bulk download plus USDA geospatial services
- **Format:** Excel, ZIP, tract-level tables, GIS-friendly files, ArcGIS services
- **How to use it:** Join tract IDs to Census boundaries, then overlay grocery, SNAP retailer, transit, or population data
- **Good fit for:** `FA-01`, broader access and affordability work, neighborhood prioritization

### 2. U.S. Census American Community Survey API

- **Link:** [ACS API overview](https://www.census.gov/programs-surveys/acs/data/data-via-api.html) and [example queries](https://api.census.gov/data/2020/acs/acs5/examples.html)
- **Coverage:** National, filterable to New Mexico, Bernalillo County, Albuquerque-area tracts, ZIP Code Tabulation Areas, and other geographies
- **What it contains:** Income, poverty, rent burden, vehicle access, age, disability, internet access, education, commute, and household characteristics
- **Why it is relevant:** Adds social and economic context to almost every problem statement in this repo
- **Access:** REST API over HTTP; a key is recommended for higher-volume use
- **Format:** JSON or CSV-style API responses
- **How to use it:** Fetch only the fields you need, store them in your app database, and calculate composite neighborhood indicators
- **Example query:** `https://api.census.gov/data/2022/acs/acs5?get=NAME,B01003_001E&for=tract:*&in=state:35&in=county:043`
- **Good fit for:** `FA-01`, `FA-02`, `MC-02`, equity overlays, demographic context

### 3. USDA SNAP Retailer Data

- **Link:** [Historical SNAP retailer data](https://www.fns.usda.gov/snap/retailer/historicaldata) and [retailer locator](https://www.fns.usda.gov/snap/retailer-locator)
- **Coverage:** National, filterable to New Mexico and Albuquerque
- **What it contains:** SNAP-authorized retailers, addresses, coordinates, retailer types, and authorization history
- **Why it is relevant:** Helps teams map where EBT can actually be used and where food assistance infrastructure already exists
- **Access:** Public CSV download and locator tools
- **Format:** Zipped CSV and ArcGIS-compatible location data
- **How to use it:** Import into a database or map service, then calculate nearest retailers, retailer density, or overlap with low-access tracts
- **Good fit for:** `FA-01`, `FA-02`, food assistance navigation, EBT-friendly store discovery

### 4. USDA Local Food Directories

- **Link:** [Data sharing page](https://www.usdalocalfoodportal.com/fe/datasharing/)
- **Coverage:** National, searchable by state, city, ZIP code, or radius
- **What it contains:** Farmers markets, food hubs, CSAs, on-farm markets, and agritourism listings
- **Why it is relevant:** Strongest machine-readable source for local and regional food channels that are not traditional grocery stores
- **Access:** Full directory downloads or JSON API with an API key
- **Format:** Pipe-delimited CSV for bulk download and JSON arrays from directory-specific REST endpoints
- **How to use it:** Query by `city=albuquerque&state=nm`, or pre-download the directories and filter locally in your app
- **Example endpoint family:** `https://www.usdalocalfoodportal.com/api/farmersmarket/`
- **Good fit for:** local food resilience, new grower market access, `MC-01`, procurement, community-market projects

### 5. EPA Excess Food Opportunities Map

- **Link:** [Excess Food Opportunities Map](https://www.epa.gov/sustainable-management-food/excess-food-opportunities-map) and [user guide](https://www.epa.gov/sustainable-management-food/user-guide-excess-food-opportunities-map)
- **Coverage:** National, facility-level
- **What it contains:** Potential excess food generators, recipient organizations, compost sites, anaerobic digestion sites, and related food-recovery infrastructure
- **Why it is relevant:** Best public source for food rescue, donation logistics, and surplus diversion projects
- **Access:** Interactive map, downloadable exports, ArcGIS-backed services
- **Format:** Excel export, downloadable datasets, ArcGIS map services
- **How to use it:** Build generator-to-recipient matching, donation route planning, or food-waste diversion dashboards
- **Good fit for:** food waste, `DW-01`, `DW-02`, emergency food logistics

### 6. Feeding America Map the Meal Gap

- **Link:** [County data request page](https://www.feedingamerica.org/research/map-the-meal-gap/by-county) and [interactive map](https://map.feedingamerica.org/)
- **Coverage:** U.S. counties, including Bernalillo County
- **What it contains:** Food insecurity rates, counts, child food insecurity, meal cost, and budget shortfall estimates
- **Why it is relevant:** Useful when teams want a county-level need indicator rather than only tract-level access measures
- **Access:** Interactive map plus downloadable data by request
- **Format:** Web tool and request-based tabular data
- **How to use it:** Use it as a summary layer or benchmark to justify where intervention is needed
- **Good fit for:** affordability, county dashboards, food waste and rescue framing

### 7. NM-IBIS Food Insecurity And SNAP Indicators

- **Link:** [SNAP query builder](https://ibis.doh.nm.gov/query/builder/acs/ACSEconomic/FoodSNAP.html) and [food insecurity summary](https://ibis.doh.nm.gov/indicator/summary/FoodInsec.html)
- **Coverage:** New Mexico statewide with county and other local views
- **What it contains:** New Mexico-specific food insecurity and SNAP participation indicators
- **Why it is relevant:** Gives local context that is more specific to New Mexico than national summary tools
- **Access:** Public web query tools
- **Format:** Query/report interface rather than a full developer API
- **How to use it:** Export or manually collect key values into your app for New Mexico-specific comparisons
- **Good fit for:** `FA-02`, statewide context, Bernalillo County benchmarking

### 8. USDA NASS Quick Stats API

- **Link:** [Quick Stats API](https://quickstats.nass.usda.gov/api) and [API tutorial](https://quickstats.nass.usda.gov/tutorials)
- **Coverage:** National, state, county, and other geographies where available
- **What it contains:** Census of Agriculture and survey data on farm counts, acreage, production, sales, and producer demographics
- **Why it is relevant:** One of the best sources for understanding the scale, composition, and demographics of agriculture in New Mexico
- **Access:** REST API with a free API key
- **Format:** JSON, CSV, and XML outputs
- **How to use it:** Query by geography, commodity, year, and data item, then use the results for dashboards, trend charts, or local production benchmarking
- **Good fit for:** local food resilience, new growers, aging workforce, procurement, grower economics

### 9. NRCS Soil Data Access / SSURGO

- **Link:** [Soil Data Access](https://sdmdataaccess.nrcs.usda.gov/), [help](https://sdmdataaccess.nrcs.usda.gov/Help.aspx), and [spatial web services](https://sdmdataaccess.sc.egov.usda.gov/Spatial2/)
- **Coverage:** National, parcel- and soil-map-unit scale
- **What it contains:** Soil properties such as texture, drainage, depth, salinity risk, and available water capacity
- **Why it is relevant:** Especially useful for evaluating whether land is actually suitable for production, not just available on a map
- **Access:** Public web services and soil data tools
- **Format:** Tabular outputs, WMS, WFS, and downloadable SSURGO resources
- **How to use it:** Use it in a pre-processing pipeline to score parcels or candidate sites, then serve the results in your app rather than querying live for every user action
- **Good fit for:** new grower land matching, water scarcity, soil suitability, fertilizer and water-related problems

### 10. Bernalillo County Parcel Data Via Albuquerque GIS

- **Link:** [Parcel layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/AddressReport/MapServer/4)
- **Coverage:** Bernalillo County
- **What it contains:** Parcel geometry and assessor-related attributes
- **Why it is relevant:** Most practical local land-discovery dataset for projects involving lot identification, parcel scoring, land access, or site feasibility
- **Access:** Public ArcGIS REST layer
- **Format:** GIS feature service with JSON and GeoJSON-style query access
- **How to use it:** Query parcels in bulk, store them in PostGIS or a local spatial database, then enrich them with soils, zoning, and distance-to-market metrics
- **Example ArcGIS query pattern:** append `/query?where=1%3D1&outFields=*&f=json`
- **Good fit for:** `LP-01`, new grower land discovery, public-space feasibility tools

### 11. USDA Cropland Data Layer

- **Link:** [Cropland Data Layer web service](https://www.nass.usda.gov/Research_and_Science/Cropland/docs/WebService.html)
- **Coverage:** National annual cropland and land-cover coverage
- **What it contains:** Satellite-derived crop and land-cover classifications
- **Why it is relevant:** Helps teams understand what is already being grown, where farmland is active, and how land use changes over time
- **Access:** Web services and raster downloads
- **Format:** GeoTIFF, WMS/WCS-style services, image outputs, CSV/JSON stats endpoints
- **How to use it:** Use it in a geospatial pre-processing step to derive summary indicators by county, tract, or parcel
- **Good fit for:** new grower planning, aging workforce context, land-use change, large-producer climate work

### 12. New Mexico Agriculture And Food Supply Chain Atlas

- **Link:** [Atlas](https://nmfoodchainatlas.nmsu.edu/) and [data hub](https://supply-chain-data-hub-nmcdc.hub.arcgis.com/)
- **Coverage:** New Mexico statewide
- **What it contains:** Aggregators, processors, commercial kitchens, warehouses, storage facilities, transportation firms, and farmers markets
- **Why it is relevant:** One of the best New Mexico-specific sources for the “missing middle” infrastructure between growers and buyers
- **Access:** Public map tools and ArcGIS Hub resources
- **Format:** ArcGIS Hub datasets, web maps, and GIS-style resources
- **How to use it:** Use the atlas to build proximity searches, infrastructure gap maps, or routing tools for growers and buyers
- **Good fit for:** local food resilience, new growers, value-add infrastructure, procurement, distribution

### 13. USGS Water Data APIs

- **Link:** [USGS Water Data APIs](https://api.waterdata.usgs.gov/) and [daily values service details](https://waterservices.usgs.gov/docs/dv-service/daily-values-service-details/)
- **Coverage:** National with local station-level coverage
- **What it contains:** Monitoring locations, streamflow, groundwater, and daily or real-time hydrologic observations
- **Why it is relevant:** Water scarcity and water reliability are central to agriculture in New Mexico
- **Access:** Open APIs with no key required for common use
- **Format:** JSON, WaterML, and tab-delimited formats
- **How to use it:** Pull station data into a backend service, cache it, and derive alerts, risk scores, or seasonal planning indicators
- **Good fit for:** water scarcity, resilience, crop planning, grower operations

### 14. NOAA Climate Data Online

- **Link:** [API documentation](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) and [token request](https://www.ncdc.noaa.gov/cdo-web/token)
- **Coverage:** National, station-level
- **What it contains:** Temperature, precipitation, daily summaries, station metadata, and other climate observations
- **Why it is relevant:** Helpful for crop timing, weather risk, heat exposure, and long-term resilience analysis
- **Access:** REST API with a free token
- **Format:** JSON responses with pagination
- **How to use it:** Pull historical climate data for Albuquerque-area stations, derive monthly or seasonal summaries, then expose those summaries in your app
- **Rate limits:** 5 requests per second and 10,000 requests per day per token
- **Good fit for:** aging workforce planning, climate resilience, water-related problem statements

### 15. Albuquerque Civic And Place-Based GIS Layers

- **Links:** [GIS download page](https://www.cabq.gov/gis/geographic-information-systems-data), [ABQ Data](https://www.cabq.gov/abq-data), [public facilities layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer), [land use service](https://coageo.cabq.gov/cabqgeo/rest/services/agis/Land_Use/FeatureServer), [public zoning viewer](https://coagisweb.cabq.gov/Geocortex/Essentials/geo482/REST/sites/Public_Zoning_Viewer/map)
- **Coverage:** Albuquerque and surrounding local jurisdictions depending on layer
- **What it contains:** Public facilities, parks, municipal boundaries, neighborhood associations, city council districts, land use, and zoning-related context
- **Why it is relevant:** These layers are the local foundation for any civic-tech project tied to place, governance, public spaces, permits, or siting
- **Access:** Download files from the GIS portal or query ArcGIS REST services directly
- **Format:** Shapefile, KMZ, ArcGIS REST feature services, and open-data downloads
- **How to use it:** Normalize these layers into a single spatial base map for local hackathon projects, then join them to demographics, food access, or market datasets
- **Good fit for:** `MC-01`, `MC-02`, permitting, public participation, local facilities planning

## Data Formats And Integration Notes

### CSV, Excel, and tabular downloads

- Best for quick prototypes, notebooks, DuckDB, pandas, and Supabase/Postgres imports.
- Good examples: USDA Food Access Research Atlas, SNAP retailer data, USDA Local Food Directory exports.
- Recommended pattern: download once, clean the fields, and check the data into a private working area or database for your app.

### REST and JSON APIs

- Best for live lookups, narrow queries, and dynamic search experiences.
- Good examples: ACS API, USDA Local Food Directories API, NASS Quick Stats API, NOAA CDO, USGS Water Data.
- Recommended pattern: call these from a backend service, cache responses, and expose a simplified API to your frontend.

### ArcGIS REST services

- Best for maps, local public data, and feature queries with geometry.
- Good examples: Albuquerque parcel, facilities, and land-use layers; EPA map services.
- Recommended pattern: query the service directly during exploration, then export or mirror the parts you need into GeoJSON or PostGIS for production prototypes.

### GIS rasters and heavier spatial data

- Best for suitability analysis, land-cover summaries, and geospatial preprocessing.
- Good examples: Cropland Data Layer, SSURGO-derived outputs.
- Recommended pattern: preprocess the raster or soil data into tract-, parcel-, or county-level summary tables before wiring it into a web app.

## Suggested Source Combinations

- **Food access finder:** USDA Food Access Research Atlas + ACS API + SNAP retailer data
- **New grower land matcher:** Bernalillo County parcels + SSURGO + Albuquerque zoning/land use
- **Local sourcing dashboard:** NASS Quick Stats + NM Food Supply Chain Atlas + USDA Local Food Directories
- **Food rescue coordinator:** EPA Excess Food Opportunities Map + public facilities + Feeding America county context
- **Community market planner:** Albuquerque public facilities and boundaries + ACS API + USDA Local Food Directories

## Access Notes And Caveats

- Some of the strongest local sources are ArcGIS services rather than polished developer APIs. They are still useful, but teams should expect some GIS cleanup work.
- `USDA Local Food Directories`, `USDA NASS Quick Stats`, and `NOAA CDO` require an API key or token for programmatic access.
- `U.S. Census ACS API` works without a key for limited usage, but a key is recommended.
- Several local government layers are best thought of as “current operational data,” so freshness should be spot-checked before demos or production use.
- Some challenges in the sheet, especially around water rights, permitting complexity, or procurement workflow, may need partner interviews or administrative records in addition to public datasets.

## Contributing

If you find a better dataset, API, or local partner resource, open a pull request and add:

- the problem statement it supports
- the link to the source
- what the data contains
- access method and format
- one sentence on how a team could use it
