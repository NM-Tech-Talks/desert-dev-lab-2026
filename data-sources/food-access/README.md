# Food Access And Affordability Datasets

This guide supports the food-access problem statements in the working sheet, especially:

- `Food Access & Affordability`: Albuquerque's dependence on out-of-state food
- `FA-01`: neighborhood access gaps to fresh, healthy food
- `FA-02`: confusion around assistance resources during disruptions
- food waste and household affordability ideas connected to recovery and access

## Best Starting Sources

### USDA Food Access Research Atlas

- **Link:** [Food Access Research Atlas](https://www.ers.usda.gov/data-products/food-access-research-atlas/) and [download page](https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data)
- **Coverage:** U.S. census tracts
- **What it contains:** Low-income and low-access indicators, supermarket distance measures, vehicle access, and tract-level access flags
- **Why it matters:** Best starting dataset for neighborhood-level food-access mapping and “food desert” analysis
- **Access:** Bulk download and USDA geospatial services
- **Format:** Excel, ZIP, tabular data, GIS-friendly files
- **Use in an app:** Join the tract identifiers to Census boundaries, then overlay store, SNAP, transit, or population data

### U.S. Census ACS API

- **Link:** [ACS API overview](https://www.census.gov/programs-surveys/acs/data/data-via-api.html) and [example queries](https://api.census.gov/data/2020/acs/acs5/examples.html)
- **Coverage:** National, filterable to New Mexico and Bernalillo County tracts
- **What it contains:** Poverty, income, age, disability, vehicle access, internet access, rent burden, and other household characteristics
- **Why it matters:** Adds the socioeconomic context needed to understand who is most affected by access gaps
- **Access:** REST API; a key is recommended for heavier use
- **Format:** JSON API responses
- **Use in an app:** Fetch only needed variables and store a cleaned neighborhood profile table for scoring or filtering
- **Example query:** `https://api.census.gov/data/2022/acs/acs5?get=NAME,B01003_001E&for=tract:*&in=state:35&in=county:043`

### USDA SNAP Retailer Data

- **Link:** [Historical SNAP retailer data](https://www.fns.usda.gov/snap/retailer/historicaldata) and [SNAP retailer locator](https://www.fns.usda.gov/snap/retailer-locator)
- **Coverage:** National, filterable to New Mexico and Albuquerque
- **What it contains:** SNAP-authorized retailers, addresses, coordinates, retailer types, and authorization history
- **Why it matters:** Helps teams map where EBT can actually be used and where food-assistance retail infrastructure already exists
- **Access:** Public download plus locator tools
- **Format:** Zipped CSV and map-ready location data
- **Use in an app:** Import into a map or database, then calculate nearest retailers, store density, or overlap with low-access tracts

### USDA Local Food Directories

- **Link:** [Data sharing page](https://www.usdalocalfoodportal.com/fe/datasharing/)
- **Coverage:** National, searchable by city, state, ZIP code, or radius
- **What it contains:** Farmers markets, food hubs, CSAs, on-farm markets, and agritourism listings
- **Why it matters:** Useful when teams want alternatives to traditional grocery retail, especially for local-food access or market discovery
- **Access:** Bulk download or JSON API with a key
- **Format:** Pipe-delimited CSV and JSON arrays
- **Use in an app:** Query for Albuquerque-area listings or pre-filter the CSV to New Mexico before shipping it with a prototype

### NM-IBIS Food Insecurity And SNAP Indicators

- **Link:** [SNAP query builder](https://ibis.doh.nm.gov/query/builder/acs/ACSEconomic/FoodSNAP.html) and [food insecurity summary](https://ibis.doh.nm.gov/indicator/summary/FoodInsec.html)
- **Coverage:** New Mexico statewide with county-level views
- **What it contains:** New Mexico-specific food insecurity and SNAP participation indicators
- **Why it matters:** Gives a state-local framing that is more relevant to Albuquerque teams than a national dashboard alone
- **Access:** Public query interface
- **Format:** Query/report tool
- **Use in an app:** Pull key values manually or through a preprocessing script and use them as context cards or comparison metrics

## Useful Secondary Sources

### Feeding America Map the Meal Gap

- **Link:** [County data request page](https://www.feedingamerica.org/research/map-the-meal-gap/by-county) and [interactive map](https://map.feedingamerica.org/)
- **Why it matters:** Good county-level need signal when tract-level access data is too granular or teams want a high-level story
- **Best use:** Bernalillo County benchmark cards and summary dashboards

### EPA Excess Food Opportunities Map

- **Link:** [Excess Food Opportunities Map](https://www.epa.gov/sustainable-management-food/excess-food-opportunities-map)
- **Why it matters:** Useful if a team wants to connect food access to food recovery or food-waste reduction
- **Best use:** Matching food donors and recipients or mapping recovery infrastructure

## Recommended Source Combinations

- **Neighborhood access map:** Food Access Research Atlas + ACS API + SNAP retailer data
- **Assistance finder:** SNAP retailer data + NM-IBIS + Albuquerque public facilities from the civic guide
- **Local-food access tool:** SNAP retailer data + USDA Local Food Directories + ACS demographic overlays

## Integration Notes

- Start with CSV downloads if the team is short on time.
- Use live APIs only for search, filtering, or dynamic user lookups.
- For map-heavy apps, mirror raw source data into GeoJSON or PostGIS instead of calling third-party endpoints directly from the frontend.
