# Where PEI Public Servants Live and Work (and can we get them to leave their cars at home?)

These are materials related to the [a presentation I gave](slides/agripp-slides.pdf) to the Applied Geospatial Research in Public Policy Workshop, University of Prince Edward Island, October 4, 2019.

It is an initial analysis of the home and primary work locations of provincial public servants in Prince Edward Island, Canada, with an eye to identifying opportunities to shift commuting to public transit and active transportation.

The data allowing for this analysis results from a Freedom of Information request made September 2019 to the PEI Public Service Commission and [fulfiled](foipp/Signed Decision Letter.pdf) September 27, 2019 with [data as of September 19, 2019](foipp/Postal Codes_Location 16sep19.xlsx).

## Data Files

[pei-public-servants-work-home.csv](pei-public-servants-work-home-geocoded.csv) is a CSV file extracted from the Excel sheet provided from the FOIPP request; it transforms the data to a format with one row per postal code.

[pei-public-servants-work-home-geocoded.csv](pei-public-servants-work-home-geocoded.csv) is the same CSV file, with each postal code geolocated using Canadian postal code data from [ZipCodeDownload.com](http://ZipCodeDownload.com).

## Supplementary Data

[charlottetown-bus-route-1.geojson](public_transit/charlottetown-bus-route-1.geojson) and [charlottetown-bus-route-2.geojson](public_transit/charlottetown-bus-route-2.geojson) are GeoJSON files of [Charlottetown Transit](https://t3transit.ca/) routes #1 and #2, extracted from [ReadyPass](http://charlottetown.readypass.ca/web/map).

## Limitations

* I am a Hacker in Residence, not formally trained in GIS or, really, anything.
* Canadian postal codes are not points nor polygons, but address ranges, so the ZipCodeDownload.com data used to geolocate the home addresses is necessarily imperfect.
* Rural postal codes on Prince Edward Island cover large geographic areas; my analysis focused on a single forward sortation area, C1A, in urban Charlottetown.
* Neither civic addresses nor geolocations were provided with the data received from the FOIPP request; to do additional analysis would require geocoding the work locations. Not an impossible task, but one requiring a lot of manual look-up and interpretation.

## Credits

This is a project of [Peter Rukavina](https://ruk.ca/), Hacker in Residence, [Robertson Library](http://library.upei.ca), [University of Prince Edward Island](http://upei.ca).

[Attribution-NonCommercial-ShareAlike 2.0 Generic (CC BY-NC-SA 2.0)](https://creativecommons.org/licenses/by-nc-sa/2.0/) 