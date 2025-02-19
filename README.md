***Latest version is v20250219***

# FDRA_FODR_FOD

Tool that automates the acquisition of wildfire occurrence data and preps it for use in Fire Family Plus.

### How does it work?

The tool provides users with the ability to acquire data from the [InFORM Fire Occurrence Data Records (FODR)](https://data-nifc.opendata.arcgis.com/datasets/nifc::inform-fire-occurrence-data-records/about) dataset and the [Fire Program Analysis Fire-Occurrence Database (FOD)](https://www.fs.usda.gov/rds/archive/catalog/RDS-2013-0009.6). Once acquired, the tool will merge these datasets into a consistent FODR-based schema, and intersect the points with a user provided Fire Danger Rating Area (FDRA) boundary dataset.

FODR data is selected using the user's provided date range, along with this query: "IncidenTypeCategory = 'WF' AND IncidentSize IS NOT NULL AND FireCauseID IS NOT NULL"
