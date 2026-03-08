# Water And Climate Datasets

This guide is for teams exploring water availability, drought, irrigation risk, groundwater, reservoir conditions, and climate change impacts on agriculture in New Mexico.

This is one of the most important themes for Food & Agriculture projects in the state. A strong hackathon idea in this area could focus on:

- irrigation and planting risk
- water availability for growers
- drought early warning
- groundwater and pumping trends
- Rio Grande operations and reservoir conditions
- climate-change impacts on agricultural planning

## Best Starting Sources

### USGS Water Data APIs

- **Link:** [USGS Water Data APIs](https://api.waterdata.usgs.gov/) and [daily values service details](https://waterservices.usgs.gov/docs/dv-service/daily-values-service-details/)
- **Coverage:** National with local station-level coverage in New Mexico
- **What it contains:** Monitoring locations, streamflow, groundwater, and daily or real-time hydrologic observations
- **Why it matters:** Best starting point for real observed water conditions, especially stream gages and groundwater-related time series
- **Access:** Open APIs
- **Format:** JSON, WaterML, and tab-delimited outputs
- **Use in an app:** Pull nearby station data into a backend, cache it, and build simple risk indicators such as low-flow alerts, recent trend charts, or water-condition summaries

### New Mexico Water Data

- **Link:** [New Mexico Water Data](https://newmexicowaterdata.org/)
- **Coverage:** New Mexico statewide
- **What it contains:** A statewide hub for water-use, water-quantity, groundwater, reservoir, climate, hazard, and planning-related datasets
- **Why it matters:** Useful as a discovery layer because it brings together many New Mexico-specific sources in one place
- **Access:** Public website and dataset catalog
- **Format:** Mixed formats depending on the underlying dataset
- **Use in an app:** Use it to identify relevant state and basin-specific datasets, then pull the underlying source data into your prototype

### New Mexico Dynamic Statewide Water Budget

- **Link:** [NM Dynamic Statewide Water Budget](https://nmwrri.nmsu.edu/statewide-water-assessment/nmds-water-budget-beta-version/nmds-water-budget-beta-version.html)
- **Coverage:** New Mexico statewide with views by basin, county, and planning region
- **What it contains:** Historical and future scenario views of water use and water availability
- **Why it matters:** Strong source for teams that want to connect current agricultural stress to long-term climate and planning scenarios
- **Access:** Public web tool
- **Format:** Interactive data visualization and derived summaries
- **Use in an app:** Pull out scenario insights and summary metrics for dashboards, planning tools, or climate-risk explainers

### Bureau Of Reclamation Rio Grande Water Operations

- **Link:** [Albuquerque Water Operations](https://www.usbr.gov/uc/albuq/water/index.html) and [Rio Grande Basin status map dataset](https://catalog.newmexicowaterdata.org/dataset/rio-grande-basin-status-map)
- **Coverage:** Rio Grande Basin across Colorado, New Mexico, Texas, and Mexico
- **What it contains:** Reservoir storage, inflow, releases, precipitation, snowpack, basin conditions, and water-operations summaries
- **Why it matters:** Critical for teams focused on Rio Grande irrigation, reservoir dependence, and system-level water constraints affecting agriculture
- **Access:** Public dashboards, maps, reports, and basin-status tools
- **Format:** Web dashboards, reports, and map-based datasets
- **Use in an app:** Build status cards, seasonal operations summaries, or reservoir-condition explainers for growers and planners

### NOAA Drought.gov And Climate Datasets

- **Link:** [New Mexico drought data](https://www.drought.gov/states/new-mexico/data) and [data downloads](https://www.drought.gov/data-download)
- **Coverage:** National with New Mexico-specific views
- **What it contains:** Drought indicators, climate anomalies, precipitation departures, and GIS-ready drought datasets
- **Why it matters:** Good source for agricultural drought context and public-facing drought communication
- **Access:** Public downloads and web tools
- **Format:** GIS-ready downloads, web-ready datasets, and maps
- **Use in an app:** Add drought layers or summary indicators to a grower dashboard, planning tool, or early-warning map

## Useful Secondary Sources

### Evaporative Demand Drought Index (EDDI)

- **Link:** [EDDI](https://psl.noaa.gov/eddi)
- **Why it matters:** Measures atmospheric water demand and can provide early warning for agricultural drought
- **Best use:** Early-stress indicators for crops, irrigation, and fire-weather-adjacent risk

### NM Water Rights Reporting System

- **Link:** [NMWRRS catalog entry](https://catalog.newmexicowaterdata.org/dataset/ose-nmwrrs) and [NMWRRS](https://nmwrrs.ose.nm.gov/nmwrrs/index)
- **Why it matters:** Useful for projects dealing with water rights, points of diversion, and water administration constraints
- **Best use:** Reference layer for rights-aware planning tools, with the caveat that statewide completeness varies

### NM OSE Agricultural Groundwater Pumping

- **Link:** [Agricultural groundwater pumping dataset](https://catalog.data.gov/dataset/nmose-agricultural-gw-pumping)
- **Why it matters:** Adds pumping history for parts of the Lower Rio Grande region
- **Best use:** Trend analysis, groundwater stress storytelling, and pumping-related visualizations

### NOAA Climate Data Online

- **Link:** [API docs](https://www.ncdc.noaa.gov/cdo-web/webservices/v2) and [token request](https://www.ncdc.noaa.gov/cdo-web/token)
- **Why it matters:** Useful for station-level temperature and precipitation trends that help explain climate-change impacts on water and agriculture
- **Best use:** Historical weather summaries and climate-risk baselines

## Recommended Source Combinations

- **Irrigation risk dashboard:** USGS Water Data + Drought.gov + NOAA Climate Data Online
- **Rio Grande conditions tracker:** Bureau of Reclamation operations data + USGS gage data + drought indicators
- **Water-aware grower planner:** New Mexico Water Data + Dynamic Statewide Water Budget + NMWRRS reference data
- **Groundwater trend explorer:** Agricultural groundwater pumping + USGS groundwater or streamflow data + climate summaries

## Integration Notes

- Water data often comes from a mix of APIs, dashboards, and GIS tools rather than a single clean source.
- For a weekend prototype, precompute a small set of indicators instead of trying to expose every raw hydrology variable.
- Water-rights and irrigation-administration questions may require domain knowledge beyond what is visible in the public data.
- If a team wants a polished user experience, it is usually better to summarize the data into a few clear signals such as “drying,” “stable,” “above normal,” or “high risk.”
