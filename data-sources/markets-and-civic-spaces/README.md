# Markets, Civic Spaces, And Local Government Datasets

This guide supports civic-tech and public-space prompts, especially:

- `Go / MC-02`: community influence over food-related public spaces
- `MC-01`: operational barriers facing community markets
- parts of `PR-01` and `PR-02` that depend on place, zoning, and city coordination

## Best Starting Sources

### Albuquerque GIS Downloads

- **Link:** [Download GIS data](https://www.cabq.gov/gis/geographic-information-systems-data)
- **Coverage:** Albuquerque and nearby local layers depending on dataset
- **What it contains:** Parks, administrative boundaries, city facilities, municipal layers, and related spatial data
- **Why it matters:** Best broad starting point for local place-based civic projects
- **Access:** Public downloads
- **Format:** Shapefile, KMZ, and other GIS-friendly formats
- **Use in an app:** Build a local basemap and join it to demographics, food access, or public comment data

### Albuquerque Public Facilities Layer

- **Link:** [Public facilities ArcGIS layer](https://coageo.cabq.gov/cabqgeo/rest/services/agis/PublicFacilities/MapServer)
- **Coverage:** Albuquerque metropolitan area
- **What it contains:** Public facilities such as community centers, libraries, and other civic locations
- **Why it matters:** Strong source for identifying places that could host food programs, markets, or engagement activities
- **Access:** ArcGIS REST service
- **Format:** JSON-style feature queries
- **Use in an app:** Add searchable civic locations to a map and score them by proximity to residents or other services

### Albuquerque Land Use And Zoning Resources

- **Link:** [Land use service](https://coageo.cabq.gov/cabqgeo/rest/services/agis/Land_Use/FeatureServer) and [public zoning viewer](https://coagisweb.cabq.gov/Geocortex/Essentials/geo482/REST/sites/Public_Zoning_Viewer/map)
- **Coverage:** Albuquerque
- **What it contains:** Land-use categories, zoning context, and siting-related planning information
- **Why it matters:** Important for understanding whether a location is realistically suited for a market, garden, kitchen, or public food activity
- **Access:** Public GIS services
- **Format:** ArcGIS feature layers and map viewers
- **Use in an app:** Use this as a site-feasibility layer before recommending locations to users

### U.S. Census ACS API

- **Link:** [ACS API overview](https://www.census.gov/programs-surveys/acs/data/data-via-api.html)
- **Coverage:** National, tract-level and other geographies
- **What it contains:** Demographics, income, age, disability, vehicle access, and household characteristics
- **Why it matters:** Lets teams connect public-space planning to who lives nearby and who may be underserved
- **Access:** REST API
- **Format:** JSON
- **Use in an app:** Add neighborhood context panels, equity filters, or population-based prioritization

### USDA Local Food Directories

- **Link:** [Data sharing page](https://www.usdalocalfoodportal.com/fe/datasharing/)
- **Coverage:** National, searchable by location
- **What it contains:** Farmers markets, food hubs, CSAs, on-farm markets
- **Why it matters:** Helps teams anchor civic-space projects to actual local food-market activity
- **Access:** Bulk download or JSON API with a key
- **Format:** Pipe-delimited CSV and JSON
- **Use in an app:** Compare current local food infrastructure to available civic spaces or neighborhoods with low participation

## Useful Secondary Sources

### ABQ Data

- **Link:** [ABQ Data](https://www.cabq.gov/abq-data)
- **Why it matters:** Good umbrella portal for city data beyond GIS-only downloads
- **Best use:** Supplemental local government data for permitting, operations, or coordination projects

## Recommended Source Combinations

- **Community market planner:** public facilities + land use/zoning + USDA Local Food Directories
- **Neighborhood influence tool:** public facilities + ACS API + administrative boundaries from Albuquerque GIS downloads
- **Public-space activation map:** parks and facilities + local markets + demographic overlays

## Integration Notes

- Most local civic datasets are better for maps and planning tools than for heavy transactional apps.
- ArcGIS REST endpoints are useful for exploration, but many teams will want to export subsets into GeoJSON for easier frontend use.
- Public-space and governance projects usually benefit from qualitative feedback data too, even when the initial prototype is map-based.
