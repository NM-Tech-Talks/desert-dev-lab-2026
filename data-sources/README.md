# Dataset Index

This directory breaks the hackathon source list into smaller, dataset-first guides.

## Guides

- [Food access and affordability](food-access/README.md)
- [Growers, land, water, and supply chain](growers-and-supply/README.md)
- [Markets, civic spaces, and local government](markets-and-civic-spaces/README.md)
- [Operations, food rescue, and permitting](operations-and-recovery/README.md)

## Quick Picks

If a team only has time to integrate a few sources, these are the highest-value starting points:

- [USDA Food Access Research Atlas](https://www.ers.usda.gov/data-products/food-access-research-atlas/)
- [U.S. Census ACS API](https://www.census.gov/programs-surveys/acs/data/data-via-api.html)
- [USDA SNAP retailer data](https://www.fns.usda.gov/snap/retailer/historicaldata)
- [USDA Local Food Directories](https://www.usdalocalfoodportal.com/fe/datasharing/)
- [USDA NASS Quick Stats API](https://quickstats.nass.usda.gov/api)
- [NRCS Soil Data Access / SSURGO](https://sdmdataaccess.nrcs.usda.gov/)
- [New Mexico Agriculture and Food Supply Chain Atlas](https://nmfoodchainatlas.nmsu.edu/)
- [USGS Water Data APIs](https://api.waterdata.usgs.gov/)
- [Albuquerque GIS downloads](https://www.cabq.gov/gis/geographic-information-systems-data)

## Choosing The Right Source Type

| Source type | Best for | Typical use |
| --- | --- | --- |
| CSV or spreadsheet download | Fast prototypes | Import into pandas, DuckDB, or Postgres |
| REST/JSON API | Search and live lookups | Call from a backend and cache responses |
| ArcGIS REST service | Maps and spatial queries | Export to GeoJSON or mirror into PostGIS |
| Raster or heavy GIS data | Suitability analysis | Preprocess into simpler app-friendly summaries |

## Idea Crosswalk

| Theme | Best starting guide |
| --- | --- |
| Food access and assistance | [Food access and affordability](food-access/README.md) |
| New growers, land, supply, and resilience | [Growers, land, water, and supply chain](growers-and-supply/README.md) |
| Community markets and public participation | [Markets, civic spaces, and local government](markets-and-civic-spaces/README.md) |
| Food rescue, permitting, and operations | [Operations, food rescue, and permitting](operations-and-recovery/README.md) |
