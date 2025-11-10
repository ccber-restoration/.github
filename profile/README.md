## About
Repositories for research using data from the UCSB Cheadle Center's Ecological Restoration & Management Program, including the Restoration and Monitoring Mentorship Program (RAMMP).

## Spatial data 
Spatial data are generally also on ArcGIS Online: 

  - See information from the UCSB Library about accessing ArcGIS Online: https://www.library.ucsb.edu/dreamlab/spatial/arcgis-online
  - CCBER's ArcGIS Online https://ucsb.maps.arcgis.com/home/group.html?id=5196673ce5ea4d68882435ddc2f8ae3f#overview
  - See documentation for tools to integrate ArcGIS data into R workflows: https://developers.arcgis.com/r-bridge/

## Box

- For accessing continually-updated data stored on Box, consider using the boxr package: https://r-box.github.io/boxr/

## Campus Lagoon Plant List

-  Last updated in 2018, use as starter list for overall plant list for all areas managed by the Cheadle Center.
-  See https://docs.google.com/spreadsheets/d/1Ohz8c5m1lBqxH9XWiNraP3bbalaCag7DjCJmezXetsI/edit?gid=604560383#gid=604560383
-  See also:
  - Calflora https://www.calflora.org/search.html
  - Jepson eFlora https://ucjeps.berkeley.edu/eflora/
  

## Hydrology/water data
-  We have YSI readings (collected weekly via ArcGIS Survey123) on ArcGIS Online.
-  We have water level data (collected at 15 minute intervals) that is stored on Box. It requires some preprocessing.
-  COPR created a Devereux Slough Water Quality Explorer shiny app, which allows both custom visualizations and data downloads for data manually collected by COPR interns at four sites between the slough mouth and Venoco bridge. App is here: https://019a366b-24b1-1b2b-5d87-a4dcf12a2d5f.share.connect.posit.cloud/ And GitHub repository is here: https://github.com/michellemoreno18/devereux-water-data/tree/main

## eScholarship
Descriptions of data sets should also be archived on eScholarship: https://escholarship.org/uc/ccber

## Weather data

- Santa Barbara Airport (SBA) automated weather station data can be accessed via:
  - this website: https://mesonet.agron.iastate.edu/request/download.phtml?network=CA_ASOS
  - the riem R package: https://docs.ropensci.org/riem/
 
- Santa Barbara County weather data:
  - https://rain.cosbpw.net/
  - Link to excel files of daily rainfall for specific stations: https://www.countyofsb.org/2328/Daily-Rainfall-Data-XLS  
