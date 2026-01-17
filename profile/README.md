# About
Repositories for research using data from the UCSB Cheadle Center's Ecological Restoration & Management Program, including the Restoration and Monitoring Mentorship Program (RAMMP).

## Reproducible & Collaborative Research: 
This GitHub organization is intended to facilitate reproducible and collaborative research, following the principles of this great resource: https://ucsb-library-research-data-services.github.io/reproducible-lab/

## Setup instructions: 
If you are new to GitHub and need to connect RStudio and GitHub, follow steps 1, 2, and 4-7 in these excellent instructions from the Bren School Master of Environmental Data Science (MEDS) program: https://ucsb-meds.github.io/MEDS-installation-guide/#install

Then, follow step 16 (specifically 16.2.2) from this tutorial to connect a specific existing repository to RStudio: https://happygitwithr.com/existing-github-first 

**Repository templates**: 

- When creating new repositories for relatively straightforward/discrete research projects, please use the "repo-template" template repository: https://github.com/ccber-restoration/repo-template.

- See instructions here on basic templates: https://ucsb-library-research-data-services.github.io/reproducible-lab/github_template.html
  
- For setting up new repositories with continually-updated data, consider using the https://github.com/ccber-restoration/livedat-github-actions template (see https://www.updatingdata.org/) 


## Spatial data 
Spatial data are generally also on ArcGIS Online: 

  - See information from the UCSB Library about accessing ArcGIS Online: https://www.library.ucsb.edu/dreamlab/spatial/arcgis-online
  - CCBER's ArcGIS Online https://ucsb.maps.arcgis.com/home/group.html?id=5196673ce5ea4d68882435ddc2f8ae3f#overview
  - See documentation for tools to integrate ArcGIS data into R workflows: https://developers.arcgis.com/r-bridge/
  - TODO: would be good to implement best practices for the CCBER ArcGIS Online group, following the example of the Dangermond Restoration Group (https://ucsb.maps.arcgis.com/home/group.html?id=901ab359c49249de8ceffaa6be093057#overview)

## Box

- For accessing continually-updated data stored on Box, consider using the boxr package: https://r-box.github.io/boxr/

- To access files on Box, first follow these instructions to set up a "Box Interactive Map":
    -  https://r-box.github.io/boxr/articles/boxr-app-interactive.html#create 
    -  https://developer.box.com/guides/authentication/oauth2/oauth2-setup/
    -  Make sure to set the Redirect URI to http://localhost:1410/
-  Files and directories can be identified using file_id and dir_id, respectively, rather than filepaths.
-  Use variants of box_read() to load files on Box (e.g. csv or xlsx files) into memory: https://r-box.github.io/boxr/reference/box_read.html    

## eScholarship
Descriptions of data sets should also be archived on eScholarship: https://escholarship.org/uc/ccber

# Data sets potentially used for many projects

## Weather data

- Coal Oil Point Reserve has had a NOAA weather station since 2008 (station id 1529, see https://www.ncei.noaa.gov/access/crn/station.htm?stationId=1529) 
- Santa Barbara Airport (SBA) automated weather station data can be accessed via:
  - this website: https://mesonet.agron.iastate.edu/request/download.phtml?network=CA_ASOS
  - the riem R package: https://docs.ropensci.org/riem/
 
- Santa Barbara County weather data:
  - https://rain.cosbpw.net/
  - Link to excel files of daily rainfall for specific stations: https://www.countyofsb.org/2328/Daily-Rainfall-Data-XLS  

## Hydrology/water data
-  **Manual YSI readings** collected weekly via ArcGIS Survey123 are on ArcGIS Online.
-  **Water levels** from pressure transducers (Solinst leveloggers) at multiple locations within the slough and tributaries at 15 min intervals. Raw data files are stored on Box, as are data for each site compiled by water year.
    -  eScholarship data description (2018-2023): https://escholarship.org/uc/item/8186r0jp
    -  Dryad repository (2018-2023): https://datadryad.org/dataset/doi:10.25349/D9RP7X
    -  Zenodo repository (2018-2022): https://zenodo.org/records/8156402   
-  We have water level data (collected at 15 minute intervals at) that is stored on Box. It requires some preprocessing.
-  COPR created a Devereux Slough Water Quality Explorer shiny app, which allows both custom visualizations and data downloads for data manually collected by COPR interns at four sites between the slough mouth and Venoco bridge. App is here: https://019a366b-24b1-1b2b-5d87-a4dcf12a2d5f.share.connect.posit.cloud/ And GitHub repository is here: https://github.com/michellemoreno18/devereux-water-data/tree/main

## Campus Lagoon Plant List
-  Last updated in 2018, use as starter list for overall plant list for all areas managed by the Cheadle Center.
-  See https://docs.google.com/spreadsheets/d/1Ohz8c5m1lBqxH9XWiNraP3bbalaCag7DjCJmezXetsI/edit?gid=604560383#gid=604560383

## Species nomenclature
Try to use standardized species names (and/or codes) in Cheadle Center data sets. Some sources of authoritative/up-to-date species names:

-  **Plants**:  
    - Calflora https://www.calflora.org/search.html
    - Jepson eFlora https://ucjeps.berkeley.edu/eflora/
      
- **California herp list:** "ESTABLISHED EXTANT AMPHIBIANS AND REPTILES OF CALIFORNIA (206 SPECIES)" from the Center for North American Herpetology (CNAH): https://cnah.org/state.aspx?state=California (would be nice to find this in tabular format and confirm whether the common names are standardized/authoritative)
  
- **Mammals:** for standardized names of mammals, should use the Mammal Diversity Database (MDD), published by the American Society of Mammalogists: https://www.mammaldiversity.org/
- **Birds:** use one of the following (should only have minor differences):
  - AOS checklist of North American birds: https://checklist.americanornithology.org/
  - eBird/Clements checklist: https://www.birds.cornell.edu/clementschecklist/
  - AviList https://www.avilist.org/checklist/v2025/


