# PovertyComprehensive

Comprehensive Poverty map using older ArcGIS Javascript. Using table B17024 of the 5 Year ACS by census tract.

Data for map is maintained in ArcGIS Online and updated each year with the new ACS data.

To update the data:
1. Download table B17024 for all tracts in Colorado, including the MOE.
2. In the downloaded spreadsheet, create a new column for GEOID (11 digit code, 08 for Colorado, three digits for county code and 6 digits for tract code.
3. Delete the Unique ID column and the top row.
4. From a previous version of the data, copy the column headers and past them in place of the existing column headers.
5. Attach the spreadsheet to a census tract shapefile and delete unnecessary columns (everything but the geoid and data rows).
6. Upload the shapefile into ArcGIS Online.
7. Modify index.html and indiv.js in this repository to read the new data.
8. Pull the changes into the website2 docker container.

## This is one to rewrite in newer code at some point.
