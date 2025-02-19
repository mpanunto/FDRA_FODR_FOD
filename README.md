***Latest version is v20250219***

# FDRA_FODR_FOD

Tool that automates the acquisition of wildfire occurrence data and preps it for use in Fire Family Plus.

### How does it work?

Users have the option of acquiring data from the [InFORM Fire Occurrence Data Records (FODR)](https://data-nifc.opendata.arcgis.com/datasets/nifc::inform-fire-occurrence-data-records/about) dataset and the [Fire Program Analysis Fire-Occurrence Database (FOD)](https://www.fs.usda.gov/rds/archive/catalog/RDS-2013-0009.6). Once acquired, the tool will merge these products into a single dataset with a consistent FODR-based schema. The merged points will then be intersected with the user's provided Fire Danger Rating Area (FDRA) boundary dataset to attach FDRA attribution to the points.
\
\
FODR data is selected using the specified start/end dates of interest, along with this query:
- IncidentTypeCategory = 'WF' AND IncidentSize IS NOT NULL AND FireCauseID IS NOT NULL


### User inputs
1. Toggle to process FODR data
2. Option to "Download" FODR data or to "Specify Feature Class Path" of already downloaded data
3. Specify start date of FODR temporal data range
4. Specify end date of FODR temporal data range
5. Toggle to process FOD data
6. Option to "Download" FOD data or to "Specify Feature Class Path" of already downloaded data
7. Specify start date of FOD temporal data range
8. Specify end date of FOD temporal data range
9. Specify path to FDRA boundary feature class
10. Specify FDRA feature class field containing FDRA names
11. Specify Timezone of FDRAs
12. Specify Output Directory
13. Toggle to export a single output CSV, or one CSV for each FDRA
14. Toggle to add user specified start/end dates to output filenames
   
![screenshot_FDRAFODRFOD_1.png](https://github.com/mpanunto/FDRA_FODR_FOD/blob/main/screenshot_FDRAFODRFOD_1.png)



## Usage

To use this toolbox:
1. [Download the repository](https://github.com/mpanunto/FDRA_FODR_FOD/archive/refs/heads/main.zip)
2. Extract FDRA_FODR_FOD.tbx
3. Run tool using ArcGIS Pro
