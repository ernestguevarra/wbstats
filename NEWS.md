# wbstats v0.2.0
## Bug fixes:
* `wbdatacatalog()` now returns all catalog entries instead of first 10
* When only Namibia is queried the iso2c column now returns `"NA"` instead of logical `NA`
* For some indicators `wb()` queries would return iso3c IDs in the iso2c column. This is a behavior
  of the world bank API. This is now properly handled.

## Changes:
* Now uses Version 2 of the World Bank API.
* More explicit error messaging when encountering API call errors
* v2 of the API returns some new columns the old version didn't. Including
  data of last update for all available data sources
* update cached data in `wb_cachelist`


# wbstats v0.1.1
## Changes:
* Add 'aggregates' and 'countries_only' options to `wb()` per bapfeld pr
* update cached data in `wb_cachelist`
