# Operations, Food Rescue, And Permitting Datasets

This guide supports operational and coordination prompts, especially:

- `DW-01`: surplus food is not consistently redirected to people who need it
- `DW-02`: composting and organic waste diversion are uneven and hard to track
- `PR-01`: food entrepreneurs face permitting and registration complexity
- `PR-02`: city departments lack a shared view of food-system-related activity
- procurement-related ideas connected to local purchasing workflows

## Best Starting Sources

### EPA Excess Food Opportunities Map

- **Link:** [Excess Food Opportunities Map](https://www.epa.gov/sustainable-management-food/excess-food-opportunities-map) and [user guide](https://www.epa.gov/sustainable-management-food/user-guide-excess-food-opportunities-map)
- **Coverage:** National, facility-level
- **What it contains:** Potential excess food generators, recipient organizations, composting sites, anaerobic digestion sites, and related recovery infrastructure
- **Why it matters:** Best public source for food rescue and waste-diversion prototypes
- **Access:** Interactive map, downloadable data, ArcGIS-backed services
- **Format:** Exportable datasets, Excel downloads, map services
- **Use in an app:** Build donor-recipient matching, route optimization, or recovery-infrastructure maps

### Albuquerque Public Facilities Layer

- **Link:** [Public facilities ArcGIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer)
- **Coverage:** Albuquerque metropolitan area
- **What it contains:** Civic facilities that may overlap with service delivery or local coordination workflows
- **Why it matters:** Helpful for identifying public locations that can anchor food distribution, outreach, or service coordination
- **Access:** ArcGIS REST service
- **Format:** JSON-style feature queries
- **Use in an app:** Join with rescue or assistance data to suggest pickup, distribution, or partner locations

### ABQ Data

- **Link:** [ABQ Data](https://www.cabq.gov/abq-data)
- **Coverage:** Albuquerque
- **What it contains:** City open data across departments and operational domains
- **Why it matters:** Good starting point for permitting, process transparency, and interdepartmental coordination projects
- **Access:** Public portal
- **Format:** Mixed formats depending on dataset
- **Use in an app:** Pull relevant permit, service, or program datasets into a lightweight city-operations dashboard

### Albuquerque GIS Downloads And Zoning Resources

- **Link:** [GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data) and [public zoning viewer](https://coagisweb.cabq.gov/Geocortex/Essentials/geo482/REST/sites/Public_Zoning_Viewer/map)
- **Coverage:** Albuquerque
- **What it contains:** Location and land-use context for sites, districts, facilities, and planning layers
- **Why it matters:** Useful for permitting and operational questions that depend on where activity happens
- **Access:** Public downloads and GIS services
- **Format:** Shapefiles, KMZ, ArcGIS services
- **Use in an app:** Add siting context to a permit helper or operating-status map

## Useful Secondary Sources

### Feeding America Map the Meal Gap

- **Link:** [County data request page](https://www.feedingamerica.org/research/map-the-meal-gap/by-county)
- **Why it matters:** Helps explain where food rescue or emergency support may have the highest potential impact
- **Best use:** County-level context cards and need benchmarks

### USDA Local Food Directories

- **Link:** [Data sharing page](https://www.usdalocalfoodportal.com/fe/datasharing/)
- **Why it matters:** Useful for procurement and market-operations ideas because it exposes existing food hubs and related market actors
- **Best use:** Local vendor discovery and sourcing maps

### USDA NASS Quick Stats API

- **Link:** [Quick Stats API](https://quickstats.nass.usda.gov/api)
- **Why it matters:** Useful for procurement projects that need a rough estimate of regional production capacity
- **Best use:** Supporting analytics rather than front-line operational workflows

## Recommended Source Combinations

- **Food rescue matching tool:** EPA Excess Food Opportunities Map + public facilities + Feeding America county context
- **Permit helper:** zoning resources + ABQ Data + public facilities
- **Local procurement explorer:** USDA Local Food Directories + NM Food Supply Chain Atlas from the grower guide + NASS Quick Stats

## Integration Notes

- This cluster often needs operational rules that are not fully present in public datasets.
- Teams should expect to add assumptions or partner interviews for business rules, eligibility, pickup windows, and agency workflows.
- For permitting and coordination work, the strongest prototype may be a search, routing, or transparency tool rather than a fully automated workflow.
